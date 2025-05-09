---
title: "Education"
layout: gridlay
sitemap: false
permalink: /education/
---

# Education

{% if site.courses %}
<!-- Sort courses by year -->
{% assign courses = site.courses | sort: 'year_start' | reverse %}

## Courses Taught
<div class="rowl1" style="padding-top: 10px;">

{% for course in courses %}
{{ forloop.index }}. {% if course.url %}<a href="{{ course.url }}" target="_blank">{% endif %} <strong>{{ course.name }}</strong> {% if course.name_url %}</a>{% endif %} ({{ course.institution }}, {{ course.year_start }}–{{ course.year_end }}) {% if course.type == 'bs' %}<button class="btn-completed">BS Cyber Security</button>{% endif %}{% if course.type == 'ms' %}<button class="btn-inprogress">MS</button>{% endif %}{% if course.type == 'phd' %}<button class="btn-notstarted">PhD</button>{% endif %}{% if course.comment %} – {{ course.comment }}{% endif %}
<br/>
<i>{{ course.code }}. {{ course.subheading }}</i>.

{% endfor %}

</div>
{% endif %}


{% if site.data.degrees %}
<!-- Sort courses by year -->
{% assign students = site.data.degrees | sort: 'year' | reverse %}
## Degrees
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

{{ forloop.index }}. {% if student.name_url %}<a href="{{ student.name_url }}" target="_blank">{% endif %} <strong>{{ student.name }}</strong> {% if student.name_url %}</a>{% endif %} ({{ student.year }}) {% if student.status == 'notstarted' %}<button class="btn-notstarted">NOT STARTED</button>{% endif %}{% if student.status == 'bs' %}<button class="btn-inprogress">UNDERGRADUATE</button>{% endif %}{% if student.status == 'ms' %}<button class="btn-completed">GRADUATE</button>{% endif %}{% if student.comment %} – {{ student.comment }}{% endif %}
<br/>
<i>{{ student.project }}</i>{% if pdffile %} (<a href="{{ pdffile }}" target="_blank">link</a>){% endif %}.

{% endfor %}
</div>
{% endif %}


{% if site.data.thesis_azhar %}
<!-- Sort courses by year -->
{% assign students = site.data.thesis_azhar | sort: 'year' | reverse %}
## Master's Thesis
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



{% if site.data.awards %}
## Courses & Certifications
<div class="rowl1" style="padding-top: 10px;">

{% for award in site.data.awards %}
{{ forloop.index }}. {% if award.name_url %}<a href="{{ award.name_url }}" target="_blank">{% endif %}<strong>{{ award.name }}</strong>{% if award.name_url %}</a>{% endif %} {% if award.organisation %} from {% if award.organisation_url %}<a href="{{ award.organisation_url }}" target="_blank">{% endif %} {{ award.organisation }}{% if award.organisation_url %}</a>{% endif %}{% endif %}{% if award.subtitle %}: {{ award.subtitle }}{% endif %} ({{ award.year }}).
{% endfor %}
</div>
{% endif %}




{% if site.data.medium %}
<!-- Sort students by year -->
{% assign students = site.data.medium | sort: 'year' | reverse %}
## Cyber Security Writings
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

{{ forloop.index }}. {% if student.name_url %}<a href="{{ student.name_url }}" target="_blank">{% endif %} <strong>{{ student.name }}</strong> {% if student.name_url %}</a>{% endif %} ({{ student.year }}) {% if student.status == 'incomplete' %}<button class="btn-notstarted">INCOMPLETE</button>{% endif %}{% if student.status == 'inprogress' %}<button class="btn-inprogress">IN PROGRESS</button>{% endif %}{% if student.status == 'published' %}<button class="btn-completed">PUBLISHED</button>{% endif %}{% if student.comment %} – {{ student.comment }}{% endif %}
<br/>
<i>{{ student.project }}</i>{% if pdffile %} (<a href="{{ pdffile }}" target="_blank">link</a>){% endif %}.

{% endfor %}
</div>
{% endif %}




{% if site.data.manuals %}
<!-- Sort courses by year -->
{% assign students = site.data.manuals | sort: 'year' | reverse %}
## Hands-On Cybercraft
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
