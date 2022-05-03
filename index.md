---
layout: page
title: Software, technology, product and leadership
subtitle: Devloop
---

## <img src="../img/news.png" height="50px"> News
- [Firefox turns 100!!](https://techcrunch.com/2022/05/03/a-diminished-firefox-turns-100/) in May 2022


<div class="posts-list">
  {% for post in site.posts limit:1 %}
  <article class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
	  <h2 class="post-title">{{ post.title }}</h2>

	  {% if post.subtitle %}
	  <h3 class="post-subtitle">
	    {{ post.subtitle }}
	  </h3>
	  {% endif %}  
    </a>

    <p class="post-meta">
      Posted on {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div class="post-entry">
      {{ post.content | truncatewords: 50 | strip_html | xml_escape}}
	  <a href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</a>
    </div>

   </article>
  {% endfor %}
</div>

## <img src="../img/contact.png" height="50px"> Contact

```
Email: dhanu.gupta[at]gmail.com
```
