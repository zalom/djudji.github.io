---
layout: about
title: About
permalink: /about/
tags: about
flicker: true
headshot: /images/headshot.jpg
---

{% assign currentYear = site.time | date: '%Y' %}
{% assign sinceYear = 2015 %}
{% assign everSinceYear = 1999 %}
{% assign professionalAge = currentYear | minus: sinceYear %}

I am a <a href="#" class="highlighted-link">Software Engineer</a> and a <a href="#" class="highlighted-link">Judo coach</a>.

I code professionally for <a href="#" class="highlighted-link">{{professionalAge}}+</a> years, and I've been wrapping my mind around programming and concepts ever since {{everSinceYear}}!

My life included a lot of work and joy, but hardship and mistakes as well. It took me from a <a href="#" class="highlighted-link">salesperson</a> to a <a href="#" class="highlighted-link">support engineer</a> and a <a href="#" class="highlighted-link">tour guide</a> (a fun for seven years) to where I am at right now.

But I always wanted to be an <a href="#" class="highlighted-link">entrepreneur</a> and an <a href="https://www.urbandictionary.com/define.php?term=indie%20hacker" target="_blank" class="highlighted-link">indie hacker</a>.

Now I am building web applications with <a href="https://rubyonrails.org/" class="highlighted-link">Ruby on Rails</a>  and all sorts of <a href="#" class="highlighted-link">JavaScript</a>  black magic. And I spend all other time coaching Judo and traveling with my wife and kid.

{% if site.show_talks_section %}
## Talks

- Put something here!
{% endif %}

{% if site.show_workshops_section %}
## Workshops

- Put something here!
{% endif %}


<style>
.post-header, .post-content, #talks, #workshops {
  text-align: center; /* Want the About Page header to be in the middle */
}
</style>

