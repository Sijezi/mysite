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

Neighborhood Map | <span style="color:  #D85950">JavaScript, HTML & CSS</span>
----------------------------------------
I developed a single-page application in KnockoutJS framework. The project features a map of my neighborhood's parks and recreational centers utilizing google maps API. I added additional functionality to this application, including: map markers to identify locations, a search function to easily discover these locations, and a list-view to support simple browsing of all locations. I also included the FourSquare API to pull important location data.

* * *


[![map](../img/hood.png)](http://wehelie.github.io/neighborhood-map-project/)

* * *

UdaciFeeds: Feed Reader Testing | <span style="color:  #D85950">Jasmine</span>
----------------------------------------

Used the red-green-refactor workflow to develop the UdaciFeeds project. I was given a web-based application that reads RSS feeds. The original developer of this application included Jasmine, but with incomplete test suites. I completed all the required tests by: 

- <span style="color: #D85950">Validating opinions</span>
- <span style="color: #D85950">Identifying and defining expectations</span> 
- <span style="color: #D85950">Writing expectations in code</span>

* * * 

[![feed reader](../img/udacifeed.png)](http://wehelie.github.io/feed-reader/)

* * * 

Website Optimization | <span style="color:  #D85950">JavaScript, HTML & CSS</span>
----------------------------------------
I resolved a number of optimization and performance related issues so that the provided application can achieve a target PageSpeed score and run 60 frames per second. Through this project, I discovered easy-to-implement performance gains while also developing a simple and a powerful model for uncovering optimization opportunities.

* * * 

[![performance](../img/perf.png)](http://wehelie.github.io/projectfour/)

* * * 

Classic Arcade Game Clone  | <span style="color:  #D85950">JavaScript, HTML5 & CSS</span>
----------------------------------------

* * * 

Provided with visual assets and a game loop engine, I used Object-Oriented Javascript and HTML5 Canvas to add a number of entities to the game. This included the player characters and enemies to recreate the classic arcade game Frogger.

* * * 


