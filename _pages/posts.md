---
title: "Updates"
layout: archive
permalink: /posts/
author_profile: true
lang: en
lang_switch_url: /ja/posts/
classes: wide
---

{% assign entries_layout = page.entries_layout | default: 'list' %}
{% assign posts_source = site.posts | where: "lang", "en" %}

<p>This page lists all updates in reverse chronological order.</p>

{% for post in posts_source %}
  {% include archive-single.html type=entries_layout %}
{% endfor %}
