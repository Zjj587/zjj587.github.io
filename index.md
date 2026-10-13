---
layout: single
title: 'Junjie Zhang \| 张骏杰'
permalink: /
author_profile: true
---

<section id="about" class="academic-section" markdown="1">

I am a master's student at **Chongqing University**, expected to graduate in **2027**. My current interests center on active vision for robotic manipulation, bio-inspired robotics, and UMI-style robot data collection.

My work spans multi-sensor fusion SLAM, LiDAR intensity simulation, and end-effector localization, combining algorithm development with datasets and benchmarking. During internships at **Shanghai AI Lab**, **PokeBot**, and **ENGINEAI**, I worked on UMI (Universal Manipulation Interface) and whole-body UMI systems. My long-term goal is to contribute to the development of **Physical AGI**.

[Xiaohongshu](https://www.xiaohongshu.com/user/profile/654cda6b0000000008003b9d) · [Bilibili](https://space.bilibili.com/266735709?spm_id_from=333.1007.0.0)

</section>

<section id="research" class="academic-section" markdown="1">

## Publications

<ul class="publication-list">
{% for paper in site.data.publications %}
<li class="publication{% unless paper.image %} publication--text-only{% endunless %}" id="{{ paper.id }}">
{% if paper.image %}<a class="publication__media" href="{{ paper.url }}" aria-label="Read {{ paper.title }}"><img src="{{ site.url }}{{ site.baseurl }}/{{ paper.image }}" alt="{{ paper.image_alt }}" loading="lazy" decoding="async"></a>{% endif %}
<div class="publication__content">
<h3 class="publication__title"><a href="{{ paper.url }}">{{ paper.title }}</a></h3>
<p class="publication__authors">{% for author in paper.authors %}{% if author == 'Junjie Zhang' %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}</p>
<p class="publication__venue">{{ paper.venue }}</p>
<nav class="publication__links" aria-label="Resources for {{ paper.label }}">
{% for link in paper.links %}<a href="{{ link.url }}">{{ link.label }}</a>{% endfor %}
<a href="{{ site.url }}{{ site.baseurl }}/assets/bib/{{ paper.id }}.bib">BibTeX</a>
</nav>
</div>
</li>
{% endfor %}
</ul>

</section>
