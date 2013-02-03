---
layout: post
title: My Writing Tools
date: 2013-02-04 00:42:12 +0100
summary: An overview of my writing tools
---

This is a post going through some of my everyday tools I use when working at the computer. I wanted to do this because I believe that the supposedly immaterial acts of thinking, writing and communicating are actually material practices. They are more akin to craftsmanship than we like to think. Not only as a means to get things done most efficiently but also. as Nietsche said, "our writing tools are also working on our thoughts". And given the amount of hours spent with these tools on a daily basis, its worth paying attention to them. I concentrate here mostly on things related to writing activities. Some of my configs and hacks for these softwares are on github so check them out (literally) over there. 

# Desktop

## Basics

### Mac lion
I use a macbook pro, right now only with OS X Lion installed. From time to time I'm thinking that I should switch to Linux and then I either dual boot or use Virtualbox to run a virtual machine, but at the moment I have given up on those thoughts. I am always ready to jump ship though since I try to use plain text[link] files organized through naming conventions [link] as much as I can, as well as free and/or cross-platform (also mobile devices) software. So I'm not so much of an Apple fan boy as this post might make me come across!

Actually, I do have my server too. A virtual machine running Debian somewhere out there. My local workflow is very tied to that machine so it deserves a mention. I keep all my sites (a few dozen!) there as well as my IRC shell. If it's down, I'm feeling down too.

### Firefox
No surprises here, never really given another browser a shot. Two extensions are crucial to my browsing; Vimperator and Pocket. 

Vimperator creates vim-style keybindings, navigation and editing so the hands never need to leave their optimal position on the keyboard, and never (for gods sake) touch the mouse or trackpad. For example, hitting 'f' displays a number for each link on the page and typing that number + enter follows that link (and 'F' to follow in a background tab). 

Pocket is a service that saves web pages to a reading list by hitting alt+w. They can then be accessed later and, especially useful, be read in a readable text-only mode that's good for distraction free reading of TL;DR blogposts.

For RSS I just use Google Reader and it's easy to save to pocket from there.

### iTerm2
I switched the original terminal.app for iTerm2 which feels good, looks good and can do some things like horizontal and vertical split windows, proper fullscreen and tabs. I'm in the terminal a lot, often with an IRC shell in one tab and another in the filesystem editing files with vim, fixing something with the blog or using todo.txt.

### Dropbox
I store all my notes in Dropbox plus some other important files its good to have backed up (not really personal information though). Dropbox is also used to sync PDFs from Zotero to an iPad where I do most of the reading and highlighting of books and articles with Goodreader.

### Yokofukurou
Yes, Twitter. Try to keep it closed as much as possible because it is too easy to just alt+TAB to it and spend/waste a few minutes reading tweets. The good thing with that is when I open it I always have too many tweets to even think about reading them all, so my Twitter following is very random and fragmented.

### preview / skim
I mostly use Preview for PDF reading, highlighting and note taking on the Mac (and Goodreader on iPad and RepliGo Reader on Android). It works really well actually. Also not bad as a simple image editor. I also have Skim installed for some special cases where it's needed, but I find its user interface a bit more combersome.

### Bunch of apps for 3D modelling and printing, coding etc.
I have other stuff for 3D and for movie and audio editing but I'm gonna skip it here.

## Some nifty things
Here are some smaller nifty apps I have that really help making things more smooth.

### Totalfinder
You can have tabs in Finder. That says it all.

### Alfred/Launchbar
I mostly use Alfred as launcher to open files, folders and applications. But I know Launchbar can do a lot more in terms of file manipulation so I might learn that instead. A launcher is a must though. One of my most used applications.

### textexpander
With Textexpander you can create macros that expand if you write a given textcombination anywhere. I mostly use it for writing "dtt" which expands to todays date in YYMMDD format. This is how all my notes filenames begin. Also useful for markdown stuff like inputting a link.

### cloudapp
Not much to it. Sits in the menu bar. Drag a file there and it will upload to cloudapp and put the link in the clipboard. Good for temporary file transfers or pasting a link to an image in IRC. My script "uppa" does sort off the same but for my own server.

### Spirited Away
Recently discovered this. Does one thing; it hides all applications that has been inactive for more than 60 seconds. You often end up only with the window you are working on not realizing how cluttered your work environment was before all the rest is gone. *poof* -- instant Zen!

