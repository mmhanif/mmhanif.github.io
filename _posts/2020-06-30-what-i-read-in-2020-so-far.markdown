---
layout: post
title:  "What I read in 2020 (so far)"
categories: books
tags: [books, lists, 2020]
---

I've only read [17 books in 2020](#book_list). I started well, completing 10 books by the end of February, but then Covid happened. Working from home killed my reading velocity. The roughly 3 hours a day I spent commuting was my reading time. I would typically read non-fiction during the morning commute when my brain was sharp and able to absorb new ideas. On the way home, I would escape to fiction. I still haven't been able to replace that commute time with at-home reading time on a regular basis. There always seems to be something slightly more pressing to do at home than sitting down and reading a book.

In any case, my standout book so far in 2020 has been [Spillover - Animal Infections And The Next Human Pandemic]({{ site.baseurl }}{% link _posts/books/2020-05-20-spillover-animal-infections-and-the-next-human-pandemic.md %}) by David Quammen. Essential reading for a Covid-19 world.

[The Art of Statistics - How To Learn From Data]({{ site.baseurl }}{% link _posts/books/2020-01-20-the-art-of-statistics.md %}) by David Spiegelhalter was an entertaining and educational tour through the world of statistics.

I enjoyed listening to [Alchemy: The Dark Art and Curious Science of Creating Magic in Brands, Business, and Life]({{ site.baseurl }}{% link _posts/books/2020-06-29-alchemy.md %}) by Rory Sutherland. The content was thought-provoking and the narration by the author was excellent.

{% include 2020_book_stats.html %}

<div id="book_list">
<h1 id="y2020">All the books I read (or listened to) in 2020:</h1>
<ol>
{% for post in site.posts reversed %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate == "2020" %}
    {% if post.title != "What I read in 2020 (so far)" %}
      <li>
        <a href="{{ post.url }}">
          [<em>{{ post.book_type }}</em>]: <strong>{{ post.title }}</strong> by {{ post.authors }}
        </a>
      </li>
    {% endif %}
  {% endif %}
{% endfor %}  
</ol>
</div>
