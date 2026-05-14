---
layout: page
title: Projects
permalink: /projects/
description: A summary of my academic projects developed independently.
nav: true
---

<div class="projects-table">
  <table class="table table-hover table-sm border-0">
    <thead>
      <tr>
        <th scope="col" style="width: 25%">Title</th>
        <th scope="col" style="width: 20%">Keywords</th>
        <th scope="col">Abstract</th>
      </tr>
    </thead>
    <tbody>
      {% for project in site.data.projects_list %}
      <tr>
        <td class="font-weight-bold">{{ project.title }}</td>
        <td>{{ project.keywords }}</td>
        <td class="text-justify">
        <p>
          <details>
            <summary style="cursor: pointer;">
              {{ project.abstract | truncate: 300 }} <span class="text-info">[...]</span>
            </summary>
            <div class="card card-body mt-2 shadow-none border-0 bg-light">
            {{ project.abstract }}
            </div>
          </details>
        </p>
        </td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<!-- <ul class="post-list">
  {% for project in site.data.projects_list %}
  <li>
    <div class="row">
      <div class="col-sm-9">
        <h5>{{ project.title }}</h5>
        <p class="project-keywords"><em>{{ project.keywords }}</em></p>
        <p>
          <details>
            <summary style="cursor: pointer;">
              {{ project.abstract | truncate: 300 }} <span class="text-info">[...]</span>
            </summary>
            <div class="card card-body mt-2 shadow-none border-0 bg-light">
            {{ project.abstract }}
            </div>
          </details>
        </p>
      </div>
    </div>
    <hr>
  </li>
  {% endfor %}
</ul> -->