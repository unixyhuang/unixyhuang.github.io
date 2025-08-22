---
layout: page
permalink: /publications/
title: 
description:
nav: true
nav_order: 2

pubs:
  - tag: "SenSys ’25"
    type: "Conference"
    year: "2025"
    title: "GPIoT: Tailoring Small Language Models for IoT Program Synthesis and Development"
    author: "Leming Shen, Qiang Yang, <u><b>Xinyu Huang</b></u>, Zijing Ma, Yuanqing Zheng"
    booktitle: "SenSys 2025, May 6–9, 2025, Irvine, USA"
    acceptance_rate: "19.6%"
    url: ""
    link: "https://dl.acm.org/doi/10.1145/3715014.3722064"
    pdf: ""
    slides: ""
    bibtex: ""
    abs: ""

  - tag: "Journal"
    type: "Journal"
    year: "2024"
    title: "GD3N: Adaptive Clustering-Based Detection of Selective Forwarding Attacks in WSNs under Variable Harsh Environments"
    author: "Haozhen Wang, <u><b>Xinyu Huang</b></u>, Yuanming Wu"
    booktitle: "Information Sciences, 2024"
    url: ""
    link: "https://www.sciencedirect.com/science/article/pii/S0020025524002883"
    pdf: ""
    bibtex: ""
    abs: ""

  - tag: "Journal"
    type: "Journal"
    year: "2023"
    title: "LSTM-NV: A Combined Scheme against Selective Forwarding Attack in Event-Driven Wireless Sensor Networks under Harsh Environments"
    author: "<u><b>Xinyu Huang</b></u>, Shunan Li, Yuanming Wu"
    booktitle: "Engineering Applications of Artificial Intelligence, 2023"
    url: ""
    link: "https://www.sciencedirect.com/science/article/pii/S0952197623006255"
    pdf: ""
    bibtex: ""
    abs: ""

  - tag: "Journal"
    type: "Journal"
    year: "2022"
    title: "Identify Selective Forwarding Attacks Using Danger Model: Promote the Detection Accuracy in Wireless Sensor Networks"
    author: "<u><b>Xinyu Huang</b></u>, Yuanming Wu"
    booktitle: "IEEE Sensors Journal, 2022"
    url: ""
    link: "https://ieeexplore.ieee.org/abstract/document/9755128"
    pdf: ""
    bibtex: ""
    abs: ""
---

<style>
.pub-card{
  display:grid;
  grid-template-columns: 110px 1fr 70px;
  gap:18px;
  padding:20px;
  margin:18px 0;
  border:1px solid #e5e7eb;
  border-radius:12px;
  background:#ffffff;
  box-shadow:0 2px 6px rgba(0,0,0,0.04);
}
.pub-left{display:flex;align-items:flex-start}
.pub-pill{
  background:#f3f4f6;
  border:1px solid #d1d5db;
  color:#374151;
  border-radius:999px;
  padding:6px 12px;
  font-size:12px;
  font-weight:600;
}
.pub-title{margin:0 0 6px;font-size:18px;font-weight:700;color:#111827}
.pub-authors{margin:4px 0;color:#374151}
.pub-venue{margin:6px 0 12px;color:#6b7280;font-size:14px;font-style:italic}
.pub-btns{display:flex;gap:8px;margin:6px 0 0;flex-wrap:wrap}
.pub-btn{
  border:1px solid #d1d5db;
  background:#f9fafb;
  color:#374151;
  padding:6px 12px;
  border-radius:6px;
  font-size:12px;
  font-weight:600;
  text-decoration:none;
}
.pub-btn:hover{background:#f3f4f6}
.pub-abs{border:1px dashed #d1d5db;border-radius:10px;padding:10px;margin-top:12px;background:#fafafa;color:#374151;font-size:14px}
.pub-year{grid-column:3;grid-row:1;color:#9ca3af;font-weight:700;font-size:20px;justify-self:end}
@media (max-width:800px){
  .pub-card{grid-template-columns:90px 1fr}
  .pub-year{display:none}
}
.section-title{margin-top:28px}
</style>

{% assign confs = page.pubs | where: "type", "Conference" | sort: "year" | reverse %}
{% assign journals = page.pubs | where: "type", "Journal" | sort: "year" | reverse %}

# Conference Papers

{% for pub in confs %}
<article class="pub-card">
  <div class="pub-left"><span class="pub-pill">{{ pub.tag }}</span></div>
  <div>
    <h2 class="pub-title">{% if pub.url %}<a href="{{ pub.url }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}</h2>
    <div class="pub-authors">{{ pub.author }}</div>
    <div class="pub-venue">
      {{ pub.booktitle }}
      {% if pub.acceptance_rate %}(Acceptance rate={{ pub.acceptance_rate }}){% endif %}
      {% if pub.type == "Technical Report" and pub.number %} {{ pub.number }}{% endif %}
      {% if pub.school %} {{ pub.school }}{% endif %}
      {% if pub.journal %} {{ pub.journal }}{% endif %}
    </div>
    <div class="pub-btns">
      {% if pub.link %}<a class="pub-btn" href="{{ pub.link }}">LINK</a>{% endif %}
      {% if pub.pdf and pub.pdf != "" %}<a class="pub-btn" href="{{ pub.pdf }}">PDF</a>{% endif %}
      {% if pub.slides and pub.slides != "" %}<a class="pub-btn" href="{{ pub.slides }}">Slides</a>{% endif %}
      {% if pub.bibtex and pub.bibtex != "" %}<a class="pub-btn" href="{{ pub.bibtex }}">BibTeX</a>{% endif %}
    </div>
    {% if pub.abs and pub.abs != "" %}<div class="pub-abs">{{ pub.abs }}</div>{% endif %}
  </div>
  <div class="pub-year">{{ pub.year }}</div>
</article>
{% endfor %}

# Journal Papers

{% for pub in journals %}
<article class="pub-card">
  <div class="pub-left"><span class="pub-pill">{{ pub.tag }}</span></div>
  <div>
    <h2 class="pub-title">{% if pub.url %}<a href="{{ pub.url }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}</h2>
    <div class="pub-authors">{{ pub.author }}</div>
    <div class="pub-venue">
      {{ pub.booktitle }}
      {% if pub.journal %} {{ pub.journal }}{% endif %}
    </div>
    <div class="pub-btns">
      {% if pub.link %}<a class="pub-btn" href="{{ pub.link }}">LINK</a>{% endif %}
      {% if pub.pdf and pub.pdf != "" %}<a class="pub-btn" href="{{ pub.pdf }}">PDF</a>{% endif %}
      {% if pub.slides and pub.slides != "" %}<a class="pub-btn" href="{{ pub.slides }}">Slides</a>{% endif %}
      {% if pub.bibtex and pub.bibtex != "" %}<a class="pub-btn" href="{{ pub.bibtex }}">BibTeX</a>{% endif %}
    </div>
    {% if pub.abs and pub.abs != "" %}<div class="pub-abs">{{ pub.abs }}</div>{% endif %}
  </div>
  <div class="pub-year">{{ pub.year }}</div>
</article>
{% endfor %}
