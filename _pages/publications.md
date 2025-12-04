---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 3

pubs:
  - tag: "SenSys'25"
    type: "Conference"
    year: "2025"
    title: "GPIoT: Tailoring Small Language Models for IoT Program Synthesis and Development"
    author: "Leming Shen, Qiang Yang, <u><b>Xinyu Huang</b></u>, Zijing Ma, Yuanqing Zheng"
    booktitle: "SenSys 2025, May 6–9, 2025, Irvine, USA"
    acceptance_rate: "19.6%"
    link: "https://dl.acm.org/doi/10.1145/3715014.3722064"
    pdf: "https://unixyhuang.github.io/pubs/GPIoT.pdf"
    slides: ""
    bibtex: ""
    abs: ""

  - tag: "CCS'25"
    type: "Conference"
    year: "2025"
    title: "LLMalware: An LLM-Powered Robust and Efficient Android Malware Detection Framework"
    author: "Zijing Ma, Leming Shen, <u><b>Xinyu Huang</b></u>, Yuanqing Zheng"
    booktitle: "CCS 2025 (Poster), October 13–17, 2025, Taipei, Taiwan"
    link: ""
    slides: ""
    bibtex: ""
    abs: ""
    
  - tag: "MobiCom'25"
    type: "Conference"
    year: "2025"
    title: "Towards Privacy-Preserving and Personalized Smart Homes via Tailored Small Language Models"
    author: "<u><b>Xinyu Huang</b></u>, Leming Shen, Zijing Ma, Yuanqing Zheng"
    booktitle: "MobiCom 2025 (Poster), November 4–8, 2025, Hong Kong, China"
    link: "https://dl.acm.org/doi/10.1145/3680207.3765677"
    slides: ""
    bibtex: ""
    abs: ""

  - tag: "arXiv"
    type: "Journal"
    year: "2025"
    title: "Towards Privacy-Preserving and Personalized Smart Homes via Tailored Small Language Models"
    author: "<u><b>Xinyu Huang</b></u>, Leming Shen, Zijing Ma, Yuanqing Zheng"
    booktitle: "arXiv Preprint"
    link: "https://arxiv.org/abs/2507.08878"
    slides: ""
    bibtex: ""
    abs: ""
    
  - tag: "INS"
    type: "Others"
    year: "2024"
    title: "GD3N: Adaptive Clustering-Based Detection of Selective Forwarding Attacks in WSNs under Variable Harsh Environments"
    author: "Haozhen Wang, <u><b>Xinyu Huang</b></u>, Yuanming Wu"
    booktitle: "Information Sciences, 2024"
    link: "https://www.sciencedirect.com/science/article/pii/S0020025524002883"
    pdf: ""
    bibtex: ""
    abs: ""

  - tag: "EAAI"
    type: "Others"
    year: "2023"
    title: "LSTM-NV: A Combined Scheme against Selective Forwarding Attack in Event-Driven Wireless Sensor Networks under Harsh Environments"
    author: "<u><b>Xinyu Huang</b></u>, Shunan Li, Yuanming Wu"
    booktitle: "Engineering Applications of Artificial Intelligence, 2023"
    link: "https://www.sciencedirect.com/science/article/pii/S0952197623006255"
    pdf: ""
    bibtex: ""
    abs: ""

  - tag: "IEEE SensJ"
    type: "Others"
    year: "2022"
    title: "Identify Selective Forwarding Attacks Using Danger Model: Promote the Detection Accuracy in Wireless Sensor Networks"
    author: "<u><b>Xinyu Huang</b></u>, Yuanming Wu"
    booktitle: "IEEE Sensors Journal, 2022"
    link: "https://ieeexplore.ieee.org/abstract/document/9755128"
    pdf: ""
    bibtex: ""
    abs: ""
---

