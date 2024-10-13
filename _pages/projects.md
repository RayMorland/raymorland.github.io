---
layout: default
title: Projects
permalink: /projects
---

  <hr>
  <div class="row mb-2">
    <h2 class="mb-3">Work</h2>
    {% for project in site.data.projects %}
      <div class="d-flex flex-row justify-content-between mb-2">
        <div>
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
        </div>

        <h4>{{ project.startMonth }} {{ project.startYear }} - {{ project.endMonth }} {{ project.endYear }}</h4>
      </div>
    {% endfor %}

  </div>
