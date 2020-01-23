---
layout: home
title: Home
group: "navigation"
rank: 0
---

<div id="fb-root"></div>
<script>(function(d, s, id) {
  var js, fjs = d.getElementsByTagName(s)[0];
  if (d.getElementById(id)) return;
  js = d.createElement(s); js.id = id;
  js.src = "//connect.facebook.net/en_US/sdk.js#xfbml=1&version=v2.10";
  fjs.parentNode.insertBefore(js, fjs);
}(document, 'script', 'facebook-jssdk'));</script>

<script async defer id="github-bjs" src="https://buttons.github.io/buttons.js"></script>

<p class="lead">
Located at UC Irvine, the mission of the <b>'Software Engineering & Testing Using Artificial Intelligence for Reliable Software' (STAIRS)</b> lab is helping developers efficiently create maintainable software. With a primary focus on software engineering, we strive to create more effective techniques and tools for developing reliable, scalable, and maintainable software. Currently, one area of our research is the question of how to implement artificial intelligence techniques to analyze software evolution, as well as how software engineering can improve the quality of artificial intelligence software systems.
</p>

<p class="lead">
We are looking for highly motivated <b>PhD or Masters</b> students. Please send resumes and cover letters to iftekha@uci.edu
</p>


## Recent News
<!-- see also news.markdown -->
<style>
#RecentNews li>p {display: inline;}
</style>
<ul id="RecentNews">
{% assign news = (site.data.news | sort: 'date') | reverse %}
{% for n in news limit:4 %}
  <li>
   <span><b>{{ n.date | date: "%B %-d, %Y" }}</b></span>: {{ n.description | markdownify }}
  </li>
{% endfor %}
  <li>
   <a href="news.html">View all news</a>
  </li>
</ul>


<!-- ## Projects

{% include current_projects %} -->

&nbsp;&nbsp;

<div height="50" class="flex-container logos images-container">

<!-- <a href="http://www.nsf.gov/"> -->
<img src="{{ site.baseurl }}/images/Stairs-Logo.png" class="img-thumbnail" style="min-height:180px; height:180px;">
<!-- </a> -->

    <!-- <a href="https://uci.edu/"> -->
    <img src="{{ site.baseurl }}/images/UCI-Logo.png" class="img-thumbnail" style="min-height:100px; height:100px;">
    <!-- </a> -->

</div>
