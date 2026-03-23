---
layout: default
---

<div class="hero">
  <h1>Empowering the Next Generation of AI Scholars</h1>
  <p>Join BtechInAI to master the future of technology with premium educational resources, career mentorship, and hands-on AI projects designed for current and aspiring AI practitioners.</p>
  <a href="#getting-started" class="site-nav page-link" style="font-size: 1.25rem; font-weight: 700;">Explore Courses →</a>
</div>

<div id="getting-started" class="features-grid">
  <div class="feature-card">
    <h3>High-Quality AI Courses</h3>
    <p>Dive deep into Machine Learning, Deep Learning, and Neural Networks with world-class curriculum.</p>
  </div>
  <div class="feature-card">
    <h3>Career Guidance</h3>
    <p>Strategic mentorship to help you secure prestigious roles in the AI industry.</p>
  </div>
  <div class="feature-card">
    <h3>Hands-on Projects</h3>
    <p>Build your portfolio with real-world applications and cutting-edge Research & Development.</p>
  </div>
</div>

<div class="wrapper" style="margin-top: 80px;">
  <h2 style="font-size: 2rem; font-weight: 800; margin-bottom: 30px;">Latest from the Blog</h2>
  
  {% if site.posts.size > 0 %}
    <ul class="post-list">
      {% for post in site.posts %}
        <li>
          <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
          <h3>
            <a class="post-link" href="{{ post.url | relative_url }}">
              {{ post.title | escape }}
            </a>
          </h3>
          {% if site.show_excerpts %}
            {{ post.excerpt }}
          {% endif %}
        </li>
      {% endfor %}
    </ul>
  {% endif %}
</div>
