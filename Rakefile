# Magnus Eriksson
# Modified from Jason Heppler
# Modified from Jeff McFadden:
# http://jeffmcfadden.com/blog/2011/04/13/rsync-your-jekyll/

## -- Config -- ##
source_dir  = "_site"
draft_dir   = "_drafts"
posts_dir   = "_posts"
stash_dir   = "_stash"
server_port = "4000"

## -- Working with Jekyll -- ##
desc 'default: list available rake tasks'
task :default do
	puts 'Try one of these specific tasks:'
	sh 'rake --tasks --silent'
end

desc 'deploy to blay.se via git'
task :deploy do
  puts 'DEPLOYING TO BLAY.SE'
  sh "time jekyll && gitta"
  puts 'Done!'
end

desc "nuke and rebuild"
task :nuke do
    sh 'rm -rf _site'
    system "jekyll"
end

desc "watch the site and regenerate when it changes"
task :watch do
  puts "Starting to watch source with Jekyll."
  system "jekyll --server --auto"
end

desc "preview site in browser with localhost:4000"
task :preview do
  puts "Starting site preview in http://localhost:4000."
  system "jekyll --server"
end

desc "give title as argument and create new post"
# usage rake write["Post Title Goes Here",category]
# category is optional
task :write, [:title, :category] do |t, args|
  filename = "#{Time.now.strftime('%Y-%m-%d')}-#{args.title.gsub(/\s/, '-').downcase}.md"
  path = File.join("_posts", filename)
  if File.exist? path; raise RuntimeError.new("Won't clobber #{path}"); end
  File.open(path, 'w') do |file|
    file.write <<-EOS
---
layout: post
title: #{args.title}
date: #{Time.now.strftime('%Y-%m-%d %k:%M:%S')}
tags:
- 
category: #{args.category}
---
EOS
    end
    puts "Now opening #{path} in subl..."
    system "subl #{path}"
end

desc "give title as argument and create new post"
# usage rake link["Post Title Goes Here", link]
# category is optional
task :link, [:title, :hreflink] do |t, args|
  filename = "#{Time.now.strftime('%Y-%m-%d')}-#{args.title.gsub(/\s/, '-').downcase}.md"
  path = File.join("_posts", filename)
  if File.exist? path; raise RuntimeError.new("Won't clobber #{path}"); end
  File.open(path, 'w') do |file|
    file.write <<-EOS
---
layout: post
title: #{args.title}
external-url: #{args.hreflink}
date: #{Time.now.strftime('%Y-%m-%d %k:%M:%S')}
tags:
- link
category: link
---
EOS
    end
    puts "Now opening #{path} in subl..."
    system "subl #{path}"
end

desc "give title as argument for draft post"
# usage rake draft["Post Title Goes Here",category]
# category is optional
task :draft, [:title, :category] do |t, args|
  filename = "#{Time.now.strftime('%Y-%m-d')}-#{args.title.gsub(/\s/, '-').downcase}.md"
  path = File.join("_drafts", filename)
  if File.exist? path; raise RuntimeError.new("Won't clobber #{path}"); end
  File.open(path, 'w') do |file|
    file.write <<-EOS
---
layout: post
title: #{args.title}
date: #{Time.now.strftime('%Y-%m-d %k:%M:%S')}
tags:
- 
category: #{args.category}
---
EOS
    end
    puts "Now opening #{path} in subl..."
    system "subl #{path}"
end
