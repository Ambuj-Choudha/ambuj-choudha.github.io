---
layout: default
title: Resume
permalink: /resume/
---

<div class="resume-header">
  <h1>~/resume</h1>
  <a class="cta-button primary" href="{{ '/assets/resume.pdf' | relative_url }}">⬇ Download PDF</a>
</div>

**Ambuj Choudha**
[email]({{ 'mailto:' | append: site.author.email }})
{% if site.author.github %}· [github](https://github.com/{{ site.author.github }}){% endif %}
{% if site.author.linkedin and site.author.linkedin != "" %}· [linkedin](https://www.linkedin.com/in/{{ site.author.linkedin }}){% endif %}
{% if site.author.scholar and site.author.scholar != "" %}· [scholar](https://scholar.google.com/citations?user={{ site.author.scholar }}){% endif %}

<section class="resume-section">
<h2>Experience</h2>

<div class="resume-row">
  <div class="resume-role">Role Title — Company</div>
  <div class="resume-when">2024 — Present</div>
</div>
<ul>
  <li>Bullet describing impact, ideally with a number.</li>
  <li>Bullet describing a specific technical contribution.</li>
</ul>

<div class="resume-row">
  <div class="resume-role">Previous Role — Company</div>
  <div class="resume-when">2022 — 2024</div>
</div>
<ul>
  <li>Bullet describing impact.</li>
  <li>Bullet describing a specific technical contribution.</li>
</ul>
</section>

<section class="resume-section">
<h2>Education</h2>

<div class="resume-row">
  <div class="resume-role">M.Sc. / B.Sc. Program — University</div>
  <div class="resume-when">Year — Year</div>
</div>
<p>Notable coursework, thesis, or honors.</p>
</section>

<section class="resume-section">
<h2>Skills</h2>

<p>
  <strong>Languages:</strong>
  <span class="tag">#python</span>
  <span class="tag">#c++</span>
  <span class="tag">#cuda</span>
</p>
<p>
  <strong>ML / CV:</strong>
  <span class="tag">#pytorch</span>
  <span class="tag">#tensorrt</span>
  <span class="tag">#opencv</span>
  <span class="tag">#onnx</span>
  <span class="tag">#numpy</span>
</p>
<p>
  <strong>Tools:</strong>
  <span class="tag">#docker</span>
  <span class="tag">#git</span>
  <span class="tag">#linux</span>
</p>
<p>
  <strong>Domains:</strong>
  <span class="tag">#computer-vision</span>
  <span class="tag">#deep-learning</span>
  <span class="tag">#real-time-systems</span>
</p>
</section>

<section class="resume-section">
<h2>Selected projects</h2>
<p>See <a href="/projects/">~/projects</a> for the full list.</p>
</section>
