---
layout: single
title: "Hi, I'm Harsh"
author_profile: true
---

<style>
body { padding-top: 72px; }
.top-nav {
  display: flex; gap: 18px; align-items: center; position: fixed; top: 0; left: 0; width: 100%; background: #fff; z-index: 9; box-shadow: 0 2px 8px rgba(0,0,0,0.025);
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
}
.nav-links a {
  text-decoration: none;
  color: #007acc;
  padding: 6px 12px;
  border-radius: 6px;
  transition: 0.25s;
  white-space: nowrap;
}
.nav-links a:hover {
  background: #007acc;
  color: #fff;
}
.animated-heading { font-size: 28px; font-weight: bold; color: #007acc; animation: fadeInSlideUp 1.2s ease-out forwards; text-align: center; margin-bottom: 20px; }
.services-container { max-width: 960px; margin: 60px auto; padding: 20px; border-radius: 15px; background: #f9f9f9; box-shadow: 0 4px 12px rgba(0,0,0,0.06); }
.services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px,1fr)); gap: 18px; align-items: start; }
.service-card { background: #fff; padding: 18px; border-radius: 12px; box-shadow: 0 6px 18px rgba(2,6,23,0.04); text-align: center; display:flex; flex-direction: column; gap: 12px; align-items: center; }
.service-icon { width: 64px; height: 64px; border-radius: 12px; display:flex; align-items:center; justify-content:center; background: linear-gradient(135deg,#e6f7fb,#dff8f9); box-shadow: inset 0 -4px 8px rgba(0,0,0,0.03);}
.service-icon svg { width:36px; height:36px; fill: #007acc; }
.service-title { color:#007acc; font-weight:700; font-size:1rem; }
.service-desc { color:#444; font-size:0.95rem; }
.contact-form-container{ max-width:500px; margin:20px auto; background:#f9f9f9; padding:20px; border-radius:10px; box-shadow:0 4px 10px rgba(0,0,0,0.08);}
.contact-form-container label{ display:block; margin-bottom:8px; font-weight:600; color:#222; }
.contact-form-container input, .contact-form-container textarea { width:100%; padding:10px; border-radius:6px; border:1px solid #ddd; margin-bottom:12px; font-size:0.95rem; box-sizing:border-box; }
.contact-form-container button { background:#007acc;color:white;padding:10px 14px;border:none;border-radius:6px;cursor:pointer;font-weight:700;}
.form-note{ font-size:0.9rem; color:#555; margin-top:10px; text-align:center; }
@media (max-width:880px){
  body { padding-top:84px; }
  #navToggle{ display:block; }
  .nav-links{
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
  .nav-links.open{ display:flex; }
  .nav-links a{ padding: 10px; display:block; }
}
</style>

<div class="top-nav" role="navigation" aria-label="Main navigation">
  <button id="navToggle" aria-expanded="false" aria-controls="navLinks">☰</button>
  <div id="navLinks" class="nav-links">
    <a href="#services" class="top-nav-link">Services</a>
    <a href="#my-work" class="top-nav-link">My Work</a>
    <a href="#certificates" class="top-nav-link">Certificates</a>
    <a href="#contact" class="top-nav-link">Contact</a>
  </div>
</div>

<h2 class="animated-heading">📢 Data Tells The Truth</h2>

<div style="max-width: 200px; margin: 30px auto 10px auto; border-radius: 50%; overflow: hidden; box-shadow: 0 0 15px #007accbb;">
  <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" alt="Harsh Profile Photo" style="width: 100%; display: block;" />
</div>

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

<div id="services" class="services-container">
  <h2 style="color:#007acc; font-weight:bold; margin-bottom:18px; text-align:center;">
    <img src="https://raw.github.com/harsh-bca/portfolio-assets/blob/main/Data%20analytics%20logo.jpg" alt="Services logo" style="height:28px; vertical-align:middle; margin-right:8px;">
    💼 My Services
  </h2>
  <div class="services-grid">
    <!-- Dashboard -->
    <div class="service-card">
      <div class="service-icon"><svg viewBox="0 0 24 24"><path d="M3 13h3v7H3v-7zm5-6h3v13H8V7zm5 4h3v9h-3v-9zm5-8h3v17h-3V3z"/></svg></div>
      <div class="service-title">Dashboard Creation</div>
      <div class="service-desc">Interactive Power BI / Tableau dashboards with clear KPIs.</div>
    </div>
    <!-- Automation -->
    <div class="service-card">
      <div class="service-icon"><svg viewBox="0 0 24 24"><path d="M13 2L3 14h7l-1 8L21 10h-7l-1-8z"/></svg></div>
      <div class="service-title">Automation</div>
      <div class="service-desc">Scripts & jobs to save reporting time and reduce manual steps.</div>
    </div>
    <!-- Data Pipeline -->
    <div class="service-card">
      <div class="service-icon"><svg viewBox="0 0 24 24"><path d="M3 6h6v2H3V6zm0 5h10v2H3v-2zm0 5h14v2H3v-2z"/></svg></div>
      <div class="service-title">Data Pipeline Building</div>
      <div class="service-desc">ETL, scheduling and clean data flows for reliable reporting.</div>
    </div>
    <!-- Insights -->
    <div class="service-card">
      <div class="service-icon"><svg viewBox="0 0 24 24"><path d="M9 21h6v-1H9v1zm3-19C8.48 2 5 5.48 5 9.5c0 2.54 1.69 4.74 4 5.43V17h6v-2.07c2.31-.69 4-2.9 4-5.43C19 5.48 15.52 2 12 2z"/></svg></div>
      <div class="service-title">Insights Generation</div>
      <div class="service-desc">Actionable recommendations with clear business metrics.</div>
    </div>
  </div>
</div>

## 💼 Featured Projects <a id="my-work"></a>
... <!-- rest of your markdown content for projects, certificates, contact; no structure changes needed as they're already valid markdown/HTML mix -->

<script>
  document.addEventListener('DOMContentLoaded', function () {
    // Nav toggle (mobile)
    const navToggle = document.getElementById('navToggle');
    const navLinks = document.getElementById('navLinks');
    if (navToggle && navLinks) {
      navToggle.addEventListener('click', () => {
        const isOpen = navLinks.classList.toggle('open');
        navToggle.setAttribute('aria-expanded', isOpen ? 'true' : 'false');
      });
    }
    const themeToggle = document.getElementById('themeToggle');
    if (themeToggle) {
      if (localStorage.getItem('theme') === 'light') {
        document.body.classList.add('light-mode');
      }
      themeToggle.addEventListener('click', () => {
        document.body.classList.toggle('light-mode');
        if (document.body.classList.contains('light-mode')) localStorage.setItem('theme', 'light');
        else localStorage.removeItem('theme');
      });
    }
  });
</script>
