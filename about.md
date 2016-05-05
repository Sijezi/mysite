---
layout: default
permalink: /about/
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
<div class="content list">
{about.md}
</div>
