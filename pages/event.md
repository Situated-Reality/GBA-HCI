---
layout: page
title: Past Events
permalink: /event/
---

Browse previous GBA-HCI forums, programmes and workshops.

<p lang="zh-Hans">浏览历届大湾区人机交互论坛、会议日程及工作坊。</p>

## 2026

- [GBA Pre-CHI 2026]({{ '/prechi2026/' | relative_url }}) · 21–22 March · Shenzhen · [SUSTech recap](https://designschool.sustech.edu.cn/news/893.html)

## 2025

- [Greater Bay HCI Summer School]({{ '/summerschool/' | relative_url }}) · 30 June–5 July · Shenzhen
- [GBA Pre-CHI 2025]({{ '/prechi2025/' | relative_url }}) · Conference programme

## 2024

- [GBA HCI Forum Pre-CHI 2024]({{ '/prechi2024/' | relative_url }}) · Forum archive
- [Doctoral Consortium 2024]({{ '/doctoral/' | relative_url }}) · Archived call and programme information

## Other events <span lang="zh-Hans">其他历届活动</span>

<ul>
{% for post in site.posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a> · <time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%-d %B %Y' }}</time></li>
{% endfor %}
</ul>
