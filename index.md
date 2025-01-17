---
layout: default
title: "John Doe"
---

# John Doe

I'm a software engineer specializing in full-stack web development. 
I love creating efficient, scalable, and user-friendly applications.

Below are some of my recent projects:

<div class="projects-grid">
{% for project in site.data.projects %}
  <div class="project-card">
    <img src="{{ project.image }}" alt="{{ project.name }}">
    <h3>{{ project.name }}</h3>
    <p><strong>Role:</strong> {{ project.role }}</p>
    <p>{{ project.description }}</p>
  </div>
{% endfor %}
</div>
