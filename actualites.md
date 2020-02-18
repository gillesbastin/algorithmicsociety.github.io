---

layout:		default
title:  	Actualités
type:		page
navigation: 	true
details:        true

date:   	2019-10-13
excerpt: 	"Retrouvez sur cette page toutes les actualités de la chaire postées sur le site."
gradient: 	2
image: 		header-1.jpg

---

<div class="home-page">
        {% for post in site.posts offset: site.pagination + 1 %}
        <ul>
        <li>
            <span class="date">{{ post.date | date: "%Y-%m-%d" }}</span> | <a class="link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </li>
        </ul>
        {% endfor %}
</div>
