---
layout: default
is_contact: true
---

<h1 class="mt-4">Publications</h1>
<h4 class="mt-4">Conference papers</h4>

{% assign publications = site.conf | sort: "year" | reverse %}
{% for pub in publications %}
<div class="pubitem">
<div class="pubteaser">
  <a href="{{pub.project}}">
    <img
      src="/images/publication-pages/{{ pub.slug }}_small.png"
      alt="{{pub.slug}} publication teaser"
    />
  </a>
</div>
  <div class="pubtitle">{{ pub.title }}</div>
  <div class="pubauthors">{{ pub.authors }}</div>
  <div class="pubinfo">{{ pub.publication }}, {{ pub.year}}</div>
  <div class="publinks">
  <a href="{{ pub.pdf }}"><i class="far fa-file-pdf"></i> PDF</a
  >&nbsp;&nbsp;
  <a href="{{ pub.project }}"><i class="fas fa-link"></i> Project Page</a>
</div>
</div>
{% endfor %}

<h4 class="mt-4">Talk</h4>

{% assign publications = site.talks | sort: "year" | reverse %}
{% for pub in publications %}
<div class="pubitem">
<div class="pubteaser">
  <a href="{{pub.project}}">
    <img
      src="/images/publication-pages/{{ pub.slug }}_small.png"
      alt="{{pub.slug}} publication teaser"
    />
  </a>
</div>
  <div class="pubtitle">{{ pub.title }}</div>
  <div class="pubauthors">{{ pub.authors }}</div>
  <div class="pubinfo">{{ pub.publication }}, {{ pub.year}}</div>
  <div class="publinks">
  <a href="{{ pub.pdf }}"><i class="far fa-file-pdf"></i> PDF</a
  >&nbsp;&nbsp;
  <a href="{{ pub.project }}"><i class="fas fa-link"></i> Project Page</a>
</div>
</div>
{% endfor %}

<h2 class="mt-4">Project</h2>

{% assign publications = site.projects | sort: "year" | reverse %}
{% for pub in publications %}
<div class="pubitem">
<div class="pubteaser">
  <a href="{{pub.project}}">
    <img
      src="/images/publication-pages/{{ pub.slug }}_small.png"
      alt="{{pub.slug}} publication teaser"
    />
  </a>
</div>
  <div class="pubtitle">{{ pub.title }}</div>
  <div class="pubinfo"><it>{{ pub.info }}</it></div>
  <div class="publinks">
  <a href="{{ pub.project }}"><i class="fas fa-link"></i> Project Page</a>
</div>
</div>
{% endfor %}