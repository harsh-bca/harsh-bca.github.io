---
layout: single
title: "Hi, I'm Harsh"
author_profile: true
---
<style>
/* ===== Navigation Bar ===== */
.top-nav {
  position: fixed;
  top: 15px;
  right: 30px;
  display: flex;
  gap: 25px;
  font-size: 16px;
  font-weight: bold;
  z-index: 1000;
}
.top-nav a {
  text-decoration: none;
  color: #007acc;
  padding: 6px 12px;
  border-radius: 6px;
  transition: 0.3s ease;
}
.top-nav a:hover {
  background: #007acc;
  color: white;
}

/* ===== Fade Animation ===== */
@keyframes fadeInSlideUp {
  0% { opacity: 0; transform: translateY(30px); }
  100% { opacity: 1; transform: translateY(0); }
}
.animated-heading {
  font-size: 28px;
  font-weight: bold;
  color: #007acc;
  animation: fadeInSlideUp 1.2s ease-out forwards;
  text-align: center;
  margin-bottom: 20px;
}
</style>


<!-- Updated Navbar order -->
<div class="top-nav">
  <a href="#services" class="top-nav-link">Services</a>  <!-- Moved services first -->
  <a href="#my-work" class="top-nav-link">My Work</a>
  <a href="#certificates" class="top-nav-link">Certificates</a>
  <a href="#contact" class="top-nav-link">Contact</a>
</div>

<h2 class="animated-heading">📢 Data Tells The Truth</h2>

<!-- Profile Pic Above Intro Video -->
<div style="max-width: 200px; margin: 30px auto 10px auto; border-radius: 50%; overflow: hidden; box-shadow: 0 0 15px #007accbb;">
  <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" alt="Harsh Profile Photo" style="width: 100%; display: block;" />
</div>

<!-- Introduction Video Container -->
<div id="intro-video" class="intro-container" style="max-width: 800px; margin: 0 auto; padding: 20px; border-radius: 15px; background: #f9f9f9; box-shadow: 0px 4px 12px rgba(0,0,0,0.1); text-align: center;">
  <h2 style="color:#007acc; font-weight: bold; margin-bottom: 15px;">
    🌟 Intro Video – Why I’m Your Next Best Employee
  </h2>
  <p style="font-size: 16px; color:#333; margin-bottom: 20px;">
    Sometimes a CV doesn’t tell the whole story. Here’s a short video where I introduce myself, my journey, 
    and why I bring confidence, creativity, and data-driven problem solving to the table.
  </p>
  <iframe src="https://drive.google.com/file/d/1nYuJfaCucRcubVW8LNzWMyibpHnZTDif/preview" 
          width="100%" height="420" 
          style="border-radius: 12px; border: none;">
  </iframe>
</div>

<!-- Services Section -->
<div id="services" class="services-container" style="max-width: 800px; margin: 60px auto; padding: 20px; border-radius: 15px; background: #f9f9f9; box-shadow: 0px 4px 12px rgba(0,0,0,0.1);">
  <h2 style="color:#007acc; font-weight: bold; margin-bottom: 30px; text-align: center;">💼 My Services</h2>
  <ul style="list-style:none; padding:0; font-size: 18px; color:#222; max-width: 400px; margin: 0 auto;">
    <li>📊 Dashboard Creation</li>
    <li>⚡ Automation</li>
    <li>🔧 Data Pipeline Building</li>
    <li>💡 Insights Generation</li>
  </ul>
</div>

---
## 💼 Featured Projects <a id="my-work"></a>
<div style="display: flex; flex-direction: column; gap: 20px;">
  <div style="border:1px solid #ddd; padding:15px; border-radius:10px;">
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/Youth%20trends%20analysis%20banner.png" alt="Youth Trends Analysis Banner" style="width:100%; border-radius: 10px; margin-bottom: 10px;" />
    <h3><a href="https://github.com/harsh-bca/youth-trends-analysis">📈 Youth Trends Analysis</a></h3>
    <p>Analyzed behavioral patterns, technology usage, and mental health trends among Indian youth using survey data. Utilized Python and Power BI to turn raw responses into actionable insights.</p>
  </div>
  <div style="border:1px solid #ddd; padding:15px; border-radius:10px;">
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/EDA%20project%20banner.png" alt="EDA Project Banner" style="width:100%; border-radius: 10px; margin-bottom: 10px;" />
    <h3><a href="https://github.com/harsh-bca/EDA-Project">📈 EDA Project</a></h3>
    <p>Performed Exploratory Data Analysis on global job market data to uncover hiring trends and skill demand. Used Python for EDA and Matplotlib/Seaborn for visualization.</p>
  </div>
  <div style="border:1px solid #ddd; padding:15px; border-radius:10px;">
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/NFHS%20data%20analysis%20banner.png" alt="NFHS Project Banner" style="width:100%; border-radius: 10px; margin-bottom: 10px;" />
    <h3><a href="https://github.com/harsh-bca/National-Family-Health-Survey-Analysis">📊 NFHS Health Survey</a></h3>
    <p>Explored Indian public health trends using NFHS data. Processed large-scale health and demographic data in Python and visualized findings with Power BI dashboards.</p>
  </div>
