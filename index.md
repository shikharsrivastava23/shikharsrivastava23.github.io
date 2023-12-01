---
layout: default
---

<div class="home-page">
    <h1>My Blog</h1>
    <ul class="post-list">
        {% for post in site.posts %}
        <li class="post-list-item">
            <h2 class="post-title">
                <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
            </h2>
            <p class="post-excerpt">{{ post.excerpt }}</p>
            <p class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</p>
        </li>
        {% endfor %}
    </ul>
</div>
