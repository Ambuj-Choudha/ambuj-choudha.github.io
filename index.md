---
layout: default
title: Home
---

<section class="hero">
  <h1>Ambuj Choudha</h1>
  <p class="hero-pitch">
    <!-- Replace with your one-line pitch. Example:
         "MSc student building real-time computer vision systems for autonomous perception." -->
    Computer vision & ML engineer — building real-time perception systems.
  </p>

  <div class="hero-cta">
    <a class="cta-button primary" href="{{ '/assets/resume.pdf' | relative_url }}">⬇ Resume PDF</a>
    {% if site.author.github %}
      <a class="cta-button" href="https://github.com/{{ site.author.github }}">GitHub</a>
    {% endif %}
    {% if site.author.linkedin and site.author.linkedin != "" %}
      <a class="cta-button" href="https://www.linkedin.com/in/{{ site.author.linkedin }}">LinkedIn</a>
    {% endif %}
    <a class="cta-button" href="mailto:{{ site.author.email }}">Email</a>
  </div>

  <p class="hero-currently">
    <!-- One sentence: what you are working on RIGHT NOW. Updates every few months. -->
    <strong>Currently:</strong> exploring real-time object detection & tracking on edge hardware.
  </p>
</section>

<div class="section-heading">
  <h2>Selected work</h2>
  <a class="see-all" href="{{ '/projects/' | relative_url }}">all projects →</a>
</div>

<ul class="post-list">
  {% for project in site.data.featured_projects limit:2 %}
    <li class="post-item">
      <h3 class="post-item-title">{{ project.title }}</h3>
      <div class="post-meta">{{ project.year }} :: {{ project.stack }}</div>
      <p class="project-result"><strong>Result:</strong> {{ project.result }}</p>
      <p class="excerpt">{{ project.summary }}</p>
      {% if project.link %}<a class="read-more" href="{{ project.link }}">Read more</a>{% endif %}
    </li>
  {% else %}
    <li class="post-item">
      <p class="excerpt">
        Add featured projects to <code>_data/featured_projects.yml</code> to
        surface them here. Full list on the <a href="{{ '/projects/' | relative_url }}">projects</a> page.
      </p>
    </li>
  {% endfor %}
</ul>

<div class="section-heading">
  <h2>Latest writing</h2>
  <a class="see-all" href="{{ '/blog/' | relative_url }}">all posts →</a>
</div>

<ul class="post-list">
  {% for post in site.posts limit:3 %}
    <li class="post-item">
      <h3 class="post-item-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <div class="post-meta">
        {{ post.date | date: "%Y-%m-%d" }} :: {{ post.author | default: site.author.name }}
      </div>
      {% if post.tags %}
        <div class="tags">
          {% for tag in post.tags %}<span class="tag">#{{ tag }}</span>{% endfor %}
        </div>
      {% endif %}
      <p class="excerpt">{{ post.excerpt | strip_html | truncate: 180 }}</p>
      <a class="read-more" href="{{ post.url | relative_url }}">Read more</a>
    </li>
  {% endfor %}
</ul>
