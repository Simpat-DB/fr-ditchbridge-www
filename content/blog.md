---
layout: default
title: DitchBidge
description: >-
  Ce site est 

navigation:
  - title: L'offre
    url: /product
  - title: La societé
    url: /company
  - title: Les equipes
    url: /team
  - title: Nous rejoindre
    url: /recrutement
  - title: Nos valeurs
    url: /values
  - title: Blog
    url: /
  - title: Tags
    url: /tags
  - title: About
    url: /about
social:
paginate: posts
---

<!-- Introduction Section 
<div class="intro">
  <h1>{site.data.greeting}</h1>
  <p>{site.data.tagline}</p>
</div>
-->

<!-- Posts Section -->
<div class="posts">
  <h3>Blog</h3>
  <div class="posts-wrapper">
    {#for post in site.collections.posts.paginated(page.paginator)}
    {#postCard post site/}
    {/for}
  </div>

  {#include partials/posts-paginator /}
</div>