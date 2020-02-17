---

layout:     default
title:      Bienvenue
type:       page
navigation: false
details:    true

date:       2019-10-14
image:      header-1.jpg
excerpt:    "La chaire Société algorithmique est une des chaires de recherche de l'institut <b>MIAI</b> (Multidisciplinary Institute in Artificial Intelligence) de l'Université Grenoble Alpes"
gradient:   2

---

La chaire Société algorithmique conduit des recherches sur le tournant algorithmique de la société contemporaine. Elle étudie l'intelligence artificielle dans ses contextes sociaux, soutient la recherche multidisciplinaire sur les biais de l'intelligence artificelle et favorise le développement d'une litératie algorithmique parmi les étudiants en sciences sociales.

<hr>

<h2>Actualité</h2>
<p>Voir la rubrique « Archive » pour retrouver l'ensemble des actualités postées sur ce site.</p>

<ul class="post-list">
{% for post in site.posts limit:site.pagination %}
      <span class="post-meta">{{ post.date | date: "%d %b %Y" }}
      </span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
          {{ post.title }}
        </a>
      <br>
{% endfor %}
</ul>
