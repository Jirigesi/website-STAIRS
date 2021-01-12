---
layout: page
title: News
group: "navigation"
id: "news"
---
## News
<!-- see also index.markdown -->
<style>
 #RecentNews li>p {display: inline;}
</style>
<ul id="RecentNews">
{% assign news = (site.data.news | sort: 'date') | reverse %}
{% for n in news %}
  <li>
   <span><b>{{ n.date | date: "%B %-d, %Y" }}</b></span>: {{ n.description | markdownify }}
  </li>
{% endfor %}
</ul>

&nbsp;&nbsp;

<div height="50" class="flex-container logos images-container">

<!-- <a href="http://www.nsf.gov/"> -->
<img src="{{ site.baseurl }}/images/Stairs-Logo.png" class="img-thumbnail" style="min-height:180px; height:180px;">
<!-- </a> -->

<!-- <a href="https://uci.edu/"> -->
<img src="{{ site.baseurl }}/images/UCI-Logo.png" class="img-thumbnail" style="min-height:100px; height:100px;">
<!-- </a> -->

</div>