<style>
:root{
  --pub-bg: #ffffff;
  --pub-border: #d1d5db;
  --pub-shadow: rgba(0,0,0,0.03);

  --pub-title: #111111;
  --pub-text: #333333;
  --pub-venue: #555555;
  --pub-year: #777777;

  --pub-pill-bg: #f5f5f5;
  --pub-pill-border: #d1d5db;
  --pub-pill-text: #333333;

  --pub-btn-bg: #ffffff;
  --pub-btn-hover: #f0f0f0;
  --pub-btn-border: #d1d5db;
  --pub-btn-text: #111111;

  --pub-abs-bg: #fafafa;
  --pub-abs-border: #d1d5db;
  --pub-abs-text: #333333;
}

html[data-theme="dark"]{
  --pub-bg: #0f172a;
  --pub-border: #1e293b;
  --pub-shadow: rgba(0,0,0,0.5);

  --pub-title: #e5e7eb;
  --pub-text: #cbd5e1;
  --pub-venue: #94a3b8;
  --pub-year: #64748b;

  --pub-pill-bg: #020617;
  --pub-pill-border: #1e293b;
  --pub-pill-text: #e5e7eb;

  --pub-btn-bg: #020617;
  --pub-btn-hover: #1e293b;
  --pub-btn-border: #1e293b;
  --pub-btn-text: #e5e7eb;

  --pub-abs-bg: #020617;
  --pub-abs-border: #1e293b;
  --pub-abs-text: #cbd5e1;
}

.pub-card{
  display:grid;
  grid-template-columns:110px 1fr 70px;
  gap:18px;
  padding:20px;
  margin:18px 0;
  border:1px solid var(--pub-border);
  border-radius:10px;
  background:var(--pub-bg);
  box-shadow:0 1px 4px var(--pub-shadow);
}

.pub-left{
  display:flex;
  align-items:flex-start
}

.pub-pill{
  background:var(--pub-pill-bg);
  border:1px solid var(--pub-pill-border);
  color:var(--pub-pill-text);
  border-radius:999px;
  padding:5px 11px;
  font-size:12px;
  font-weight:600;
}

.pub-title{
  margin:0 0 6px;
  font-size:17px;
  font-weight:700;
  color:var(--pub-title);
  line-height:1.35;
}

.pub-title a{
  color:inherit;
  text-decoration:none;
}

.pub-title a:hover{
  text-decoration:underline;
}

.pub-authors{
  margin:4px 0;
  color:var(--pub-text);
  font-size:14.5px;
}

.pub-venue{
  margin:6px 0 12px;
  color:var(--pub-venue);
  font-size:14px;
  font-style:italic;
}

.pub-btns{
  display:flex;
  gap:8px;
  margin:6px 0 0;
  flex-wrap:wrap;
}

.pub-btn{
  border:1px solid var(--pub-btn-border);
  background:var(--pub-btn-bg);
  color:var(--pub-btn-text);
  padding:5px 12px;
  border-radius:4px;
  font-size:12px;
  font-weight:600;
  text-decoration:none;
}

.pub-btn:hover{
  background:var(--pub-btn-hover);
}

.pub-abs{
  border:1px dashed var(--pub-abs-border);
  border-radius:8px;
  padding:10px;
  margin-top:12px;
  background:var(--pub-abs-bg);
  color:var(--pub-abs-text);
  font-size:14px;
  line-height:1.6;
}

.pub-year{
  grid-column:3;
  grid-row:1;
  color:var(--pub-year);
  font-weight:700;
  font-size:18px;
  justify-self:end;
}

@media (max-width:800px){
  .pub-card{grid-template-columns:90px 1fr}
  .pub-year{display:none}
}

.section-title{
  margin-top:28px
}
</style>



{% assign confs = page.pubs | where: "type", "Conference" | sort: "year" | reverse %}
{% assign journals = page.pubs | where: "type", "Journal" | sort: "year" | reverse %}
{% assign others = page.pubs | where: "type", "Others" | sort: "year" | reverse %}

## Conference

