---
layout: page
title: Portfolio
icon: <i class="far fa-clipboard"></i>
permalink: /portfolio/
order: 2
---

# Computer Graphics

<div class="container">
  {% assign projects = site.projects | reverse %}
  {% for p in projects %}
  {% if p.tag == "graphics" %}
  <div class="row bottom-padding">
    <div class="col-5 no-lpadding">
        <a href="{{ p.permalink }}"><img class="project-thumb" src="{{ p.thumbnail }}"/></a>
    </div>
    <div class="col-7 no-rpadding">
      <h2><a href="{{ p.permalink }}">{{ p.short-title }}</a></h2>
      <p>{{ p.summary }}</p>
      <p>
      {% if p.project-type %}
      <a href="{{ p.permalink }}">
        <button>
          {% if p.project-type == "PDF Report" %}
            <i class="far fa-file-pdf"></i>
          {% else %}
            <i class="fas fa-globe-americas"></i>
          {% endif %}
          {{ p.project-type }}
        </button>
      </a>
      {% endif %}
      {% if p.github %}
        <a href="{{ p.github }}"><button><i class="fab fa-github"></i> GitHub</button></a>
      {% endif %}
      {% if p.video %}
        <a href="{{ p.video }}"><button><i class="far fa-play-circle"></i> Video</button></a>
      {% endif %}
      </p>
    </div>
  </div>
  {% endif %}
  {% endfor %}
</div>


# Deep Learning

<div class="container">
  {% assign projects = site.projects | reverse %}
  {% for p in projects %}
  {% if p.tag == "deep-learning" %}
  <div class="row bottom-padding">
    <div class="col-5 no-lpadding">
        <a href="{{ p.permalink }}"><img class="project-thumb" src="{{ p.thumbnail }}"/></a>
    </div>
    <div class="col-7 no-rpadding">
      <h2><a href="{{ p.permalink }}">{{ p.short-title }}</a></h2>
      <p>{{ p.summary }}</p>
      <p>
      {% if p.project-type %}
      <a href="{{ p.permalink }}">
        <button>
          {% if p.project-type == "PDF Report" %}
            <i class="far fa-file-pdf"></i>
          {% else %}
            <i class="fas fa-globe-americas"></i>
          {% endif %}
          {{ p.project-type }}
        </button>
      </a>
      {% endif %}
      {% if p.github %}
        <a href="{{ p.github }}"><button><i class="fab fa-github"></i> GitHub</button></a>
      {% endif %}
      {% if p.video %}
        <a href="{{ p.video }}"><button><i class="far fa-play-circle"></i> Video</button></a>
      {% endif %}
      </p>
    </div>
  </div>
  {% endif %}
  {% endfor %}
</div>
