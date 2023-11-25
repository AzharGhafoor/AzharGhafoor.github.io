---
title: "About"
layout: gridlay
sitemap: false
permalink: /about/
---

## About 


{% for member in site.data.pi %}

<div class="row">
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo-large }}" class="img-responsive avatar-about" />
  <h3>{{ member.name }}</h3>
  <i style="font-size:20px">{{ member.info }}</i><br>

  {% if member.website %}<a href="{{ member.website }}" target="_blank"><i class="fa fa-home fa-3x"></i></a> {% endif %}
  {% if member.email %}<a href="mailto:{{ member.email }}" target="_blank"><i class="fa fa-envelope-square fa-3x"></i></a> {% endif %}
  {% if member.cv %} <a href="{{ member.cv }}" target="_blank"><i class="ai ai-cv-square ai-3x"></i></a> {% endif %}
  {% if member.orcid %} <a href="{{ member.orcid }}" target="_blank"><i class="ai ai-orcid-square ai-3x"></i></a> {% endif %}
  {% if member.linkedin %} <a href="{{ member.linkedin }}" target="_blank"><i class="fa fa-linkedin-square fa-3x"></i></a> {% endif %}
  {% if member.scholar %} <a href="{{ member.scholar }}" target="_blank"><i class="ai ai-google-scholar-square ai-3x"></i></a> {% endif %}
  {% if member.researchgate %} <a href="{{ member.researchgate }}" target="_blank"><i class="ai ai-researchgate-square ai-3x"></i></a> {% endif %}
  {% if member.github %} <a href="{{ member.github }}" target="_blank"><i class="fa fa-github-square fa-3x"></i></a> {% endif %}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  {% if member.number_educ == 6 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
  {% endif %}

  </ul>
</div>

{% endfor %}

## Short biography

<div class="short-bio">
 <p align="justify">Azhar Ghafoor is a seasoned Cybersecurity Analyst with a profound passion for the field. With over a year of experience at Cytomate, he has spearheaded innovative projects in compliance, post-attack assessment, and attack surface management. Azhar's expertise extends to machine learning-driven log analysis, advanced cyber deception, and impactful phishing awareness campaigns. As a Cybersecurity Content Writer on Medium and a Professional Freelancer on Fiverr, he shares his knowledge and delivers top-tier results. Azhar holds a Master's in Information Security from COMSATS University Islamabad, cementing his commitment to cybersecurity excellence.</p>
</div>



## Skills 

| Technical Skills | Soft Skills |
|---------------------------------------------------|---------------------------------------------------------|
| <button class="btn-completed">Cyber Deception</button> - Expert in creating deceptive systems to mislead attackers. | <button class="btn-completed">Analytical Thinking</button> - I analyze complex data to spot patterns and identify security vulnerabilities. |
| <button class="btn-completed">Logs Analysis</button> Extensive experience in analyzing and interpreting logs for security insights. | <button class="btn-completed">Communication Skills</button> I communicate technical concepts clearly for effective collaboration in cybersecurity. |
| <button class="btn-completed">Python Tools Customization</button> Proficient in customizing tools using Python for enhanced cybersecurity functionality. | <button class="btn-completed">Adaptability</button> I adapt swiftly to evolving cybersecurity landscapes, addressing emerging threats proactively. |
| <button class="btn-completed">Machine Learning Models</button> Skilled in both utilizing and creating machine learning models for cybersecurity. | <button class="btn-completed">Attention to Detail</button> I pay meticulous attention to detail, ensuring thorough security system examinations and precise documentation. |
| <button class="btn-completed">Employee Training Campaigns</button> Develops and executes phishing awareness campaigns for employee training. | <button class="btn-completed">Ethical Judgement</button> I maintain high ethical standards, handling sensitive information responsibly in compliance with privacy and legal requirements. |
| <button class="btn-completed">Compliance Auditing Knowledge</button> Knowledgeable in auditing firms for compliance with various standards and frameworks. | <button class="btn-completed"> Long Life Learning</button> I maintain high ethical standards, handling sensitive information responsibly in compliance with privacy and legal requirements.





| Technical Skills | Soft Skills |
|---------------------------------------------------|---------------------------------------------------------|
| <button class="btn-completed">Cyber Deception</button> 
- Expert in creating deceptive systems to mislead attackers. | <button class="btn-completed">Analytical Thinking</button>
- I analyze complex data to spot patterns and identify security vulnerabilities. |
| <button class="btn-completed">
- Logs Analysis</button> Extensive experience in analyzing and interpreting logs for security insights. | <button class="btn-completed">
- Communication Skills</button> I communicate technical concepts clearly for effective collaboration in cybersecurity. |








{% if site.data.collaborators %}
## Collaborations
<div class="rowl1" style="padding-top: 10px;">

{% for collaborator in site.data.collaborators %}
{{ forloop.index }}. {% if collaborator.name_url %}<a href="{{ collaborator.name_url }}" target="_blank">{% endif %}<strong>{{ collaborator.name }}</strong>{% if collaborator.name_url %}</a>{% endif %} ({{ collaborator.field }}, {% if collaborator.institution_url %}<a href="{{ collaborator.institution_url }}" target="_blank">{% endif %}{{ collaborator.institution }}{% if collaborator.institution_url %}</a>{% endif %}).
{% endfor %}
</div>
{% endif %}


