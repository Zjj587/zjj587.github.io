---
layout: single
title: 'Junjie Zhang \| 张骏杰'
permalink: /
author_profile: true
---

<section id="about" class="academic-section" markdown="1">

I am a master's student at **Chongqing University**, expected to graduate in **2027**. My current interests center on active vision for robotic manipulation, bio-inspired robotics, and UMI-style robot data collection.

My work spans multi-sensor fusion SLAM, LiDAR intensity simulation, and end-effector localization, combining algorithm development with datasets and benchmarking. During internships at **Shanghai AI Lab**, **PokeBot**, and **ENGINEAI**, I worked on UMI (Universal Manipulation Interface) and whole-body UMI systems. My long-term goal is to contribute to the development of **Physical AGI**.

I am actively seeking robotics research and engineering roles, PhD opportunities, and like-minded co-founders to build a robotics venture.

</section>

<section id="education" class="academic-section" markdown="1">

## Education

- **2024–2027 (expected)** — Master’s in Mechanical Engineering, **Chongqing University**.
- **2020–2024** — Bachelor’s in Mechanical Design, Manufacturing and Automation, **China University of Petroleum (Beijing)**.

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

<section id="vision" class="academic-section" markdown="1">

## Vision

I envision a future where robots help us build the world around us. I hope to find like-minded partners to turn that vision into reality.

<figure class="academic-vision__figure">
<img src="{{ site.url }}{{ site.baseurl }}/assets/vision/robot.png" alt="A robot-assisted future depicted in The Wandering Earth II" width="1698" height="612" loading="lazy" decoding="async">
<figcaption>Film still from <em>The Wandering Earth II</em> (2023).</figcaption>
</figure>

</section>
