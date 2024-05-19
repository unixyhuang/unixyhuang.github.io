---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 2
pubs:

### Topic: IoT Network Security

  - author: "Haozhen Wang, **Xinyu Huang**, Yuanming Wu"
    title: "GD3N: Adaptive Clustering-Based Detection of Selective Forwarding Attacks in WSNs under Variable Harsh Environments"
    month: "Feburary"
    year: "2024"
    booktitle: "Information Sciences (INS)"
    url: "https://www.sciencedirect.com/science/article/pii/S0020025524002883"

  - author: "**Xinyu Huang**, Shunan Li, Yuanming Wu"
    title: "LSTM-NV: A Combined Scheme against Selective Forwarding Attack in Event-Driven Wireless Sensor Networks under Harsh Environments"
    month: "May"
    year: "2023"
    booktitle: "Engineering Applications of Artificial Intelligence (EAAI)"
    url: "https://www.sciencedirect.com/science/article/pii/S0952197623006255"
    
  - author: "**Xinyu Huang**, Yuanming Wu"
    title: "Identify Selective Forwarding Attacks Using Danger Model: Promote the Detection Accuracy in Wireless Sensor Networks"
    month: "May"
    year: "2022"
    booktitle: "IEEE Sensors Journal"
    url: "https://ieeexplore.ieee.org/abstract/document/9755128"


---

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}<br>
    {% if pub.address %}{{pub.address}}
    {% endif %} {{pub.month}}, {{pub.year}} {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}

