---
layout: default
title: Home
---


# 🐸 Welcome to **Yikepedia**

_An encyclopedia for the culture, informed by Claire._

---

Does Claire give you some fire reccomendations? Do you find yourself taking notes, but struggling to get in all the information? Look no further than the Yikepedia. Currated with all of Claire's top picks in resteraunts, bars, cafes, and other places, you now have a consolidated place to explore all of the amazing recomendations that she gives. Take a look around. There is always more coming!

---

## Contents

<div class="sections-nav">
  • <a class="section-link" href="{{ '/restaurants' | relative_url }}"> Restaurants</a> •
  <a class="section-link" href="{{ '/cafes' | relative_url }}"> Cafes</a> •
  <a class="section-link" href="{{ '/bars' | relative_url }}"> Bars</a> •
  <a class="section-link" href="{{ '/museums' | relative_url }}"> Museums</a> • 
  <a class="section-link" href="{{ '/parks' | relative_url }}"> Parks</a> •
  <a class="section-link" href="{{ '/meals' | relative_url }}"> Home Cooked Meals</a>
</div>

---

## Featured Articles

<table class="featured-table">
  <tr>
    {% assign shuffled_articles = site.articles | sample: 3 %}
    {% for article in shuffled_articles %}
    <td>
      <img src="{{ article.image | relative_url }}" alt="{{ article.image_alt }}">
      <div class="caption">
        <a href="{{ article.url | relative_url }}">{{ article.title }}</a>
      </div>
      <p>{{ article.excerpt | strip_html | truncate: 120 }}</p>
    </td>
    {% endfor %}
  </tr>
</table>



---

## Suggestions?

If you think something should be added to the site, just text me :)