### Fantastical
Great way to add new events into iCal. Click the menu bar icon, type something like "Secret meeting, Wednesday, 19-21" and it will add it with that title on that date and time. 

### 1Password
Password manager. Allows one to forget all passwords for web services and therefor be able to use really complicated ones without effort.

### App Zapper
Properly delete applications. Don't just drag from the Applications folder to the trash. Get those preferences files too!

### Clean my mac
Cleans the computer of cache and other useless files when you need more space. Hasn't crashed my whole system yet.

### Little snitch
Monitor and filter outgoing internet connections. Prevent applications from "calling home".

## Terminal scripts and aliases
I have lots of little scripts and really enjoy doing easy scripting. These are my Sudoku puzzles. Activating the brain a bit by trying to formalize and solve problems mostly having to do with making text and file manipulation easier (well, that's what computing in general is about, no?). Best way to learn the UNIX-shell and in general how to approach programming problems. 

### todo.txt
My todo-list. It's a plain text file. I comes with a script to list and manipulates it's entries in as many ways possible as you can think of form the terminal. Has apps for Android and iPhone too, synced with Dropbox. Super easy to script. My most used script is to type something like "tm 4" to schedule task number 4 to tomorrow instead of today (mañana...). Something quite beautiful when so much can be some with a simple text file. Syntax looks like this:

Plan world domination (B) +evilcorp t:2013-03-01

Where (B) is the priority and the rest is self evident.

### IRC
IRC -- a second home. Always there in the backgrond providing a warm glow and some of the best people in the world. A script lets me only type those three lovely letters in a terminal to be instantly logged in to a screen on my shell server.

### uppa
Replicates the function of Cloudapp but on the server. Takes a file name as argument, uploads it to a webfolder on my server and copies the link to the clipboard. Use it to share files.

### gitta
When I type 'gitta' (which has a funny double sense in Swedish) in the terminal and hit enter it means my blog is being updated. I upload the raw Jekyll files that then gets processed on the server to generate the site in my web folder. Have been thinking of hooking this up to a big, red button on my desk next to the computer to really get that publishing feeling [link Evan].

# Writing
The most important of all. The whole purpose of my computing life. To be able to write as freely and expressive as possible. I'm close now, very close. This is why I wanted to write this post.

## Inputs and note taking

### nvALT
NValt is the best thing that happened to quick notes since the papyrus. It is based on something really simple. An input field. Where you incrementally search you notes while you type and where if no note is found with the string you type, you only have to hit enter to create a new note with that name. 

When I got the idea of writing this post, I opened nvAlt, typed "dtt" (my textexpander macro), "-T-" (for thoughts, a category I'm using), "-bl-" (context code for this blog), and "tools", and ENTER. The file is now called "130203-T-bl-tools.txt". 

If I type "1302" in the input field it lists all notes written in Feb 2013. If I type "-bl- deleuze", it lists everything having to do with this blog containing the word 'deleuze'. If I type "-G-" (another category I'm using in file names) I get a listing of all my notes on commands, howtos, and procedures that I often use.

Everything goes in here. Every thought I feel worth noting down ends up here. And it is never lost due to the fantastic search features. When I enter it I dont have to think at all about where to store it and what to use it for. It its really a *braindump*. I also have this synced via Dropbox on my phone, so any time I am up and about and get struck by sudden profound insights, I'm just a swipe and a click away from putting it down. Incredibly useful for someone like me that can't hold a thought for more than ten seconds before it's gone.

### Markdown
A word about Markdown which is really not an application -- it is a lifestyle. I write everything in markdown syntax; notes, emails, academic papers -- I even write markdown with pen and paper! 

The syntax is so easy that you already know it. Most of it is what we all would write spontaneously in an email when writing in plain text. For example:

    # Header 1
    ## Header 2 
    ### Header 3

    - list item
    - list item 2
        - Nested list item   

    1. Ordered list
    2. Ordered list 2

    A text with *emphasis*

    > This paragraph is a block quote

    This sentence has a [link](/about.html)

    This sentence displays an ![image](/img/magnus_ansikte.jpg)

What this and some more ends up with is a syntax that is both human- and computer-readable and that can be used to generate anything from blogposts to academic articles with LaTeX. Personally, I use a dialect of markdown called Pandoc, which is also a powerful converter of markdown syntax to a wide variety of formats. My blog, which uses the Jekyll blog engine, uses a dialect called Kramdown, but they are more or less the same. 

A huge benefit with Pandoc is that it can be used to generate citations. I just have to input something along these lines:

    |[@latour1993]
    [see @kittler1999, p. 200]

...and Pandoc can generate this into citations using the citekeys of a bibtex file.

### Previous writing environments
I used to do everything in Emacs. Especially Emacs org-mode; notes, todo, long-form writing. Eventually, though I ended up realizing how locked in I was in Emacs, no matter how free the software is. It is not that the text files were in a proprietary format; they were plain text files. But the peculiar syntax of Emacs made it hard to make anything useful of the data outside of the application. It was a world of its own. Dumping emacs made me switch to the todo.txt file and to markdown, which was a huge improvement. It also made me finally learn the key bindings of Vim. Recently though I have given up on Vim (although it's my rpimary terminal editor) in favour of...

## Intermediaries

### Sublime Text 2
Omg, I don't know where to begin to describe how fantastic this editor is. Changed the way I write completely! The best thing that happend writing since...NVAlt! It has things like multiple cursors for editing similar parts of a file; a zoomed out little view of the *whole file* you are editing on the right side; it is super beautiful and lightning fast; the cool kids dig it and have made tons of plugins; it has the best incremental search since nvAlt with its file and functions search tools; fantastic search&replace and great macros for manipulating text. 

I now edit any longer text in Sublime Text 2, using Markdown syntax mostly though but also LaTeX. I can then render any type of output from there. Even wrote my own exporter for LaTeX Beamer using Pandoc as the renderer.

### Word (when I'm forced to)
Yes, I have to use it. I can't get rid of it. Other people send me .docx-files and no other application really displays them well (certainly not Libre Office). People ask me to use track changes for collaborating on documents. It is horrible.

###Scrivener (but less and less so)
I used to use Scrivener for any longer, academic writing project. It is great in many ways. Gives great overview of the whole project through the binder; the synopsis of each chapter, section or even paragraph that you can write on the index cards really help to structer the text. But I can't help feeling that Scrivener is a bit bloated for my purposes. It is after all written to aid novel writers and therefor has lots of functions for characters, scenes and screenplays that I just dont use. If there is only a way to get equally good overview in another software -- perhaps it can be implemented in Sublime Text 2 -- then I will ditch scrivener and be forever liberated by the *plain text*

## Outputs
Writing is all good, but it has to end up somewhere eventuall, doesn't it? For this I have several options, but most follows the syntax.

> input > markdown > pandoc > output

Markdown and Pandoc are the "obligatory points of passage" in my textual flow.

### Pandoc
I have already talked some about using Pandoc as a Markdown dialect, but as I said, it is also a Markdown processor capable of rendering a wide variety of file formats.

Well, these actually:

> It can read markdown and (subsets of) Textile, reStructuredText, HTML, LaTeX, MediaWiki markup, and DocBook XML; and it can write plain text, markdown, reStructuredText, XHTML, HTML 5, LaTeX (including beamer slide shows), ConTeXt, RTF, DocBook XML, OpenDocument XML, ODT, Word docx, GNU Texinfo, MediaWiki markup, EPUB (v2 or v3), FictionBook2, Textile, groff man pages, Emacs Org-Mode, AsciiDoc, and Slidy, Slideous, DZSlides, or S5 HTML slide shows. It can also produce PDF output on systems where LaTeX is installed.
> 
> [Pandoc User's Guide](http://johnmacfarlane.net/pandoc/README.html)

In its easiest setup you just specify an output file and an input file

    pandoc text.markdown -o text.html

In its more complicated shape, such as rendering a PDF, you can also specify a Tex-template, a CSL-bibliography style file and your Bibtex bibliography file. Here is how I rendered a recent paper for my PhD course:

    pandoc -s -S --template=/Users/svartfax/Dropbox/bibtex/template.tex --csl=/Users/svartfax/Dropbox/bibtex/chicago-note.csl --biblio=/Users/svartfax/Documents/library/zot.bib -o matkursnote.pdf matkurspaper.markdown 

Yes, the user on my computer is called 'svartfax'.

### Texshop
Sometimes the straight-from-pandoc-to-pdf model don't really work and the file needs some extra tweaking. Then I somply use pandoc to generate a .tex-file and then open up TexShop, make the final edits, additions to the preamble or other LaTeX magic and then it's good to go. I never start with pure LaTeX though because Markdown is so superior in creating quick, easily readable documents.

### Beamer
Recently I have ditched another heavily, frustratingly complex type of software -- the presentation software. No more Keynote with files over 100mb. I have gone where I never thought I would venture -- into *Beamer territory*. Beamer is a document class for LaTeX to generate presentations in the form of PDFs or other slide formats. If you do an image search for "LaTeX Beamer" you will see lots of screenshots of presentations filled with *TONS* of math formulas and *HORRIBLE* aesthetics. But it is really simple to create an outline of a presentation in Pandoc (you can for example start with the headers of the paper you are presenting) and then just tweak it a bit in TexShop to create some final touches. And I actually found some nice looking themes, for example the [Kalgan theme](https://github.com/kartikprabhu/Kalgan-Mule-template).

The benefit of using Beamer -- apart from huge nrrd cred -- is that the files are extremely lightweight, easy to re-edit and videofiles and images can be reused instead of stored within each file.

# Bibliography management

## Zotero
I have tried a bunch of bibliography managers in my days. Often they did one thing well, but were frustratingly poor in other aspects. But now I'm pretty sure I found one that is a keeper. 

First, let me paint the picture of my situation. At the moment of writing I have 1470 references in my database and about a hundred more I haven't gotten around to sorting yet. I have three major requirements on a bibliography manager:

1. It should be easy to enter references, their metadata and link to PDFs
2. It should be easy to browse, tag and search the references
3. It should play well with Bibtex (so I can use it with LaTeX)

The one I have now found that does this and a whole lot more is Zotero, a free manager developed with some kind of academic funding. From the beginning it was a Firefox plugin (that I didn't like at all) but now it has a standalone application for Mac, Linux and Windows. It is extendable through plugins (get zotfile. Essential!). The application looks nothing fancy really, but it does the job *well*.

Entering references is a breeze with the firefox plugin. Just go to the site of a reference (directly from a journal or from an aggregator) and hit the little icon that shows in the adressbar. It fetches the meta-data and you can easily drag a PDF there that gets renames (with zotfile) and sent to your library folder. 

Zotero also has a great tagging system (just drop references on your tags in the bottom left) and it can extract the highlights and notes form a PDF into a searchable textfile attached to the reference. Actually, it can even send PDFs to a Dropbox folder and monitor them for when they get back (from being annotated in Goodreader on the iPad) and incorporate them again with extracted notes. 

You need a customizable bibtex-exporter to get the citekeys right (in authoryear format) but then it plays nicely with bibtex.

## Bibtex
When it's time to put the references in the oven, I export the library into a .bib file, then either use TexShop or Pandoc to render a PDF form the .tex file and the .bib file. 

In the pandoc example above, you saw that I am using a CSL-style file that is based on the Chicago Fullnote style that I have modified a bit. That is for footnotes[^1], and I usually use an APA style for (author year) refernces inline. 

By the way, to get the references rendered nicely with pandoc, just put this at the bottom of your markdown file:

    #References

    \setlength{\parindent}{0in}
    \setlength{\leftskip}{0in}
    \setlength{\parskip}{8pt}

[^1]: Like this!

# Blogging
Well, I saved the best for last, didn't I. This might come as a surprise for some in these days of Wordpress: my blog consists of static .html-files. No php, no mysql database.

These static html-files are rendered from (you guessed it...) Markdown files using the wonderful Jekyll, a static blog generator. 

Why use a static blog? The reasons are many and there I only list a few:

- I have a local copy of my whole blog in plain text files ready to be searched, edited and manipulated.
- I can copy and backup my blog by just copying a folder.
- It has no database can become corrupted when updating or that I forget the password to.
- It is easy, simple and beautiful.
- Very easy to customize, only a few files to tweak.

I'm not gonna list more, but I highly recommend it if you plan to manage your own blog. 

The workflow should be evident by now:

> Thought > nvALT > Sublime Text 2 > (pandoc if I use bibtex) > Jekyll > gitta > Blog

Well, that's about it folks. These are the tools I use to perform my craft. As I said, go to my Github and get config files for anything you might like of this. And feel free to contact me with questions or suggestions. I'm on Twitter, Email, or IRC :)
