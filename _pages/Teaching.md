---
layout: archive
permalink: /Teaching/
title: "Teaching"
author_profile: true
header:
	image:  "/images/screenshot.png"
--- 
<dl>
	 
  <dt><font size="3">Teaching Assistant, Humphrey School of Public Affairs, University of Minnesota, Fall 2015</font></dt>
  <dd>PA 5022/5390 Economics for Policy Analysis and Planning II: Topics in Advanced Policy Analysis Methods.</dd>

 
  <dt><font size="3">Teaching Assistant, Humphrey School of Public Affairs, University of Minnesota, Fall 2013</font></dt>
  <dd>PA 5790/5022 Economics For Policy Analysis and Planning: Material-Energy Flows and Society.</dd>


{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}