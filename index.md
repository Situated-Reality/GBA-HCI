---
layout: home
---

<h1>About | 关于我们</h1>

<div class="logo-grid">
{% assign logos = 'CityUHK Logo.webp|SUSTech.webp|PolyU.webp|STU.webp|HKUST(GZ).webp|UM.png|HKUST.webp|SYSU.webp|SZU.webp|JNU_logo.webp' | split: '|' %}
{% assign names = 'City University of Hong Kong|Southern University of Science and Technology|The Hong Kong Polytechnic University|Shantou University|The Hong Kong University of Science and Technology (Guangzhou)|University of Macau|The Hong Kong University of Science and Technology|Sun Yat-sen University|Shenzhen University|Jinan University' | split: '|' %}
{% for logo in logos %}
    <div class="logo-grid-item">
        <img src="{{ '/assets/img/' | append: logo | relative_url | uri_escape }}" alt="{{ names[forloop.index0] | escape }}" />
    </div>
{% endfor %}
</div>

Greater Bay HCI is a network of human–computer interaction researchers at universities and research institutions across the Guangdong–Hong Kong–Macao Greater Bay Area. The community hosts forums, workshops, seminars and conference meetups to share research and connect researchers, practitioners and the public.

<p lang="zh-Hans">粤港澳大湾区人机交互论坛汇集来自区内高校和研究机构的人机交互研究者。论坛通过学术会议、工作坊、研讨会和会议交流活动，促进研究交流，并联系学界、产业界与公众。</p>

## Events | 活动

- [GBA Pre-CHI 2026]({{ '/prechi2026/' | relative_url }}) · 21–22 March 2026 · SUSTech · [Event recap](https://designschool.sustech.edu.cn/news/893.html)
- [Greater Bay HCI Summer School]({{ '/summerschool/' | relative_url }}) · 30 June–5 July 2025 · Shenzhen
- [GBA Pre-CHI 2025]({{ '/prechi2025/' | relative_url }}) · Conference programme
- [GBA HCI Forum Pre-CHI 2024]({{ '/prechi2024/' | relative_url }}) · Forum archive

## Activities | 学术交流

- **Pre-CHI Symposium | 年度 Pre-CHI 论坛** · A venue for researchers to present and discuss HCI work ahead of ACM CHI.
- **Doctoral Consortium | 博士生学术论坛** · Research feedback and mentorship for doctoral students.
- **Confluence Seminars | 湾区智汇系列讲座** · Research talks and discussions involving researchers and industry practitioners.
- **Research exchange | 学术互访** · Visits and exchanges among participating research groups.

## Contact | 联系我们

For collaboration, sponsorship and new initiatives, contact Xiang Li (The University of Hong Kong) at [xianghci@hku.hk](mailto:xianghci@hku.hk).
