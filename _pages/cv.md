---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<style>
.cv-hero {
  background: linear-gradient(135deg, #495057 0%, #6c757d 100%);
  color: white;
  padding: 3rem 2rem;
  margin: -2rem -2rem 3rem -2rem;
  text-align: center;
  border-radius: 0 0 20px 20px;
  position: relative;
  overflow: hidden;
}

.cv-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="documents" width="50" height="50" patternUnits="userSpaceOnUse"><text x="25" y="30" text-anchor="middle" fill="white" opacity="0.1" font-size="18">📄</text></pattern></defs><rect width="100" height="100" fill="url(%23documents)"/></svg>');
  opacity: 0.3;
}

.cv-hero-content {
  position: relative;
  z-index: 2;
}

.cv-hero h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  font-weight: 700;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

.cv-hero p {
  font-size: 1.2rem;
  opacity: 0.9;
  max-width: 600px;
  margin: 0 auto 2rem auto;
  line-height: 1.6;
}

.cv-actions {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 1.5rem;
}

.cv-action-btn {
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

.cv-action-btn:hover {
  background: rgba(255,255,255,0.3);
  transform: translateY(-2px);
  text-decoration: none;
  color: white !important;
}

.cv-action-btn.primary {
  background: #007bff;
  border: 1px solid #007bff;
}

.cv-action-btn.primary:hover {
  background: #0056b3;
  border: 1px solid #0056b3;
}

.cv-container {
  background: #fff;
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  margin: 2rem 0;
  overflow: hidden;
  border: 1px solid #e1e8ed;
}

.cv-header {
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  padding: 1.5rem 2rem;
  border-bottom: 1px solid #e1e8ed;
  text-align: center;
}

.cv-header h2 {
  font-size: 1.4rem;
  font-weight: 600;
  color: #2c3e50;
  margin: 0 0 0.5rem 0;
}

.cv-header p {
  color: #666;
  margin: 0;
  font-size: 0.95rem;
}

.cv-content {
  padding: 0;
  position: relative;
}

.pdf-viewer {
  width: 100%;
  height: 1200px;
  border: none;
  display: block;
}

.pdf-fallback {
  padding: 3rem 2rem;
  text-align: center;
  background: #f8f9fa;
  color: #666;
}

.pdf-fallback h3 {
  color: #2c3e50;
  margin-bottom: 1rem;
}

.pdf-fallback p {
  margin-bottom: 1.5rem;
  line-height: 1.6;
}

.download-btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.75rem 1.5rem;
  background: #28a745;
  color: white !important;
  text-decoration: none;
  border-radius: 25px;
  font-weight: 500;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(40, 167, 69, 0.3);
}

.download-btn:hover {
  background: #218838;
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(40, 167, 69, 0.4);
  text-decoration: none;
  color: white !important;
}

.cv-stats {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
  margin: 2rem 0;
}

.stat-card {
  background: #fff;
  padding: 1.5rem;
  border-radius: 10px;
  text-align: center;
  border: 1px solid #e1e8ed;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
}

.stat-card .stat-icon {
  font-size: 2rem;
  margin-bottom: 0.5rem;
}

.stat-card .stat-title {
  font-size: 0.9rem;
  color: #666;
  margin-bottom: 0.25rem;
}

.stat-card .stat-value {
  font-size: 1.2rem;
  font-weight: 600;
  color: #2c3e50;
}

.note-section {
  background: #e7f3ff;
  border-left: 4px solid #007bff;
  padding: 1rem 1.5rem;
  border-radius: 5px;
  margin: 2rem 0;
}

.note-section p {
  color: #004085;
  margin: 0;
  font-size: 0.95rem;
  line-height: 1.5;
}

@media (max-width: 768px) {
  .cv-hero {
    margin: -1rem -1rem 2rem -1rem;
    padding: 2rem 1rem;
  }
  
  .cv-hero h1 {
    font-size: 2rem;
  }
  
  .cv-actions {
    flex-direction: column;
    align-items: center;
  }
  
  .cv-stats {
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  }
  
  .pdf-viewer {
    height: 800px;
  }
}

@media print {
  .cv-hero,
  .cv-actions,
  .cv-stats,
  .note-section {
    display: none;
  }
  
  .cv-container {
    box-shadow: none;
    border: none;
  }
}
</style>

{% include base_path %}

<div class="cv-hero">
  <div class="cv-hero-content">
    <h1>📄 Curriculum Vitae</h1>
    <p>
      Comprehensive overview of my academic background, professional experience, technical skills, and research contributions in computer science and software engineering.
    </p>
    
    <div class="cv-actions">
      <a href="{{ base_path }}/files/Leo%20Chen%20Resume.pdf" download class="cv-action-btn primary">
        ⬇️ Download PDF
      </a>
      <a href="{{ base_path }}/files/Leo%20Chen%20Resume.pdf" target="_blank" class="cv-action-btn">
        🔗 Open in New Tab
      </a>
      <a href="javascript:window.print()" class="cv-action-btn">
        🖨️ Print Resume
      </a>
    </div>
  </div>
</div>

<div class="cv-stats">
  <div class="stat-card">
    <div class="stat-icon">🎓</div>
    <div class="stat-title">Education</div>
    <div class="stat-value">Computer Science</div>
  </div>
  <div class="stat-card">
    <div class="stat-icon">💻</div>
    <div class="stat-title">Experience</div>
    <div class="stat-value">Software Engineering</div>
  </div>
  <div class="stat-card">
    <div class="stat-icon">🔬</div>
    <div class="stat-title">Research</div>
    <div class="stat-value">Computer Vision</div>
  </div>
  <div class="stat-card">
    <div class="stat-icon">🏆</div>
    <div class="stat-title">Projects</div>
    <div class="stat-value">6+ Completed</div>
  </div>
</div>

<div class="cv-container">
  <div class="cv-header">
    <h2>Leo Chen - Resume</h2>
    <p>Computer Science Student & Software Engineer | Updated {{site.time | date: "%B %Y"}}</p>
  </div>
  
  <div class="cv-content">
    <iframe 
      src="{{ base_path }}/files/Leo%20Chen%20Resume.pdf" 
      class="pdf-viewer"
      title="Leo Chen Resume PDF">
    </iframe>
    
    <div class="pdf-fallback" style="display: none;">
      <h3>📄 Resume Not Displaying?</h3>
      <p>Your browser may not support embedded PDFs. Please download the resume directly or open it in a new tab.</p>
      <a href="{{ base_path }}/files/Leo%20Chen%20Resume.pdf" download class="download-btn">
        ⬇️ Download Resume PDF
      </a>
    </div>
  </div>
</div>

<div class="note-section">
  <p><strong>💡 Note:</strong> This resume is regularly updated to reflect my latest experience, skills, and accomplishments. For the most current version, please download the PDF above. For specific inquiries about my background or availability, feel free to contact me through the provided channels.</p>
</div>

<script>
// Fallback for browsers that don't support PDF embedding
document.addEventListener('DOMContentLoaded', function() {
  const iframe = document.querySelector('.pdf-viewer');
  const fallback = document.querySelector('.pdf-fallback');
  
  iframe.addEventListener('error', function() {
    iframe.style.display = 'none';
    fallback.style.display = 'block';
  });
  
  // Check if PDF loaded successfully after a delay
  setTimeout(function() {
    try {
      if (iframe.contentDocument === null) {
        iframe.style.display = 'none';
        fallback.style.display = 'block';
      }
    } catch (e) {
      // Cross-origin access blocked - PDF likely loaded successfully
    }
  }, 3000);
});
</script>
