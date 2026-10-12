---
layout: single
title: 'Junjie Zhang \| 张骏杰'
permalink: /
author_profile: true
---

<section id="about" class="academic-section" markdown="1">

Hi, I'm Junjie Zhang — a curious explorer and a pragmatic idealist in robotics.
{: .academic-introduction }

Hi, I'm **Junjie Zhang (张骏杰)**, a self-motivated researcher with a deep interest in **robotics**. I hope to witness, and contribute to, the arrival of **Physical AGI**.

[Xiaohongshu](https://www.xiaohongshu.com/user/profile/654cda6b0000000008003b9d) · [Bilibili](https://space.bilibili.com/266735709?spm_id_from=333.1007.0.0)

</section>

<section id="research" class="academic-section" markdown="1">

## Publications

<ul class="publication-list">
{% for paper in site.data.publications %}
  <li class="publication" id="{{ paper.id }}">
    <h3 class="publication__title"><a href="{{ paper.url }}">{{ paper.title }}</a></h3>
    <p class="publication__authors">{% for author in paper.authors %}{% if author == 'Junjie Zhang' %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}</p>
    <p class="publication__venue">{{ paper.venue }}</p>
    <nav class="publication__links" aria-label="Resources for {{ paper.label }}">
      {% for link in paper.links %}<a href="{{ link.url }}">{{ link.label }}</a>{% endfor %}
      <a href="{{ site.url }}{{ site.baseurl }}/assets/bib/{{ paper.id }}.bib">BibTeX</a>
    </nav>
  </li>
{% endfor %}
</ul>

</section>
