---
layout: home
title: Home
nav_order: 1
has_toc: false

# Set this to "false" if you removed 'previousOffering.md'
has_children: false 
---
<!-- 
This will be the home page of your module. It should give a small introduction to the student about the workshop topic.
Add, edit, or remove any content below for the workshop in question. -->

<!-- Title slide image. Replace img src with your own, or comment this out. -->
<img src="assets/img/SpecialEvents-titleSlide.png" alt="Workshop Title Slide" width="100%">

<!-- Main header -->
# Welcome to the 2025-2026 Special Events Page.

This page contains event recordings of some special events that were held in the 2025-2026 year offering.

## 2025-2026 Special Events

<div markdown="1" style="border: 1px solid #7a003c; border-radius: 6px; margin-bottom: 1em; padding: 0.5em 1em 0; margin-top: 1em;" class="toc">
<summary style="cursor:default; display: block; border-bottom: 1px solid #302d36; margin-bottom: 0.5em">
  Workshops
</summary>
<ul>
{% for workshop in workshops %}
{% if workshop.title != null and workshop.title != "Home" %}
<li><a href="{{workshop.url | absolute_url}}">{{workshop.title}}</a></li>
{% endif %}
{% endfor %}
</ul>
</div>

## Land Acknowledgement

<!-- Grabs the default SCDS land acknowledgment. If you want to use a custom one, replace this line with it. -->
{% include def/land_ack.md %}
