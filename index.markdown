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
The <b>Software Engineering & Testing Using Artificial Intelligence for Reliable Software</b> lab, located at UC Irvine, tries to develope and come with better tools and techniques to develope more reliable, scalable, and maintable softwares. We use artificial intelligence to analyze software evolution.
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


## Current Projects

{% include current_projects %}

&nbsp;&nbsp;

<div height="50" class="flex-container logos images-container">

<!-- <a href="http://www.nsf.gov/"> -->
<img src="{{ site.baseurl }}/images/Stairs-Logo.png" class="img-thumbnail" style="min-height:180px; height:180px;">
<!-- </a> -->

    <!-- <a href="https://uci.edu/"> -->
    <img src="{{ site.baseurl }}/images/UCI-Logo.png" class="img-thumbnail" style="min-height:120px; height:120px;">
    <!-- </a> -->

</div>
