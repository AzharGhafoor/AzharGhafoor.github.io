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

  {% if member.number_educ == 7 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
  <li> {{ member.education7 }} </li>
  {% endif %}
  </ul>
</div>

{% endfor %}

## Short biography

<div class="short-bio">
<p align="justify">
Azhar Ghafoor is a seasoned Cybersecurity Expert with a deep-rooted passion for advancing the field. With over five years of hands-on experience, he has led and contributed to diverse projects spanning compliance management, post-attack forensics, attack surface reduction, and security operations. His expertise also encompasses machine learning-based log anomaly detection, cyber deception strategies, phishing detection and awareness training, and intrusion detection systems like Snort and Suricata. 

Azhar actively shares his insights as a Cybersecurity Content Writer on Medium and delivers professional services as a top-rated Freelancer on Fiverr. He holds a Master’s degree in Information Security from COMSATS University Islamabad, a testament to his dedication to cybersecurity excellence and continuous learning.
</p>
</div>



## Skills 

| Technical Skills | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Soft Skills |
|---------------------------------------------------|---------------------------------------------------------|
| <button class="btn-completed">Expert in creating deceptive systems</button> |&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<button class="btn-inprogress">Analyzing complex data to spot patterns</button> |
| <button class="btn-completed">Analyzing and interpreting logs</button> |&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<button class="btn-inprogress">Communicating technical concepts clearly & effectively </button> |
| <button class="btn-completed">Customization & Creation of python tools </button> |&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<button class="btn-inprogress">Adapting swiftly to evolving cybersecurity landscapes</button> |
| <button class="btn-completed">Utilizing and creating machine learning models</button> |&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<button class="btn-inprogress">Paying meticulous attention to detail</button> |
| <button class="btn-completed">Employee Training Campaigns</button> |&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<button class="btn-inprogress">Ethical Judgement in handling sensitive information</button> |
| <button class="btn-completed">Knowledgeable in auditing firms for compliance</button> |&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<button class="btn-inprogress"> Passion for staying up to date with latest technologies</button>


## Hands-On Tools
<div class="rowl1" style="padding-top: 10px; text-align:justify;">
`ISO-27001` `NIA Policy 2.0` `NIA Standard 2.1` `NIST Standards` `PCI-DSS` `HIPPA` `Personal Data Protection Law - Qatar` `Emekie` `Splunk SIEM` `QRadar SIEM` `Wazuh EDR` `Snort IDS/IPS` `Suricata IDS` `NMAP` `Cuckoo Sandbox` `Python` `Machine Learning` `Anomaly Detection` `Pandas - Data Analytics` `Linux (Kali, Ubuntu)` `Google Dorking` `Generative Ai` `Proxmox` `Ollama` `RAG` `theHarvester` `Amass` `Mimikatz` `Metasploit` `httpX` `Metasploitable` `Recon-ng` `Censys` `Shodan` `Gophish` `W3af` `Nuclei` `Wapiti` `Dalfox` `Wappalyze` `Burpsuite` `OWASP Zap` `Sublist3r` `Subfinder` `VMware` `Virtual Box` `Whois` `Wireshark` `Hybrid Analysis` `Process Hacker` `Process Monitor` `IDA-Pro` `OWASP ZAP` `VirusTotal` `Joe Security Joe Sandbox` `PeStudio` `Open EDR` `Shodan` `IntelliganceX` `OSINT Framework` `TinyEye` `Yandex` `Maltego` `BuiltWith` `Wayback Machines` `Metagoofil` `Anaconda Distribution` `Ettercap` `Ffuf` `Dirbuster` `Wfuzz` `Hydra` `Medusa` `Hashcat` `XSStrike` `PwnXSS` `Sqlmap` `Ghouri` `Dionaea` `Cowrie` `Snare&Tanner` `Conpot` `Office 365` `Proxmox` `Teams` `Trello` `MS Azure` `Google Cloud Platform` `WireGuard` `Mx Toolbox` `Github` `Latex` `WAF Testing` `Cloud Enum` `Autopsy` `Matplotlib` `Flask` `Requests` `Beautiful Soup` `Scrapy` `Seaborn` `Scikit-learn` `NLTK` `Auto Encoder` `Joblib` `Transformers` `Volatility` `EnCase` `Autopsy` `Cellebrite` `NetworkMiner` `FTK Forensic Toolkit` `FTK Imager` `Bulk Extractor` `Redline` `MailXaminer` `DomainTools`
</div>

## Interests
<div class="rowl1" style="padding-top: 10px;">
1. GRC and Compliance
2. Cybersecurity Community Engagement
3. Cybersecurity Training and Education
4. Cybersecurity Research and Practical
5. Learning New Languages & Cultures 
6. Gym and Fitness
</div>


## Languages
<div class="rowl1" style="padding-top: 10px;">
1. Urdu
2. English
</div>



{% if site.data.collaborators %}
## Collaborations
<div class="rowl1" style="padding-top: 10px;">

{% for collaborator in site.data.collaborators %}
{{ forloop.index }}. {% if collaborator.name_url %}<a href="{{ collaborator.name_url }}" target="_blank">{% endif %}<strong>{{ collaborator.name }}</strong>{% if collaborator.name_url %}</a>{% endif %} ({{ collaborator.field }}, {% if collaborator.institution_url %}<a href="{{ collaborator.institution_url }}" target="_blank">{% endif %}{{ collaborator.institution }}{% if collaborator.institution_url %}</a>{% endif %}).
{% endfor %}
</div>
{% endif %}


## Contact Me
<div style="border: 1px solid #ddd; padding: 10px; border-radius: 8px; display: inline-block; margin: auto; width: 100%;">
<p align="center">
<a href="https://twitter.com/_azhar_ghafoor" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="_azhar_ghafoor" height="30" width="40" /></a>
<a href="https://linkedin.com/in/azhar-ghafoor" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="azhar-ghafoor" height="30" width="40" /></a>
<a href="https://medium.com/@ghafoorazhar" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/medium.svg" alt="@ghafoorazhar" height="30" width="40" /></a>
<a href="https://github.com/AzharGhafoor" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/github.svg" alt="@AzharGhafoor" height="30" width="40" /></a>
<a href="https://scholar.google.com/citations?user=UYIGXywAAAAJ" target="blank"><img align="center" src="https://upload.wikimedia.org/wikipedia/commons/c/c7/Google_Scholar_logo.svg" alt="@AzharGhafoor" height="30" width="40" /></a> 
<a href="https://www.researchgate.net/profile/Azhar-Ghafoor-3" target="blank"><img align="center" src="https://upload.wikimedia.org/wikipedia/commons/5/5e/ResearchGate_icon_SVG.svg" alt="@Azhar-Ghafoor-3" height="30" width="40" /></a> 
<a href="https://www.fiverr.com/azharghafoor39" target="blank"><img align="center" src="https://cdn3.iconfinder.com/data/icons/logos-and-brands-adobe/512/129_Fiverr-512.png" alt="@Aazharghafoor39" height="30" width="40" /></a> 
</p>
</div>