</div>

---
## 🧾 Certifications <a id="certificates"></a>
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 20px;">
  <div>
    <img src="https://github.com/harsh-bca/portfolio-assets/blob/main/google%20analytics%20certificate_page-0001.jpg?raw=true" alt="Google Analytics Certificate" style="width: 100%; border-radius: 10px;" />
    <p align="center"><strong>Google Analytics</strong><br>Google Skill Shop</p>
  </div>
  <div>
    <img src="https://github.com/harsh-bca/portfolio-assets/blob/main/CertificateOfCompletion_Career%20Essentials%20in%20Data%20Analysis%20by%20Microsoft%20and%20LinkedIn_page-0001.jpg?raw=true" alt="LinkedIn Career Essentials" style="width: 100%; border-radius: 10px;" />
    <p align="center"><strong>Career Essentials in Data Analysis</strong><br>Microsoft & LinkedIn</p>
  </div>
  <div>
    <img src="https://github.com/harsh-bca/portfolio-assets/blob/main/wadhwani%20foundation%20certificate%20_page-0001.jpg?raw=true" alt="Wadhwani Certificate" style="width: 100%; border-radius: 10px;" />
    <p align="center"><strong>Soft Skills</strong><br>Wadhwani Foundation</p>
  </div>
  <div>
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/grastech%20certificate.jpg" alt="Grastech Certificate" style="width: 100%; border-radius: 10px;" />
    <p align="center"><strong>Data Science & AI</strong><br>GRAStech</p>
  </div>
  <div>
    <img src="https://github.com/harsh-bca/portfolio-assets/blob/main/SQL%20certification%20_page-0001.jpg?raw=true" alt="SQL Certification" style="width: 100%; border-radius: 10px;" />
    <p align="center"><strong>SQL Certification</strong><br>Great Learning</p>
  </div>
  <div>
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/SAEIF%20CERTIFICATE.jpg" alt="SAEIF Certificate" style="width: 100%; border-radius: 10px;" />
    <p align="center"><strong>Personality Development</strong><br>SAEIF Foundation</p>
  </div>
</div>

---
## 📬 Contact <a id="contact"></a>
- 📧 [harsh.tripati21@gmail.com](mailto:harsh.tripati21@gmail.com)  
- 🌐 [LinkedIn](https://www.linkedin.com/in/harsh-tripathi-64376333a/)  
- 📷 [Instagram](https://www.instagram.com/harshanalyst2025?igsh=aTNyN2d4eXl1aTg=)  

<div class="contact-form-container" style="max-width:500px; margin:20px auto; background:#f9f9f9; padding:20px; border-radius:10px; box-shadow:0px 4px 10px rgba(0,0,0,0.1);">
  <form action="mailto:harsh.tripati21@gmail.com" method="post" enctype="text/plain">
    <label for="name">Name:</label><br>
    <input type="text" name="name" style="width:100%; margin-bottom:10px; padding:8px;"><br>
    
  <label for="email">Email:</label><br>
    <input type="email" name="email" style="width:100%; margin-bottom:10px; padding:8px;"><br>
    
  <label for="message">Message:</label><br>
    <textarea name="message" rows="4" style="width:100%; margin-bottom:10px; padding:8px;"></textarea><br>
    
  <button type="submit" style="background:#007acc; color:white; padding:10px 15px; border:none; border-radius:5px;">Send</button>
  </form>
</div>

<script>
  const themeToggle = document.getElementById('themeToggle');
  // Check localStorage for theme preference
  if(localStorage.getItem('theme') === 'light'){
    document.body.classList.add('light-mode');
  }

  themeToggle.addEventListener('click', () => {
    document.body.classList.toggle('light-mode');
    if(document.body.classList.contains('light-mode')){
      localStorage.setItem('theme', 'light');
    } else {
      localStorage.removeItem('theme');
    }
  });
</script>
