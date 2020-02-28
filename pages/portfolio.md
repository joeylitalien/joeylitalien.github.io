---
layout: page
title: Portfolio
icon: <i class="far fa-clipboard"></i>
permalink: /portfolio/
order: 2
---

# Publications
<section>
  <div class="container">
    {% assign pubs = site.publications %}
    {% for p in pubs limit:2 %}
    <div class="row bottom-padding">
      <div class="col-2 no-padding">
        <a href="{{ p.permalink }}">
          <img class="project-thumb" src="{{ p.thumbnail }}">
        </a>
      </div>
      <div class="col-10 no-rpadding">
        <h3><a href="{{ p.permalink }}">{{ p.title }}</a></h3>
        <p>
          <!-- List of authors -->
          {% for a in p.authors %}
            {% if forloop.last and forloop.length != 1 %}
              and 
              {% if a.author.name == "Joey Litalien" %}
                <b>{{ a.author.name }}</b>
              {% else %}
                {{ a.author.name }}
              {% endif %}
            {% else %} 
              {% if a.author.name == "Joey Litalien" %}
                <b>{{ a.author.name }}</b>{% if forloop.length != 1 %}, {% endif %}
              {% else %}
                {{ a.author.name }},
              {% endif %}
            {% endif %}
          {% endfor %}
          <br>
          <!-- Journal information -->
          <i>
            {{ p.journal }}
            {% if p.journal-note %}
              ({{ p.journal-note }}),
            {% endif %}
          </i> 
          {% assign dl = p.downloads %}
          {% if dl.published %} {{ p.month }} {% endif %} {{ p.year }}
        </p>
        <ul class="fa-ul inline-list">
          <li class="fa-li"><i class="fas fa-globe-americas"></i>
            <a href="{{ p.permalink }}">Project page</a>
          </li>
          {% if dl.published %}
            <li class="fa-li"><i class="far fa-file-pdf"></i>
              <a href="{{ dl.paper.file }}">Paper ({{ dl.paper.size }} pdf)</a>
            </li>
            {% if dl.doi.url %}
            <li class="fa-li"><i class="fas fa-atlas"></i>
              <a href="{{ dl.doi.url }}">Publisher's version</a>
            </li>
            {% endif %}
            {% if dl.supplementary.file %}
            <li class="fa-li"><i class="far fa-file-archive"></i>
              <a href="{{ dl.supplementary.url }}">Supplemental</a>
            </li>
            {% endif %}
            {% if dl.code.url %}
            <li class="fa-li"><i class="fab fa-github"></i>
              <a href="{{ dl.code.url }}">Code</a>
            </li>
            {% endif %}
          {% endif %}
        </ul>
      </div>
    </div>
    {% endfor %}
  </div>
</section>

# Other Projects
<section>
  <div class="container">
    {% assign projects = site.projects | sort: 'featured' | reverse %}
    {% for p in projects limit:5%}
    <div class="row bottom-padding">
      <div class="col-2 no-padding">
        <a href="{{ p.permalink }}"><img class="project-thumb" src="{{ p.thumbnail }}"/></a>
      </div>
      <div class="col-10 no-rpadding">
        <h3><a href="{{ p.permalink }}">{{ p.short-title }}</a></h3>
        <p class="justified">{{ p.summary }}</p>
        <ul class="fa-ul inline-list">
          {% if p.report.file %}
          <li class="fa-li"><i class="far fa-file-pdf"></i>
            <a href="{{ p.report.file }}">Report ({{ p.report.size }} pdf)</a>
          </li>
          {% endif %}
          {% if p.code.url %}
          <li class="fa-li"><i class="fab fa-github"></i>
            <a href="{{ p.code.url }}">Code repository (Git)</a>
          </li>
          {% endif %}
        </ul>
      </div>
    </div>
  {% endfor %}
  </div>
</section>