---
layout: single
author_profile: true
---

<style>
html {
  scroll-behavior: smooth;
}
body {
  padding-top: 72px;
  font-family: Arial, sans-serif;
  margin: 0;
  background: #fff;
  color: #333;
}
.top-nav {
  display: flex;
  gap: 18px;
  align-items: center;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background: #fff;
  z-index: 100;
  box-shadow: 0 2px 8px rgba(0,0,0,0.025);
  padding: 8px 16px;
  box-sizing: border-box;
}
#navToggle {
  display: none;
  background: transparent;
  border: none;
  font-size: 22px;
  color: #007acc;
  cursor: pointer;
  padding: 6px;
  border-radius: 6px;
}
.nav-links {
  display: flex;
  gap: 18px;
  align-items: center;
  flex-wrap: wrap;
}
.nav-links a {
  text-decoration: none;
  color: #007acc;
  padding: 6px 12px;
  border-radius: 6px;
  transition: 0.25s;
  white-space: nowrap;
  font-weight: 600;
}
.nav-links a:hover,
.nav-links a:focus {
  background: #007acc;
  color: #fff;
  outline: none;
}
.animated-intro {
  text-align: center;
  margin: 24px auto 40px auto;
  max-width: 800px;
}
#intro-name {
  font-size: 32px;
  font-weight: bold;
  color: #007acc;
  opacity: 0;
  animation: fadeIn 1.5s forwards;
  animation-delay: 0.3s;
  margin-bottom: 10px;
}
.animated-roles {
  font-size: 24px;
  font-weight: 600;
  color: #007acc;
  height: 30px;
  position: relative;
  overflow: hidden;
  min-height: 38px;
}
.role {
  position: absolute;
  width: 100%;
  opacity: 0;
  animation-fill-mode: forwards;
  animation-name: fadeInUp;
  animation-duration: 1s;
}
.role:nth-child(1) { animation-delay: 2s; }
.role:nth-child(2) { animation-delay: 4s; }
.role:nth-child(3) { animation-delay: 6s; }
@keyframes fadeIn { to { opacity: 1; } }
@keyframes fadeInUp {
  0% { opacity: 0; transform: translateY(20px); }
  100% { opacity: 1; transform: translateY(0); }
}
.animated-heading {
  font-size: 28px;
  font-weight: bold;
  color: #007acc;
  opacity: 0;
  animation: fadeInSlideUp 1.2s ease-out forwards;
  animation-delay: 0.5s;
  text-align: center;
  margin-bottom: 20px;
  max-width: 960px;
  margin-left: auto;
  margin-right: auto;
}
@keyframes fadeInSlideUp {
  0% {
    opacity: 0;
    transform: translateY(15px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
.services-container {
  max-width: 960px;
  margin: 40px auto 80px auto;
  padding: 20px;
  border-radius: 15px;
  background: #f9f9f9;
  box-shadow: 0 4px 12px rgba(0,0,0,0.06);
}
.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px,1fr));
  gap: 18px;
  align-items: start;
}
.service-card {
  background: #fff;
  padding: 18px;
  border-radius: 12px;
  box-shadow: 0 6px 18px rgba(2,6,23,0.04);
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 12px;
  align-items: center;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.service-card:hover {
  transform: scale(1.05);
  box-shadow: 0 12px 24px rgba(2,6,23,0.12);
  cursor: pointer;
}
.service-icon {
  width: 64px;
  height: 64px;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg,#e6f7fb,#dff8f9);
  box-shadow: inset 0 -4px 8px rgba(0,0,0,0.03);
}
.service-icon svg {
  width: 36px;
  height: 36px;
  fill: #007acc;
}
.service-title {
  color: #007acc;
  font-weight: 700;
  font-size: 1rem;
}
.service-desc {
  color: #444;
  font-size: 0.95rem;
}
.contact-form-container {
  max-width: 500px;
  margin: 20px auto 60px auto;
  background: #f9f9f9;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.08);
}
.contact-form-container label {
  display: block;
  margin-bottom: 8px;
  font-weight: 600;
  color: #222;
}
.contact-form-container input,
.contact-form-container textarea {
  width: 100%;
  padding: 10px;
  border-radius: 6px;
  border: 1px solid #ddd;
  margin-bottom: 12px;
  font-size: 0.95rem;
  box-sizing: border-box;
}
.contact-form-container button {
  background: #007acc;
  color: white;
  padding: 10px 14px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-weight: 700;
}
.form-note {
  font-size: 0.9rem;
  color: #555;
  margin-top: 10px;
  text-align: center;
}
@media (max-width: 880px) {
  body { padding-top: 84px; }
  #navToggle { display: block; }
  .nav-links {
    position: absolute;
    top: 56px;
    right: 12px;
    flex-direction: column;
    background: #fff;
    padding: 10px;
    border-radius: 10px;
    box-shadow: 0 12px 36px rgba(2,6,23,0.12);
    display: none;
    min-width: 170px;
  }
  .nav-links.open { display: flex; }
  .nav-links a { padding: 10px; display: block; }
}
</style>
<!-- Navigation -->
<div class="top-nav" role="navigation" aria-label="Main navigation">
  <button id="navToggle" aria-expanded="false" aria-controls="navLinks">☰</button>
  <div id="navLinks" class="nav-links">
    <a href="#" class="top-nav-link">Home</a>
    <a href="#services" class="top-nav-link">Services</a>
    <a href="#my-work" class="top-nav-link">My Work</a>
    <a href="#certificates" class="top-nav-link">Certificates</a>
    <a href="#contact" class="top-nav-link">Contact</a>
  </div>
</div>
<!-- Animated Intro Section -->
<div class="animated-intro">
  <h1 id="intro-name">Hi, I'm Harsh</h1>
  <div class="animated-roles">
    <span class="role">Data Analyst</span>
    <span class="role">Automation Specialist</span>
    <span class="role">Process Optimizer</span>
  </div>
</div>
<h2 class="animated-heading">📢 Data Tells The Truth</h2>
<!-- Profile Photo -->
<div style="max-width: 200px; margin: 30px auto 10px auto; border-radius: 50%; overflow: hidden; box-shadow: 0 0 15px #007accbb;">
  <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" alt="Harsh Profile Photo" style="width: 100%; display: block;" />
</div>
<!-- Intro Video -->
<div id="intro-video" class="intro-container" style="max-width: 800px; margin: 0 auto; padding: 20px; border-radius: 15px; background: #f9f9f9; box-shadow: 0px 4px 12px rgba(0,0,0,0.1); text-align: center;">
  <h2 style="color:#007acc; font-weight: bold; margin-bottom: 15px;">
    🌟 Intro Video – Why I’m Your Next Best Employee
  </h2>
  <p style="font-size: 16px; color:#333; margin-bottom: 20px;">
    Sometimes a CV doesn’t tell the whole story. Here’s a short video where I introduce myself, my journey, 
    and why I bring confidence, creativity, and data-driven problem solving to the table.
  </p>
  <iframe src="https://drive.google.com/file/d/1nYuJfaCucRcubVW8LNzWMyibpHnZTDif/preview" width="100%" height="420" style="border-radius: 12px; border: none;"></iframe>
</div>
<!-- Services -->
<div id="services" class="services-container">
  <h2 style="color:#007acc; font-weight:bold; margin-bottom:18px; text-align:center;">
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/Data%20analytics%20logo.jpg" alt="Services logo" style="height:28px; vertical-align:middle; margin-right:8px;">
    💼 My Services
  </h2>
  <div class="services-grid">
    <div class="service-card">
      <div class="service-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="M3 13h3v7H3v-7zm5-6h3v13H8V7zm5 4h3v9h-3v-9zm5-8h3v17h-3V3z"/></svg>
      </div>
      <div class="service-title">Dashboard Creation</div>
      <div class="service-desc">Interactive Power BI / Tableau dashboards with clear KPIs.</div>
    </div>
    <div class="service-card">
      <div class="service-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="M13 2L3 14h7l-1 8L21 10h-7l-1-8z"/></svg>
      </div>
      <div class="service-title">Automation</div>
      <div class="service-desc">Scripts & jobs to save reporting time and reduce manual steps.</div>
    </div>
    <div class="service-card">
      <div class="service-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="M3 6h6v2H3V6zm0 5h10v2H3v-2zm0 5h14v2H3v-2z"/></svg>
      </div>
      <div class="service-title">Data Pipeline Building</div>
      <div class="service-desc">ETL, scheduling and clean data flows for reliable reporting.</div>
    </div>
    <div class="service-card">
      <div class="service-icon" aria-hidden="true">
        <svg viewBox="0 0 24 24"><path d="M9 21h6v-1H9v1zm3-19C8.48 2 5 5.48 5 9.5c0 2.54 1.69 4.74 4 5.43V17h6v-2.07c2.31-.69 4-2.9 4-5.43C19 5.48 15.52 2 12 2z"/></svg>
      </div>
      <div class="service-title">Insights Generation</div>
      <div class="service-desc">Actionable recommendations with clear business metrics.</div>
    </div>
  </div>
</div>
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
   <div style="border:1px solid #ddd; padding:15px; border-radius:10px;">
    <img src="https://raw.github.com/harsh-bca/College-Fee-Dashboard/main/Fee%20compliance%20dashboard.png" alt="Fee Dashboard Banner" style="width:100%; border-radius: 10px; margin-bottom: 10px;" />
    <h3><a href="https://github.com/harsh-bca/College-Fee-Dashboard"> Fee Compliance Dashboard</a></h3>
    <p>A private college was facing problems in manual student fee tracking in Excel, leading to time-consuming and burnout to the faculty, So developed two interactive dashboards with Google Data Studio, cleaned the dataset with Excel, and automated them with Python to reduce the manual work and boost overall process effiency </p>
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
    <img src="https://github.com/harsh-bca/portfolio-assets/blob/main/Quantium%20data%20analysis%20certificate_page-0001.jpg?raw=true" alt="Data Analytics Certification" style="width: 100%; border-radius: 10px;" />
    <p align="center"><strong>Data Analytics Job Simulation</strong><br>Quantum Data Analytics Certificate</p>
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
 <svg xmlns="http://www.w3.org/2000/svg" style="vertical-align: middle; height:16px; width:16px; fill:#007acc; margin-right:6px;" viewBox="0 0 24 24"><path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zM4 8.99l7.06 4.42c.41.26.94.26 1.35 0L20 8.99V6l-8 5-8-5v2.99z"/></svg> <a href="mailto:harsh.tripati21@gmail.com">harsh.tripati21@gmail.com</a>
 <svg xmlns="http://www.w3.org/2000/svg" style="vertical-align: middle; height:16px; width:16px; fill:#007acc; margin-right:6px;" viewBox="0 0 24 24"><path d="M12 2.04c5.5 0 9.96 4.46 9.96 9.96S17.5 21.96 12 21.96 2.04 17.5 2.04 12 6.5 2.04 12 2.04zm3 10.49c-.26-.16-1.53-.76-1.77-.85-.24-.09-.42-.13-.6.13-.19.26-.73.85-.9 1.02-.17.17-.34.19-.6.06-.26-.13-1.11-.41-2.11-1.3-.78-.69-1.3-1.54-1.46-1.8-.16-.26-.02-.4.12-.53.12-.12.26-.33.39-.5.13-.17.17-.26.26-.43.09-.17.04-.31-.02-.43-.06-.13-.6-1.45-.82-1.98-.22-.52-.44-.45-.6-.46-.15-.02-.32-.02-.49-.02s-.43.06-.65.31c-.22.26-.84.82-.84 2 0 1.18.86 2.33.98 2.5.12.17 1.7 2.6 4.12 3.64.58.24 1.03.39 1.38.5.58.18 1.11.15 1.53.09.47-.07 1.53-.62 1.74-1.22.22-.61.22-1.13.15-1.22-.07-.09-.24-.16-.5-.31z"/></svg> <a href="https://www.linkedin.com/in/harsh-tripathi-64376333a/" target="_blank" rel="noopener noreferrer">LinkedIn</a>
 <svg xmlns="http://www.w3.org/2000/svg" style="vertical-align: middle; height:16px; width:16px; fill:#007acc; margin-right:6px;" viewBox="0 0 24 24"><path d="M7.75 2h8.5C18.77 2 19 2.23 19 2.5V5c0 .28-.23.5-.5.5H17a4.5 4.5 0 0 1-9 0h-1.5a.5.5 0 0 1-.5-.5V2.5c0-.27.23-.5.5-.5zM12 7a3 3 0 1 0 0 6 3 3 0 0 0 0-6zm-7 8.25C5 17.55 5.45 18 6 18h12c.55 0 1-.45 1-1.25V14H5v1.25z"/></svg> <a href="https://www.instagram.com/harshanalyst2025?igsh=aTNyN2d4eXl1aTg=" target="_blank" rel="noopener noreferrer">Instagram</a>
<div class="contact-form-container">
  <form id="contactForm" action="https://formspree.io/f/YOUR_FORMSPREE_ID" method="POST" autocomplete="on">
    <label for="name">Name:</label>
    <input id="name" name="name" type="text" autocomplete="name" required>
    <label for="email">Email:</label>
    <input id="email" name="email" type="email" autocomplete="email" required>
    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="5" autocomplete="on" required></textarea>
  <input type="hidden" name="_subject" value="New contact from portfolio">
    <button type="submit">Send</button>
  </form>
</div>
<script>
document.addEventListener('DOMContentLoaded',function(){
  const roles = document.querySelectorAll('.animated-roles .role');
  let idx=0;
  function showRole(i){
    roles.forEach((role,j)=>role.style.display = (i===j) ? 'inline' : 'none');
  }
  showRole(0); // Show first role
  setTimeout(()=>{ showRole(1); }, 2000); // Show second after 2s
  setTimeout(()=>{ showRole(2); }, 4000); // Show third after 4s
});
</script>
