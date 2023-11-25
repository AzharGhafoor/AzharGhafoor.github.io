---
title: "Experience"
layout: gridlay
sitemap: false
permalink: /experience/
---

# Experiences

## Cyber Security Analyst
[Cytomate Solutions & Services](https://cytomate.net/)    `Qatar`    `2022-2023`
<div class="rowl1" style="padding-top: 10px;">
```
- Spearheaded the development of the first-ever cutting-edge compliance tool, leveraging the NIA Policy Standard 2.1 Qatar. The tool measures compliance for SMEs nationwide, resulting in an impressive 80% increase in compliance rates for clients.

- Led a team of four cybersecurity professionals in creating a post-attack assessment system using machine learning models. This system proved to be 40% more effective than competing solutions in the market, detecting undetected attacks.

- Played a key role in an attack surface management project, aimed at timely detection, prevention, and containment of critical assets and information. The project is slated for implementation across multiple clients.

- Led a phishing awareness project, devising various exploits to simulate email theft and account hijacking. Developed a machine learning-based tool that reduced password harvesting attacks by over 80% compared to previous statistics.

- Led the development and deployment of advanced cyber deception systems, resulting in a remarkable 70% decrease in successful attacks on client networks.

- Conducted in-depth log analysis using advanced machine learning models to uncover hidden malicious patterns and identify threats in their early stages. This initiative strengthened the overall security posture and reduced detection time for attacks by 70%.

- Deployed network protection technologies, including IDS/IPS and firewalls, and seamlessly integrated them with various SIEM solutions such as QRadar, Wazuh, and Splunk.

- Collaborated effectively with cross-functional teams on multiple cybersecurity projects, demonstrating excellent communication and teamwork skills.

```
</div>


{% if site.data.thesis_azhar %}
<!-- Sort courses by year -->
{% assign students = site.data.thesis_azhar | sort: 'year' | reverse %}
## Cyber Security Lab
<div class="rowl1" style="padding-top: 10px;">

{% for student in students %}
  {% assign pdffile = false %}
  {% if student.project_url %}
      {% if student.project_url contains '://' %}
        {% assign pdffile = student.project_url %}
      {% else %}
        {% assign pdffile = "/publications/students/" | append:  student.project_url  | append: ".pdf" %}
      {% endif %}
  {% endif %}

{{ forloop.index }}. {% if student.name_url %}<a href="{{ student.name_url }}" target="_blank">{% endif %} <strong>{{ student.name }}</strong> {% if student.name_url %}</a>{% endif %} ({{ student.year }}) {% if student.status == 'notstarted' %}<button class="btn-notstarted">NOT STARTED</button>{% endif %}{% if student.status == 'inprogress' %}<button class="btn-inprogress">IN PROGRESS</button>{% endif %}{% if student.status == 'completed' %}<button class="btn-completed">COMPLETED</button>{% endif %}{% if student.comment %} – {{ student.comment }}{% endif %}
<br/>
<i>{{ student.project }}</i>{% if pdffile %} (<a href="{{ pdffile }}" target="_blank">link</a>){% endif %}.

{% endfor %}
</div>
{% endif %}



{% if site.data.manuals %}
<!-- Sort courses by year -->
{% assign students = site.data.manuals | sort: 'year' | reverse %}
## Intern
<div class="rowl1" style="padding-top: 10px;">

{% for student in students %}
  {% assign pdffile = false %}
  {% if student.project_url %}
      {% if student.project_url contains '://' %}
        {% assign pdffile = student.project_url %}
      {% else %}
        {% assign pdffile = "/publications/students/" | append:  student.project_url  | append: ".pdf" %}
      {% endif %}
  {% endif %}

{{ forloop.index }}. {% if student.name_url %}<a href="{{ student.name_url }}" target="_blank">{% endif %} <strong>{{ student.name }}</strong> {% if student.name_url %}</a>{% endif %} ({{ student.year }}) {% if student.status == 'notstarted' %}<button class="btn-notstarted">NOT STARTED</button>{% endif %}{% if student.status == 'available' %}<button class="btn-inprogress">AVAILABLE</button>{% endif %}{% if student.status == 'published' %}<button class="btn-completed">PUBLISHED</button>{% endif %}{% if student.comment %} – {{ student.comment }}{% endif %}
<br/>
<i>{{ student.project }}</i>{% if pdffile %} (<a href="{{ pdffile }}" target="_blank">link</a>){% endif %}.

{% endfor %}
</div>
{% endif %}
