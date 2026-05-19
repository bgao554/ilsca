---
layout: page
title: People
permalink: /people/
nav: true
nav_order: 3
---

## Faculty

{% for person in site.data.people.faculty %}
<div style="display:flex; margin-bottom:20px;">
  <img src="/assets/img/people/{{ person.photo }}" width="120" style="margin-right:20px;">
  <div>
    <b>{{ person.name }}</b><br>
    {{ person.role }}<br>
    {{ person.bio }}<br>
    <a href="mailto:{{ person.email }}">{{ person.email }}</a> |
    <a href="{{ person.website }}">Website</a>
  </div>
</div>
{% endfor %}

---

## PhD Students

{% for person in site.data.people.phd %}
<div style="display:flex; margin-bottom:20px;">
  <img src="/assets/img/people/{{ person.photo }}" width="120" style="margin-right:20px;">
  <div>
    <b>{{ person.name }}</b><br>
    {{ person.role }}<br>
    {{ person.bio }}<br>
    <a href="mailto:{{ person.email }}">{{ person.email }}</a>
  </div>
</div>
{% endfor %}

---

## Former

{% for person in site.data.people.former %}
<div style="display:flex; margin-bottom:20px;">
  <img src="/assets/img/people/{{ person.photo }}" width="120" style="margin-right:20px;">
  <div>
    <b>{{ person.name }}</b><br>
    {{ person.role }}<br>
    {{ person.bio }}<br>
    <a href="mailto:{{ person.email }}">{{ person.email }}</a>
  </div>
</div>
{% endfor %}
