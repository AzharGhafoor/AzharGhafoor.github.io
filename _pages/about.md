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
| <button class="btn-completed">Expert in creating deceptive systems</button> | <button class="btn-inprogress">Analyzing complex data to spot patterns</button> |
| <button class="btn-completed">Analyzing and interpreting logs</button> | <button class="btn-inprogress">Communicating technical concepts clearly & effectively </button> |
| <button class="btn-completed">Customization & Creation of python tools </button> | <button class="btn-inprogress">Adapting swiftly to evolving cybersecurity landscapes</button> |
| <button class="btn-completed">Skilled in utilizing and creating machine learning models</button> | <button class="btn-inprogress">Paying meticulous attention to detail</button> |
| <button class="btn-completed">Employee Training Campaigns</button> | <button class="btn-inprogress">Ethical Judgement in handling sensitive information</button> |
| <button class="btn-completed">Knowledgeable in auditing firms for compliance</button> | <button class="btn-inprogress"> Passion for staying up to date with latest technologies</button>


## Hands-On Tools
<div class="rowl1" style="padding-top: 10px; text-align:justify;">
`ISO-27001` `NIA Policy 2.0` `NIA Standard 2.1` `NIST Standards` `PCI-DSS` `HIPPA` `Personal Data Protection Law - Qatar` `Emekie` `Splunk SIEM` `QRadar SIEM` `Wazuh EDR` `Snort IDS/IPS` `Suricata IDS` `Nmap` `Cuckoo Sandbox` `Python` `Clustering - Machine Learning` `Anomaly Detection` `Classification - Machine Learning` `Pandas - Data Analytics` `Linux (Kali, Ubuntu)` `Google Dorking` `theHarvester` `Amass` `Mimikatz` `Metasploit` `httpX` `Metasploitable` `Recon-ng` `Censys` `Shodan` `Gophish` `W3af` `Nuclei` `Wapiti` `Dalfox` `Wappalyze` `Burpsuite` `OWASP Zap` `Sublist3r` `Subfinder` `VMware` `Virtual Box` `Whois` `Wireshark` `Anaconda Distribution` `Ettercap` `Ffuf` `Dirbuster` `Wfuzz` `Hydra` `Medusa` `Hashcat` `XSStrike` `PwnXSS` `Sqlmap` `Ghouri` `Dionaea` `Cowrie` `Snare&Tanner` `Conpot` `Office 365` `Proxmox` `Teams` `Trello` `MS Azure` `Google Cloud Platform` `WireGuard` `Mx Toolbox` `Github` `Latex` `WAF Testing` `Cloud Enum` `Autopsy` `Matplotlib` `Flask` `Requests` `Beautiful Soup` `Scrapy` `Seaborn` `Scikit-learn` `NLTK` `Auto Encoder` `Joblib` `Transformers` 
</div>


## Interests
<div class="rowl1" style="padding-top: 10px;">
```
1. GRC and Compliance
2. Cybersecurity Community Engagement
3. Cybersecurity Training and Education
4. Cybersecurity Research and Practical
5. Learning New Languages & Cultures 
6. Gym and Fitness
```
</div>




{% if site.data.collaborators %}
## Collaborations
<div class="rowl1" style="padding-top: 10px;">

{% for collaborator in site.data.collaborators %}
{{ forloop.index }}. {% if collaborator.name_url %}<a href="{{ collaborator.name_url }}" target="_blank">{% endif %}<strong>{{ collaborator.name }}</strong>{% if collaborator.name_url %}</a>{% endif %} ({{ collaborator.field }}, {% if collaborator.institution_url %}<a href="{{ collaborator.institution_url }}" target="_blank">{% endif %}{{ collaborator.institution }}{% if collaborator.institution_url %}</a>{% endif %}).
{% endfor %}
</div>
{% endif %}


