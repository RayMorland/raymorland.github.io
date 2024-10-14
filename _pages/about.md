---
layout: default
title: About
permalink: /about/
---

  <div class="container d-flex flex-column gap-4">
  <h1 class="fw-bold">About</h1>
  <div class="row mb-2">
  <div class="col-md-3">
    <h2 class="mb-3">Employment</h2>
    </div>
    <div class="col-md-9">
    {% for job in site.data.employment %}
      <div class="d-flex flex-row justify-content-between mb-2">
        <div>
          <a
            href="{{ job.link }}"
            target="_blank"
            rel="noopener noreferrer">
            <h3>{{ job.employer }}</h3>

          </a>
          <h4>{{ job.department }}</h4>
          <h4>
            {{ job.title }}</h4>
        </div>

        <h4>{{ job.startMonth }} {{ job.startYear }} - {{ job.endMonth }} {{ job.endYear }}</h4>
      </div>
    {% endfor %}
</div>
  </div>

  <div class="row mb-2">
    <div class="col-md-3">
      <h2 class="mb-3">Education</h2>
    </div>
    <div class="col-md-9">
      {% for education in site.data.education %}
        <div class="d-flex flex-row justify-content-between mb-2">
          <div>
            <a
              href="{{ education.link }}"
              target="_blank"
              rel="noopener noreferrer">
              <h3>{{ education.school }}</h3>
            </a>
            <h4>
              {{ education.degree }} - {{ education.major }}
            </h4>
            <p>{{ education.description }}</p>
          </div>

          <h4>{{ education.startMonth }} {{ education.startYear }} - {{ education.endMonth }} {{ education.endYear }}</h4>
        </div>
      {% endfor %}
    </div>
</div>
  </div>
