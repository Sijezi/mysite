---
layout: default
permalink: /projects/
---
<header class="masthead">        
  <h1 class="masthead-title">
    <a href="{{ site.baseurl }}/"><span> {{site.name}}</span> Layth</a>
  </h1>
  <nav class="masthead-nav">
    {% for nav in site.nav %}
    <a href="{{ nav.href }}">{{ nav.name }}</a>
    {% endfor %}
  </nav>
</header>

Neighborhood Map | <span style="color: gray">JavaScript, HTML & CSS</span>
----------------------------------------
I developed a single-page application in KnockoutJS framework. The project features a map of my neighborhood's parks and recreational centers utilizing google maps API. I added additional functionality to this application, including: map markers to identify locations, a search function to easily discover these locations, and a list-view to support simple browsing of all locations. I also included the FourSquare API to pull important location data.



<p><img src="../img/hood.png" alt='neighborhood map" width="640"></p>
