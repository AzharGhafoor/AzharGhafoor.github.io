---
title: "Publications"
layout: gridlay
sitemap: false
permalink: /publications/
---

# Publications

{% assign yeartest = true %}
{% for publi in site.publications %}
  {% if publi.year %}{% else %}
   {% assign yeartest = false %}
  {% endif %}
{% endfor %}

{% if yeartest == false %}
## Working documents
{% endif %}

{% for publi in site.publications %}

  {% assign pdfpresent = false %}
  {% if publi.pdf %}
    {% assign pdffile = "/publications/" | append:  publi.pdf  | append: ".pdf" %}
    {% for file in site.static_files %}
      {% if file.path contains pdffile %}
       {% assign pdfpresent = true %}
      {% endif %}
    {% endfor %}
  {% endif %}

  {% if publi.year %}{% else %}

  {% assign bibtest = false %}
  {% if publi.pdf %}
    {% assign bibfile = "/publications/" | append:  publi.pdf  | append: ".txt" %}
    {% for file in site.static_files %}
      {% if file.path contains bibfile %}
       {% assign bibtest = true %}
      {% endif %}
    {% endfor %}
  {% endif %}

  <div class="well-sm publication-entry">
  <ul class="flex-container">
  <li class="flex-item1">
    {% if publi.image %}
     <img src="{{ site.url }}{{ site.baseurl }}/images/publications/{{ publi.image }}" class="img-responsive"/>
    {% endif %}
  </li>
  <li class="flex-item2">
    {% if publi.pdf %}<a href="{{ publi.pdf }}" target="_blank">{% endif %} <strong>{{ publi.title }}</strong> {% if publi.pdf %}</a>{% endif %}<br/>
    {{ publi.authors }}<br/>
    <em>{{ publi.display }}</em><br/>
    {% if publi.abstract %} <a data-bs-toggle="collapse" href="#{{publi.pdf}}"  class="btn-abstract" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false" aria-controls="{{publi.pdf}}">ABSTRACT</a> {% endif %}
    {% if bibtest == true %} <a data-bs-toggle="collapse" href="#{{publi.pdf}}2"  class="btn-bib" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false" aria-controls="{{publi.pdf}}2">BIB</a> {% endif %}
    {% if pdfpresent == true %}<a href="{{ pdffile }}" target="_blank"><button class="btn-pdf">PDF</button></a>{% endif %}
    {% if publi.doi %}<a href="http://doi.org/{{ publi.doi }}" target="_blank"><button class="btn-doi">DOI</button></a> {% endif %}
    {% if publi.arxiv %}<a href="https://arxiv.org/abs/{{ publi.arxiv }}" target="_blank"><button class="btn-arxiv">ARXIV</button></a> {% endif %}
    {% if publi.code %}<a href="{{ publi.code }}" target="_blank"><button class="btn-code">CODE</button></a> {% endif %}
    {% if publi.suppmat %}<a href="{{ publi.suppmat }}" target="_blank"><button class="btn-suppmat">SUPPLEMENT</button></a> {% endif %}

  {% if publi.abstract %}
  <div class="collapse" id="{{publi.pdf}}"><div class="well-abstract">
   {{publi.abstract}}
  </div></div>
  {% endif %}

  {% if bibtest == true %}
  <div class="collapse" id="{{publi.pdf}}2"><div class="well-bib">
   <iframe src='{{site.url}}{{site.baseurl}}/publications/{{publi.pdf}}.txt' scrolling="yes" width="100%" height="210" frameborder="0"></iframe>
  </div></div>
  {% endif %}

  </li>
  </ul>
  </div>
  {% endif %}
{% endfor %}

{% if site.group_pub_by_year == true %}{% else %}
## Journal Papers and Proceedings 
{% endif %}

{% for myyear in site.data.years %}

{% assign yeartest = false %}
{% for publi in site.publications %}
  {% if publi.year == myyear.year %}
   {% assign yeartest = true %}
  {% endif %}
{% endfor %}

{% if site.group_pub_by_year == true %}
{% if yeartest == true %}
## {{ myyear.year }}
{% endif %}
{% endif %}

{% for publi in site.publications %}

{% assign pdfpresent = false %}
  {% if publi.pdf %}
    {% assign pdffile = "/publications/" | append:  publi.pdf  | append: ".pdf" %}
    {% for file in site.static_files %}
      {% if file.path contains pdffile %}
       {% assign pdfpresent = true %}
      {% endif %}
    {% endfor %}
  {% endif %}

{% if publi.year == myyear.year %}


{% assign bibtest = false %}
{% if publi.pdf %}
{% assign bibfile = "/publications/" | append:  publi.pdf  | append: ".txt" %}
{% for file in site.static_files %}
  {% if file.path contains bibfile %}
   {% assign bibtest = true %}
  {% endif %}
{% endfor %}
{% endif %}

<div class="well-sm publication-entry">
<ul class="flex-container">
<li class="flex-item1">
  {% if publi.image %}
     <img src="{{ site.url }}{{ site.baseurl }}/images/publications/{{ publi.image }}" class="img-responsive"/>
  {% endif %}
</li>
<li class="flex-item2">
  {% if publi.pdf %}<a href="{{ publi.pdf }}" target="_blank">{% endif %} <strong>{{ publi.title }}</strong>{% if publi.pdf %}</a>{% endif %}<br />
  {{ publi.authors }}<br />
  <em>{{ publi.display }}</em>{% if publi.year %}({{publi.year}}){% endif %}<br/>
  {% if publi.abstract %} <a data-bs-toggle="collapse" href="#{{publi.pdf}}"  class="btn-abstract" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false" aria-controls="{{publi.pdf}}">ABSTRACT</a> {% endif %}
  {% if bibtest == true %} <a data-bs-toggle="collapse" href="#{{publi.pdf}}2"  class="btn-bib" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false" aria-controls="{{publi.pdf}}2">BIB</a> {% endif %}
  {% if pdfpresent == true %}<a href="{{ pdffile }}" target="_blank"><button class="btn-pdf">PDF</button></a>{% endif %}
  {% if publi.doi %}<a href="http://doi.org/{{ publi.doi }}" target="_blank"><button class="btn-doi">DOI</button></a> {% endif %}
  {% if publi.arxiv %}<a href="https://arxiv.org/abs/{{ publi.arxiv }}" target="_blank"><button class="btn-arxiv">ARXIV</button></a> {% endif %}
  {% if publi.code %}<a href="{{ publi.code }}" target="_blank"><button class="btn-code">CODE</button></a> {% endif %}
  {% if publi.suppmat %}<a href="{{ publi.suppmat }}" target="_blank"><button class="btn-suppmat">SUPPLEMENT</button></a> {% endif %}

{% if publi.abstract %}
<br/>
<div class="collapse" id="{{publi.pdf}}"><div class="well-abstract">
 {{publi.abstract}}
</div></div>
{% endif %}

{% if bibtest == true %}
<div class="collapse" id="{{publi.pdf}}2"><div class="well-bib">
<iframe src='{{site.url}}{{site.baseurl}}/publications/{{publi.pdf}}.txt' scrolling="yes" width="100%" height="210" frameborder="0"></iframe>
</div></div>
{% endif %}

</li>
</ul>

</div>
{% endif %}
{% endfor %}

{% endfor %}

\* Joint first author.
