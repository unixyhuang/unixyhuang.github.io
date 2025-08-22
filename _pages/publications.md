---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 2

# 按需补充/修改
pubs:
  - tag: "SenSys ’25"
    year: "2025"
    title: "GPIoT: Tailoring Small Language Models for IoT Program Synthesis and Development"
    author: "Leming Shen, Qiang Yang, **Xinyu Huang**, Zijing Ma, Yuanqing Zheng"
    booktitle: "SenSys 2025, May 6–9, 2025, Irvine, USA"
    url: "https://dl.acm.org/doi/10.1145/3715014.3722064"
    link: "https://dl.acm.org/doi/10.1145/3715014.3722064"
    pdf: ""
    abs: ""

  - tag: "Journal"
    year: "2024"
    title: "GD3N: Adaptive Clustering-Based Detection of Selective Forwarding Attacks in WSNs under Variable Harsh Environments"
    author: "Haozhen Wang, **Xinyu Huang**, Yuanming Wu"
    type: "Journal Paper"
    booktitle: "Information Sciences, 2024"
    url: "https://www.sciencedirect.com/science/article/pii/S0020025524002883"
    link: "https://www.sciencedirect.com/science/article/pii/S0020025524002883"
    pdf: ""
    abs: ""

  - tag: "Journal"
    year: "2023"
    title: "LSTM-NV: A Combined Scheme against Selective Forwarding Attack in Event-Driven Wireless Sensor Networks under Harsh Environments"
    author: "**Xinyu Huang**, Shunan Li, Yuanming Wu"
    type: "Journal Paper"
    booktitle: "Engineering Applications of Artificial Intelligence, 2023"
    url: "https://www.sciencedirect.com/science/article/pii/S0952197623006255"
    link: "https://www.sciencedirect.com/science/article/pii/S0952197623006255"
    pdf: ""
    abs: ""

  - tag: "Journal"
    year: "2022"
    title: "Identify Selective Forwarding Attacks Using Danger Model: Promote the Detection Accuracy in Wireless Sensor Networks"
    author: "**Xinyu Huang**, Yuanming Wu"
    type: "Journal Paper"
    booktitle: "IEEE Sensors Journal, 2022"
    url: "https://ieeexplore.ieee.org/abstract/document/9755128"
    link: "https://ieeexplore.ieee.org/abstract/document/9755128"
    pdf: ""
    abs: ""
---

<style>
/* 容器与配色（深色系，可按站点主题微调） */
.pub-card{
  display:grid;
  grid-template-columns: 120px 1fr 90px; /* 左：会议名；中：详情；右：年份 */
  gap:18px;
  padding:20px;
  margin:18px 0;
  border:1px solid #22262e;
  border-radius:12px;
  background:linear-gradient(180deg,#14171c,#0f1318);
}
.pub-left{display:flex;align-items:flex-start;justify-content:flex-start}
.pub-pill{
  background:#2b2f38;border:1px solid #3a404d;color:#cbd5e1;
  border-radius:999px;padding:6px 10px;font-size:12px;font-weight:700;letter-spacing:.2px
}
.pub-title{margin:0 0 6px;font-size:20px;font-weight:700;line-height:1.3}
.pub-authors{margin:4px 0}
.pub-venue{margin:6px 0 12px;color:#9aa3af;font-size:14px;font-style:italic}
.pub-btns{display:flex;gap:8px;margin:6px 0 0}
.pub-btn{
  border:1px solid #343a46;background:#2a2f39;color:#d1d5db;
  padding:6px 12px;border-radius:8px;font-size:12px;font-weight:600;text-decoration:none
}
.pub-btn:hover{border-color:#485063}
.pub-abs{border:1px dashed #3a404d;border-radius:10px;padding:10px;margin-top:12px;background:#12151a}
.pub-year{grid-column:3;grid-row:1;color:#64748b;font-weight:800;font-size:26px;justify-self:end}
@media (max-width: 820px){
  .pub-card{grid-template-columns:100px 1fr}
  .pub-year{display:none}
}
</style>

# Selected Papers

{% for pub in page.pubs %}
{% unless pub.hidden %}
<article class="pub-card">
  <div class="pub-left">
    <span class="pub-pill">{{ pub.tag }}</span>
  </div>

  <div>
    <h2 class="pub-title">
      {% if pub.url %}<a href="{{ pub.url }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}
    </h2>

    <div class="pub-authors">{{ pub.author }}</div>

    <div class="pub-venue">
      {{ pub.booktitle }}{% if pub.type %} ({{ pub.type }}){% endif %}
    </div>

    <div class="pub-btns">
      {% if pub.link %}<a class="pub-btn" href="{{ pub.link }}">LINK</a>{% endif %}
      {% if pub.pdf and pub.pdf != "" %}<a class="pub-btn" href="{{ pub.pdf }}">PDF</a>{% endif %}
    </div>

    {% if pub.abs and pub.abs != "" %}
    <div class="pub-abs">{{ pub.abs }}</div>
    {% endif %}
  </div>

  <div class="pub-year">{{ pub.year }}</div>
</article>
{% endunless %}
{% endfor %}

