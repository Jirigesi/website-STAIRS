---
layout: page
title: People
group: "navigation"
id: "people"
---

# People

## Faculty

<div class="flex-container people image-container">
{% for person in site.data.faculty %}
  {% include person_image image=person.image caption=person.name link=person.website title=person.name %}
{% endfor %}
</div>


## PhD Students

<div class="flex-container people image-container">
{% for person in site.data.phd_students %}
  {% include person_image image=person.image caption=person.name link=person.website title=person.name %}
{% endfor %}
</div>

## Master Students
<div class="flex-container people image-container">
{% for person in site.data.master_students %}
  {% include person_image image=person.image caption=person.name link=person.website title=person.name %}
{% endfor %}
</div>

## Undergraduate Students

<div class="flex-container people image-container">
{% for person in site.data.undergraduates %}
  {% include person_image image=person.image caption=person.name link=person.website title=person.name %}
{% endfor %}
</div>

<!-- ## Alumni

<ul>
{% assign sorted_alumni = (site.data.alumni | sort:'name') %}
{% for person in sorted_alumni %}
  <li>
    {% if person.website %}
    <a href="{{ person.website }}">
      {{person.name}}
    </a>
    {% else %}
      {{person.name}}
    {% endif %}
    {% if person.at %} (now at {{ person.at }}) {% endif %}
  </li>
{% endfor %}
</ul> -->
