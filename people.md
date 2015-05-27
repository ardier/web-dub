---
layout: main-no-sidebar
# title: "HCI & Design at the University of Washington"
current_page_item: "people"
---

## Faculty
<html>
<ul>
{% assign people = (site.people | person_has_tag: 'people-faculty' | sort: 'name') %}
{% for item_person in people %}  
  <li><a href="{{ item_person.url }}">
  {% for item_name in item_person.name offset:1 %}
    {{ item_name }}
  {% endfor %}
  {{ item_person.name[0] }}
  </a></li>
{% endfor %}
</ul>
</html>

## PhD Students
<html>
<ul>
{% assign people = (site.people | person_has_tag: 'people-phd' | sort: 'name') %}
{% for item_person in people %}  
  <li><a href="{{ item_person.url }}">
  {% for item_name in item_person.name offset:1 %}
    {{ item_name }}
  {% endfor %}
  {{ item_person.name[0] }}
  </a></li>
{% endfor %}
</ul>
</html>

## Masters Students
<html>
<ul>
{% assign people = (site.people | person_has_tag: 'people-masters' | sort: 'name') %}
{% for item_person in people %}  
  <li><a href="{{ item_person.url }}">
  {% for item_name in item_person.name offset:1 %}
    {{ item_name }}
  {% endfor %}
  {{ item_person.name[0] }}
  </a></li>
{% endfor %}
</ul>
</html>
