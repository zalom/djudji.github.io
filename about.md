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

I am a Software Engineer and a Judo coach.

I code professionally for {{professionalAge}}+ years, and been wrapping my mind around programming and concepts ever since {{everSinceYear}}!

My life included a lot of work and joy, but hardship and mistakes as well. It took me from a salesperson to a support engineer and a tour guide (a fun for seven years).

But I always wanted to be an entrepreneur and <a href="https://www.urbandictionary.com/define.php?term=indie%20hacker" target="_blank">a indie hacker </a>.

Now I am building web applications with Ruby on Rails and all sorts of JavaScript black magic. And I spend all other time coaching Judo and traveling with my wife and kid.

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

