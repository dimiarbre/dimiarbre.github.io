---
layout: page
permalink: /teaching/
title: Teaching
# description: A list of the different courses I taught in.
nav: true
nav_order: 6
calendar: true
---

I mainly teach at the [university of Rennes](https://istic.univ-rennes.fr/) and the Cyberschool in Rennes.

{% assign courses = site.teachings | sort: "order" %}
{% for course in courses %}

## [{{ course.title }}]({{ course.url | relative_url }})

_{{ course.years }}_

{{ course.description }}

{% endfor %}
