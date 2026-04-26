---
title: "更新情報"
layout: archive
permalink: /ja/posts/
author_profile: true
lang: ja
lang_switch_url: /posts/
classes: wide
---

{% assign entries_layout = page.entries_layout | default: 'list' %}
{% assign posts_source = site.posts | where: "lang", "ja" %}

<p>このページでは更新情報を新しい順に一覧表示しています。</p>

{% for post in posts_source %}
  {% include archive-single.html type=entries_layout %}
{% endfor %}