{% for pub in confs %}
{% assign href = pub.url | default: pub.link %}
<article class="pub-card">
  <div class="pub-left"><span class="pub-pill">{{ pub.tag }}</span></div>
  <div>
    <h2 class="pub-title">{% if href %}<a href="{{ href }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}</h2>
    <div class="pub-authors">{{ pub.author }}</div>
    <div class="pub-venue">
      {{ pub.booktitle }}
      {% if pub.acceptance_rate %}(Acceptance rate={{ pub.acceptance_rate }}){% endif %}
      {% if pub.type == "Technical Report" and pub.number %} {{ pub.number }}{% endif %}
      {% if pub.school %} {{ pub.school }}{% endif %}
      {% if pub.journal %} {{ pub.journal }}{% endif %}
    </div>
    <div class="pub-btns">
      {% if pub.link and pub.link != "" %}<a class="pub-btn" href="{{ pub.link }}">LINK</a>{% endif %}
      {% if pub.pdf and pub.pdf != "" %}<a class="pub-btn" href="{{ pub.pdf }}">PDF</a>{% endif %}
      {% if pub.slides and pub.slides != "" %}<a class="pub-btn" href="{{ pub.slides }}">Slides</a>{% endif %}
      {% if pub.bibtex and pub.bibtex != "" %}<a class="pub-btn" href="{{ pub.bibtex }}">BibTeX</a>{% endif %}
    </div>
    {% if pub.abs and pub.abs != "" %}<div class="pub-abs">{{ pub.abs }}</div>{% endif %}
  </div>
  <div class="pub-year">{{ pub.year }}</div>
</article>
{% endfor %}

## Journal

{% for pub in journals %}
{% assign href = pub.url | default: pub.link %}
<article class="pub-card">
  <div class="pub-left"><span class="pub-pill">{{ pub.tag }}</span></div>
  <div>
    <h2 class="pub-title">{% if href %}<a href="{{ href }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}</h2>
    <div class="pub-authors">{{ pub.author }}</div>
    <div class="pub-venue">
      {{ pub.booktitle }}
      {% if pub.journal %} {{ pub.journal }}{% endif %}
    </div>
    <div class="pub-btns">
      {% if pub.link and pub.link != "" %}<a class="pub-btn" href="{{ pub.link }}">LINK</a>{% endif %}
      {% if pub.pdf and pub.pdf != "" %}<a class="pub-btn" href="{{ pub.pdf }}">PDF</a>{% endif %}
      {% if pub.slides and pub.slides != "" %}<a class="pub-btn" href="{{ pub.slides }}">Slides</a>{% endif %}
      {% if pub.bibtex and pub.bibtex != "" %}<a class="pub-btn" href="{{ pub.bibtex }}">BibTeX</a>{% endif %}
    </div>
    {% if pub.abs and pub.abs != "" %}<div class="pub-abs">{{ pub.abs }}</div>{% endif %}
  </div>
  <div class="pub-year">{{ pub.year }}</div>
</article>
{% endfor %}

## Others

{% for pub in others %}
{% assign href = pub.url | default: pub.link %}
<article class="pub-card">
  <div class="pub-left"><span class="pub-pill">{{ pub.tag }}</span></div>
  <div>
    <h2 class="pub-title">{% if href %}<a href="{{ href }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}</h2>
    <div class="pub-authors">{{ pub.author }}</div>
    <div class="pub-venue">
      {{ pub.booktitle }}
      {% if pub.type == "Technical Report" and pub.number %} {{ pub.number }}{% endif %}
      {% if pub.school %} {{ pub.school }}{% endif %}
      {% if pub.journal %} {{ pub.journal }}{% endif %}
    </div>
    <div class="pub-btns">
      {% if pub.link and pub.link != "" %}<a class="pub-btn" href="{{ pub.link }}">LINK</a>{% endif %}
      {% if pub.pdf and pub.pdf != "" %}<a class="pub-btn" href="{{ pub.pdf }}">PDF</a>{% endif %}
      {% if pub.slides and pub.slides != "" %}<a class="pub-btn" href="{{ pub.slides }}">Slides</a>{% endif %}
      {% if pub.bibtex and pub.bibtex != "" %}<a class="pub-btn" href="{{ pub.bibtex }}">BibTeX</a>{% endif %}
    </div>
    {% if pub.abs and pub.abs != "" %}<div class="pub-abs">{{ pub.abs }}</div>{% endif %}
  </div>
  <div class="pub-year">{{ pub.year }}</div>
</article>
{% endfor %}
