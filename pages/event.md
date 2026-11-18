---
layout: page
title: Latest Event
permalink: /event/
position: 7
---

## Event archive | 历届活动

- [GBA Pre-CHI 2026]({{ '/prechi2026/' | relative_url }}) · 21–22 March 2026 · Shenzhen · [SUSTech event recap](https://designschool.sustech.edu.cn/news/893.html)
- [Greater Bay HCI Summer School]({{ '/summerschool/' | relative_url }}) · 30 June–5 July 2025 · Shenzhen
- [GBA Pre-CHI 2025]({{ '/prechi2025/' | relative_url }}) · Conference programme
- [GBA HCI Forum Pre-CHI 2024]({{ '/prechi2024/' | relative_url }}) · Forum archive

## Calendar | 活动日历

<iframe src="https://calendar.google.com/calendar/embed?src=e5437755aa56250df01f979fd86e6617caedcc076d427bd5a1b004e30bdc48dd%40group.calendar.google.com&ctz=Asia%2FShanghai" 
        style="border: 0" 
        width="100%" 
        height="600" 
        frameborder="0" 
        scrolling="no"></iframe>
<!-- <iframe src="https://calendar.google.com/calendar/embed?src=e5437755aa56250df01f979fd86e6617caedcc076d427bd5a1b004e30bdc48dd%40group.calendar.google.com&ctz=Asia%2FShanghai" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe> -->

<div class="post-cards">
  {% for post in site.posts %}
    <div class="post-card">
      <!-- Post Content -->
      <div class="post-card-content">
        <h2 class="post-card-title">
          <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <!-- <p class="post-card-excerpt">
          {{ post.excerpt | strip_html | truncatewords: 20 }}
        </p> -->
        <p class="post-card-meta"> {{ post.date | date: "%B %d, %Y" }}</p>
      </div>

      <!-- Feature Image (Square on the right) -->
      {% if post.img %}
        <div class="post-card-image" style="background-image: url('{{ post.img | prepend: site.baseurl }}');"></div>
      {% endif %}
    </div>
  {% endfor %}
</div>

<!-- Pagination (if applicable) -->
{% if paginator.pages.size > 1 %}
  <div class="pagination">
    <span class="previous">
      {% if paginator.previous_page %}
        <a href="{{ paginator.previous_page_path | prepend: site.baseurl }}">&laquo; Previous</a>
      {% else %}
        <span class="disabled">&laquo; Previous</span>
      {% endif %}
    </span>
    <span class="next">
      {% if paginator.next_page %}
        <a href="{{ paginator.next_page_path | prepend: site.baseurl }}">Next &raquo;</a>
      {% else %}
        <span class="disabled">Next &raquo;</span>
      {% endif %}
    </span>
  </div>
{% endif %}
