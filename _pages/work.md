---
layout: page
title: Research
permalink: /work/
description: What I have done, am doing, and will be doing! (to be updated)
nav: true
nav_order: 3
display_categories: [research]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
  <!-- Conditionally display projects based on categories -->
  {%- if site.enable_project_categories and page.display_categories %}
    {%- for category in page.display_categories %}
      <h2 class="category">{{ category }}</h2>
      {%- assign categorized_work = site.work | where: "category", category %}
      {%- assign sorted_work = categorized_work | sort: "importance" %}
      <!-- Check if there are projects to display -->
      {%- if sorted_work.size > 0 %}
        <div class="grid">
          {%- for project in sorted_work %}
            {% include projects.html %}
          {%- endfor %}
        </div>
      {%- else %}
        <p>No projects available in {{ category }} category.</p>
      {%- endif %}
    {%- endfor %}

  {%- else %}
    <!-- Display all projects when categories are not enabled or specified -->
    {%- assign sorted_work = site.work | sort: "importance" %}
    <!-- Check if there are projects to display -->
    {%- if sorted_work.size > 0 %}
      {% if page.horizontal %}
        <div class="container">
          <div class="row row-cols-2">
            {%- for project in sorted_work %}
              {% include projects_horizontal.html %}
            {%- endfor %}
          </div>
        </div>
      {% else %}
        <div class="grid">
          {%- for project in sorted_work %}
            {% include projects.html %}
          {%- endfor %}
        </div>
      {% endif %}
    {%- else %}
      <p>No projects available at this time.</p>
    {%- endif %}
  {%- endif %}
</div>
