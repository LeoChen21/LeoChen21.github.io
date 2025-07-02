---
layout: archive
permalink: /publications/
author_profile: true
---

<style>
.publications-hero {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 3rem 2rem;
  margin: 0 0 3rem 0;
  text-align: center;
  border-radius: 20px;
  position: relative;
  overflow: hidden;
}

.publications-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="books" width="50" height="50" patternUnits="userSpaceOnUse"><text x="25" y="25" text-anchor="middle" fill="white" opacity="0.1" font-size="20">📚</text></pattern></defs><rect width="100" height="100" fill="url(%23books)"/></svg>');
  opacity: 0.3;
}

.publications-hero-content {
  position: relative;
  z-index: 2;
}

.publications-hero h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  font-weight: 700;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

.publications-hero p {
  font-size: 1.2rem;
  opacity: 0.9;
  max-width: 600px;
  margin: 0 auto 2rem auto;
  line-height: 1.6;
}

.scholar-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.75rem 1.5rem;
  background: rgba(255,255,255,0.2);
  color: white !important;
  text-decoration: none;
  border-radius: 25px;
  font-weight: 500;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.3);
  transition: all 0.3s ease;
  margin-top: 1rem;
}

.scholar-link:hover {
  background: rgba(255,255,255,0.3);
  transform: translateY(-2px);
  text-decoration: none;
  color: white !important;
}

.publications-stats {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin: 2rem 0;
  flex-wrap: wrap;
}

.stat-item {
  background: rgba(255,255,255,0.15);
  padding: 1rem 1.5rem;
  border-radius: 15px;
  text-align: center;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.2);
}

.stat-number {
  font-size: 1.8rem;
  font-weight: 700;
  display: block;
}

.stat-label {
  font-size: 0.9rem;
  opacity: 0.8;
  margin-top: 0.25rem;
}

.publications-container {
  margin: 2rem 0;
}

.publication-item {
  background: #fff;
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  margin-bottom: 2rem;
  overflow: hidden;
  border: 1px solid #e1e8ed;
  transition: all 0.3s ease;
}

.publication-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 40px rgba(0,0,0,0.15);
}

.publication-header {
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  padding: 2rem;
  border-bottom: 1px solid #e1e8ed;
  position: relative;
}

.publication-type {
  position: absolute;
  top: 1rem;
  right: 1rem;
  background: #667eea;
  color: white;
  padding: 0.25rem 0.75rem;
  border-radius: 15px;
  font-size: 0.8rem;
  font-weight: 600;
}

.publication-title {
  font-size: 1.4rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 1rem;
  line-height: 1.4;
  padding-right: 4rem;
}

.publication-authors {
  font-size: 0.95rem;
  color: #666;
  margin-bottom: 0.5rem;
}

.publication-venue {
  font-size: 0.9rem;
  color: #28a745;
  font-weight: 500;
  margin-bottom: 0.5rem;
}

.publication-date {
  font-size: 0.85rem;
  color: #999;
}

.publication-content {
  padding: 1.5rem 2rem;
}

.publication-excerpt {
  font-size: 1rem;
  line-height: 1.7;
  color: #555;
  margin-bottom: 1.5rem;
}

.publication-links {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

.publication-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 1rem;
  background: #667eea;
  color: white !important;
  text-decoration: none;
  border-radius: 20px;
  font-size: 0.85rem;
  font-weight: 500;
  transition: all 0.3s ease;
}

.publication-link:hover {
  background: #5a6fd8;
  transform: translateY(-2px);
  text-decoration: none;
  color: white !important;
}

.publication-link.pdf {
  background: #dc3545;
}

.publication-link.pdf:hover {
  background: #c82333;
}

.citation-section {
  background: #f8f9fa;
  border-top: 1px solid #e1e8ed;
  padding: 1.5rem 2rem;
}

.citation-title {
  font-size: 0.9rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 0.75rem;
}

.citation-text {
  font-family: 'Courier New', monospace;
  font-size: 0.8rem;
  background: #fff;
  padding: 1rem;
  border-radius: 8px;
  border: 1px solid #dee2e6;
  white-space: pre-wrap;
  word-break: break-all;
  line-height: 1.4;
  color: #495057;
}

.no-publications {
  text-align: center;
  padding: 4rem 2rem;
  background: #f8f9fa;
  border-radius: 15px;
  margin: 2rem 0;
}

.no-publications-icon {
  font-size: 4rem;
  margin-bottom: 1rem;
  opacity: 0.6;
}

.no-publications h3 {
  font-size: 1.5rem;
  color: #2c3e50;
  margin-bottom: 1rem;
}

.no-publications p {
  color: #666;
  font-size: 1rem;
}

.research-areas {
  background: #fff;
  padding: 2rem;
  border-radius: 15px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
  margin: 2rem 0;
  border: 1px solid #e1e8ed;
}

.research-areas h3 {
  font-size: 1.3rem;
  color: #2c3e50;
  margin-bottom: 1rem;
  text-align: center;
}

.research-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  justify-content: center;
}

.research-tag {
  background: #e3f2fd;
  color: #1976d2;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-size: 0.9rem;
  font-weight: 500;
}

