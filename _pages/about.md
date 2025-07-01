---
permalink: /
title: "Leo Chen's Personal Website"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.hero-section {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 4rem 2rem;
  margin: -2rem -2rem 3rem -2rem;
  text-align: center;
  border-radius: 0 0 25px 25px;
  position: relative;
  overflow: hidden;
}

.hero-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="20" cy="20" r="1" fill="white" opacity="0.1"/><circle cx="80" cy="80" r="1" fill="white" opacity="0.1"/><circle cx="40" cy="60" r="1" fill="white" opacity="0.05"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>');
  opacity: 0.3;
}

.hero-content {
  position: relative;
  z-index: 2;
}

.hero-title {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 1rem;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

.hero-subtitle {
  font-size: 1.3rem;
  opacity: 0.9;
  margin-bottom: 2rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
  line-height: 1.6;
}

.hero-image-container {
  margin: 2rem 0;
  position: relative;
}

.hero-image {
  max-width: 100%;
  height: auto;
  border-radius: 15px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.2);
  transition: transform 0.3s ease;
}

.hero-image:hover {
  transform: scale(1.02);
}

.quick-links {
  display: flex;
  gap: 1.5rem;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 2rem;
}

.hero-link {
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
}

.hero-link:hover {
  background: rgba(255,255,255,0.3);
  transform: translateY(-2px);
  text-decoration: none;
  color: white !important;
}

.content-section {
  background: #fff;
  padding: 3rem 2rem;
  margin: 2rem 0;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  border: 1px solid #e1e8ed;
}

.section-title {
  font-size: 2rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 1.5rem;
  text-align: center;
  position: relative;
}

.section-title::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 50%;
  transform: translateX(-50%);
  width: 60px;
  height: 3px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border-radius: 2px;
}

.intro-text {
  font-size: 1.1rem;
  line-height: 1.8;
  color: #555;
  text-align: center;
  max-width: 800px;
  margin: 0 auto;
}

.highlights-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
}

.highlight-card {
  background: #f8f9fa;
  padding: 2rem;
  border-radius: 15px;
  text-align: center;
  transition: transform 0.3s ease;
  border: 1px solid #e9ecef;
}

.highlight-card:hover {
  transform: translateY(-5px);
}

.highlight-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.highlight-title {
  font-size: 1.2rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 0.5rem;
}

.highlight-desc {
  color: #666;
  font-size: 0.95rem;
  line-height: 1.6;
}

.cta-section {
  background: linear-gradient(135deg, #28a745 0%, #20c997 100%);
  color: white;
  padding: 3rem 2rem;
  margin: 3rem 0;
  border-radius: 20px;
  text-align: center;
}

.cta-title {
  font-size: 1.8rem;
  font-weight: 600;
  margin-bottom: 1rem;
}

.cta-text {
  font-size: 1.1rem;
  opacity: 0.9;
  margin-bottom: 2rem;
}

.cta-buttons {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}

.cta-button {
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
}

.cta-button:hover {
  background: rgba(255,255,255,0.3);
  transform: translateY(-2px);
  text-decoration: none;
  color: white !important;
}

@media (max-width: 768px) {
  .hero-section {
    margin: -1rem -1rem 2rem -1rem;
    padding: 3rem 1rem;
  }
  
  .hero-title {
    font-size: 2.2rem;
  }
  
  .hero-subtitle {
    font-size: 1.1rem;
  }
  
  .quick-links {
    flex-direction: column;
    align-items: center;
  }
  
  .content-section {
    margin: 1rem 0;
    padding: 2rem 1rem;
  }
  
  .highlights-grid {
    grid-template-columns: 1fr;
    gap: 1rem;
  }
}
</style>

<div class="hero-section">
  <div class="hero-content">
    <h1 class="hero-title">👋 Hello, I'm Leo Chen</h1>
    <p class="hero-subtitle">
      Welcome to my digital journey through software engineering, computer vision, and innovative technology solutions.
    </p>
    
    <div class="hero-image-container">
      <img src="images/Hero-Image.png" alt="Leo Chen's Portfolio Showcase" class="hero-image">
    </div>
    
    <div class="quick-links">
      <a href="https://github.com/LeoChen21/LeoChen21.github.io" class="hero-link" target="_blank">
        🔗 View Source Code
      </a>
      <a href="https://leochen21.github.io/sitemap/" class="hero-link">
        🗺️ Explore Site Map
      </a>
    </div>
  </div>
</div>

<div class="content-section">
  <h2 class="section-title">🚀 About My Journey</h2>
  <p class="intro-text">
    This website serves as a comprehensive presentation of my journey through software engineering, 
    showcasing projects that span computer vision, web development, AI/ML applications, and full-stack solutions. 
    Each project represents a step forward in my continuous learning and passion for innovative technology.
  </p>
</div>

<div class="highlights-grid">
  <div class="highlight-card">
    <div class="highlight-icon">💻</div>
    <h3 class="highlight-title">Software Engineering</h3>
    <p class="highlight-desc">Full-stack development with modern frameworks and technologies</p>
  </div>
  
  <div class="highlight-card">
    <div class="highlight-icon">👁️</div>
    <h3 class="highlight-title">Computer Vision</h3>
    <p class="highlight-desc">Machine learning projects focused on image and video processing</p>
  </div>
  
  <div class="highlight-card">
    <div class="highlight-icon">🤖</div>
    <h3 class="highlight-title">AI & Machine Learning</h3>
    <p class="highlight-desc">Innovative applications of artificial intelligence and deep learning</p>
  </div>
  
  <div class="highlight-card">
    <div class="highlight-icon">📊</div>
    <h3 class="highlight-title">Research & Publications</h3>
    <p class="highlight-desc">Contributing to academic research in computer vision competitions</p>
  </div>
</div>

<div class="cta-section">
  <h2 class="cta-title">🌟 Let's Connect & Collaborate</h2>
  <p class="cta-text">
    Interested in my work? Let's discuss opportunities, share ideas, or collaborate on exciting projects!
  </p>
  <div class="cta-buttons">
    <a href="/portfolio/" class="cta-button">
      💼 View My Portfolio
    </a>
    <a href="/publications/" class="cta-button">
      📚 Read My Publications
    </a>
    <a href="/cv/" class="cta-button">
      📄 Download Resume
    </a>
  </div>
</div>

