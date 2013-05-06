---
layout: default
title: Research
---
# Thesis

My thesis is on the role of software in the regulation of urban space. It is an attempt to think digital technologies as material and spatial phenomena in order to better grasp the agency and normativity of emerging technologies that mediate between code and urban environments. I am especially interested in how urban space and physical activities are regulated and structured to ensure the functioning, capture and compliance with software systems.


The thesis is performed in a joint venture between the department of sociology of law at Lund University, Sweden and the University of Macerata, Italy with beginning spring 2013.

# Papers

### Internauts, Punks and Infrastructure. 

- [PDF](/papers/punks.PDF), [HTML](/2011/10/06/punks/)
- *From Consuming the Illegal. Leuwen, Belgium. March 2011.*

### Labbet utan egenskaper. 

- [PDF](/papers/labbet.pdf), [HTML](/papers/labbet.html)
- *Master thesis in sociology. Lund University. June 2011.*

### Kod och Materialitet / Materialization of Code
- [PDF SWEDISH](/papers/kod_och_materialitet.pdf), [PDF ENGLISH](/papers/materialization_of_code.pdf)
- *Paper from Phd course. Gothenburg University. Fall 2012.*

# Long posts and presentations

<ul class="listing">
    {% for post in site.categories.tldr %}
      <li>
        <span>{{ post.date | date: "%B %e, %Y" | ordinalize  }}</span>
        <a href="{{ post.url }}">{{ post.title }}</a>
    <br>
    <div class="summary">{{ post.summary }}</div>
    </li>
    {% endfor %}
</ul>