@media (max-width: 768px) {
  .publications-hero {
    margin: 0 0 2rem 0;
    padding: 2rem 1rem;
  }
  
  .publications-hero h1 {
    font-size: 2rem;
  }
  
  .publications-stats {
    flex-direction: column;
    align-items: center;
    gap: 1rem;
  }
  
  .publication-header {
    padding: 1.5rem;
  }
  
  .publication-title {
    padding-right: 0;
    margin-bottom: 1rem;
  }
  
  .publication-type {
    position: static;
    display: inline-block;
    margin-bottom: 1rem;
  }
  
  .publication-content {
    padding: 1rem 1.5rem;
  }
  
  .publication-links {
    flex-direction: column;
  }
  
  .citation-section {
    padding: 1rem 1.5rem;
  }
}
</style>

<div class="publications-hero">
  <div class="publications-hero-content">
    <h1>📚 Research & Publications</h1>
    <p>
      Explore my contributions to academic research in computer vision, machine learning, and competitive programming challenges.
    </p>
    
    {% if site.author.googlescholar %}
    <a href="{{site.author.googlescholar}}" target="_blank" class="scholar-link">
      🎓 Visit Google Scholar Profile
    </a>
    {% endif %}
    
    <div class="publications-stats">
      <div class="stat-item">
        <span class="stat-number">{{ site.publications.size | default: 1 }}</span>
        <span class="stat-label">Publications</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">2024</span>
        <span class="stat-label">Latest Work</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">CV</span>
        <span class="stat-label">Research Focus</span>
      </div>
    </div>
  </div>
</div>

{% include base_path %}

<div class="research-areas">
  <h3>🔬 Research Areas</h3>
  <div class="research-tags">
    <span class="research-tag">Computer Vision</span>
    <span class="research-tag">Low-Power Computing</span>
    <span class="research-tag">Machine Learning Competitions</span>
    <span class="research-tag">Edge AI</span>
    <span class="research-tag">Model Optimization</span>
    <span class="research-tag">Performance Analysis</span>
  </div>
</div>

<div class="publications-container">
  {% assign publication_count = site.publications.size %}
  {% if publication_count > 0 %}
    {% for post in site.publications reversed %}
      <div class="publication-item">
        <div class="publication-header">
          <div class="publication-type">📄 {{ post.venue | default: "Research Paper" }}</div>
          <h3 class="publication-title">{{ post.title }}</h3>
          
          {% if post.authors %}
            <div class="publication-authors">
              <strong>Authors:</strong> {{ post.authors }}
            </div>
          {% endif %}
          
          {% if post.venue %}
            <div class="publication-venue">
              📍 {{ post.venue }}
            </div>
          {% endif %}
          
          {% if post.date %}
            <div class="publication-date">
              📅 {{ post.date | date: "%B %Y" }}
            </div>
          {% endif %}
        </div>
        
        <div class="publication-content">
          {% if post.excerpt %}
            <p class="publication-excerpt">{{ post.excerpt | strip_html }}</p>
          {% endif %}
          
          <div class="publication-links">
            <a href="{{ post.url | relative_url }}" class="publication-link">
              📖 Read More
            </a>
            
            {% if post.paperurl %}
              <a href="{{ post.paperurl }}" target="_blank" class="publication-link pdf">
                📄 View Paper
              </a>
            {% endif %}
            
            {% if post.code %}
              <a href="{{ post.code }}" target="_blank" class="publication-link">
                💻 Source Code
              </a>
            {% endif %}
            
            {% if post.slides %}
              <a href="{{ post.slides }}" target="_blank" class="publication-link">
                📊 Slides
              </a>
            {% endif %}
          </div>
        </div>
        
        {% if post.citation %}
          <div class="citation-section">
            <div class="citation-title">📋 Citation</div>
            <div class="citation-text">{{ post.citation }}</div>
          </div>
        {% endif %}
      </div>
    {% endfor %}
  {% else %}
    <div class="no-publications">
      <div class="no-publications-icon">📝</div>
      <h3>Publications Coming Soon</h3>
      <p>I'm actively working on research projects. Check back for updates on my latest publications!</p>
    </div>
  {% endif %}
</div>

<div style="margin-top: 3rem; padding: 2rem; background: linear-gradient(135deg, #28a745 0%, #20c997 100%); border-radius: 15px; text-align: center; color: white;">
  <h3 style="margin-bottom: 1rem;">🤝 Collaborate with Me</h3>
  <p style="opacity: 0.9; margin-bottom: 1.5rem;">Interested in research collaboration or have questions about my work?</p>
  <div style="display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap;">
    <a href="/portfolio/" style="display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.75rem 1.5rem; background: rgba(255,255,255,0.2); color: white; text-decoration: none; border-radius: 25px; font-weight: 500; backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.3);">
      💼 View Projects
    </a>
    <a href="/cv/" style="display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.75rem 1.5rem; background: rgba(255,255,255,0.2); color: white; text-decoration: none; border-radius: 25px; font-weight: 500; backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.3);">
      📄 Download CV
    </a>
  </div>
</div>
