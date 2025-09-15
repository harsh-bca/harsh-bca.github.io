<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Harsh Tripathi | Data Analyst Portfolio</title>
  <style>
    /* === Global Styles === */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      background: #0f2027;
      color: #fff;
      line-height: 1.6;
    }
    a {
      text-decoration: none;
      color: inherit;
    }
    h1, h2, h3 {
      margin-bottom: 10px;
    }
/* === Navbar === */
    nav {
      width: 100%;
      background: #1b2735;
      padding: 15px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: fixed;
      top: 0;
      z-index: 1000;
    }
    nav .logo {
      font-size: 20px;
      font-weight: bold;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 20px;
    }
    nav ul li a {
      color: #fff;
      transition: 0.3s;
    }
    nav ul li a:hover {
      color: #00adb5;
    }
/* === Hero Section === */
    .hero {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 100px 50px;
      min-height: 100vh;
    }
    .hero-text {
      max-width: 600px;
    }
    .hero-text h1 {
      font-size: 36px;
    }
    .hero-text h2 {
      font-size: 28px;
      color: #00adb5;
      height: 40px;
      overflow: hidden;
    }
    .hero-text p {
      margin: 20px 0;
      font-size: 16px;
      color: #ddd;
    }
    .social-links {
      margin: 20px 0;
    }
    .social-links a {
      margin-right: 15px;
      font-size: 18px;
    }
    .resume-btn {
      display: inline-block;
      padding: 10px 20px;
      background: #00adb5;
      border-radius: 5px;
      margin-top: 15px;
    }
/* Profile Image */
    .profile-pic {
      width: 250px;
      height: 250px;
      border-radius: 50%;
      border: 5px solid #00adb5;
      box-shadow: 0 0 30px #00adb5;
      object-fit: cover;
    }
/* === Section Layouts === */
    section {
      padding: 80px 50px;
      text-align: center;
    }
    section h2 {
      margin-bottom: 40px;
      font-size: 28px;
      color: #00adb5;
    }
/* === Services Section === */
    .services {
      display: flex;
      justify-content: center;
      gap: 30px;
      flex-wrap: wrap;
    }
    .service-card {
      background: #1b2735;
      padding: 20px;
      width: 250px;
      border-radius: 10px;
      box-shadow: 0 0 10px #000;
    }
/* === Skills Section === */
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 20px;
      max-width: 800px;
      margin: auto;
    }
    .skill-item {
      background: #1b2735;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 0 10px #000;
    }
/* === Projects Section === */
    .projects {
      display: flex;
      gap: 30px;
      flex-wrap: wrap;
      justify-content: center;
    }
    .project-card {
      background: #1b2735;
      padding: 20px;
      width: 280px;
      border-radius: 10px;
    }
/* === Contact Section === */
    .contact {
      max-width: 600px;
      margin: auto;
    }
    .contact a {
      display: block;
      margin: 10px 0;
      color: #00adb5;
    }
  </style>
</head>
<body>
  <!-- === Navbar === -->
  <nav>
    <div class="logo">Harsh | Data Analyst</div>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><a href="https://github.com/harsh-bca/portfolio-assets/blob/main/Harsh_Tripathi_Data_Analyst_Resume.pdf" target="_blank">Resume</a></li>
    </ul>
  </nav>

  <!-- === Hero Section === -->
  <section class="hero" id="home">
    <div class="hero-text">
      <h1>Hi, I’m Harsh</h1>
      <h2>I am a <span id="role"></span></h2>
      <p>
        I see data not just as a record of the past, but as the blueprint for the future. 
        By applying AI and machine learning, I make that blueprint interactive. 
        I turn raw numbers into predictive insights and strategic action, 
        revealing the 'why' behind the 'what' to automate solutions and drive intelligent growth.
      </p>
      <div class="social-links">
        <a href="https://linkedin.com/in/harsh-tripathi-64376333a">LinkedIn</a>
        <a href="https://github.com/harsh-bca">GitHub</a>
        <a href="https://instagram.com/harsh._diaries">Instagram</a>
      </div>
      <a href="https://github.com/harsh-bca/portfolio-assets/blob/main/Harsh_Tripathi_Data_Analyst_Resume.pdf" class="resume-btn" target="_blank">📄 Download Resume</a>
    </div>
    <div>
      <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" alt="Harsh Tripathi" class="profile-pic" />
    </div>
  </section>

  <!-- === Services Section === -->
  <section id="services">
    <h2>My Services</h2>
    <div class="services">
      <div class="service-card">📊 Dashboard Creation</div>
      <div class="service-card">⚡ Automated Reporting</div>
      <div class="service-card">📈 Data Analysis & Insights</div>
    </div>
  </section>

  <!-- === Skills Section === -->
  <section id="skills">
    <h2>Skills</h2>
    <div class="skills-grid">
      <div class="skill-item">🐍 Python</div>
      <div class="skill-item">🗄️ SQL</div>
      <div class="skill-item">📊 Power BI</div>
      <div class="skill-item">📊 Tableau</div>
      <div class="skill-item">📈 Excel</div>
      <div class="skill-item">☁️ Azure</div>
    </div>
  </section>

  <!-- === Projects Section === -->
  <section id="projects">
    <h2>Projects</h2>
    <div class="projects">
      <div class="project-card">
        <h3>Fee Dashboard</h3>
        <p>Built an interactive dashboard in Looker Studio for college fee tracking and automated reminders.</p>
        <a href="#">🔗 View Project</a>
      </div>
      <div class="project-card">
        <h3>Youth Trends Analysis</h3>
        <p>Analyzed NFHS & survey data to identify behavioral trends among youth for policy insights.</p>
        <a href="#">🔗 View Project</a>
      </div>
    </div>
  </section>

  <!-- === Contact Section === -->
  <section id="contact">
    <h2>Contact Me</h2>
    <div class="contact">
      <a href="mailto:harsh.tripati21@gmail.com">📧 harsh.tripati21@gmail.com</a>
      <a href="https://linkedin.com/in/harsh-tripathi-64376333a">🔗 LinkedIn</a>
      <a href="https://instagram.com/harsh._diaries">📷 Instagram</a>
    </div>
  </section>

  <!-- === Animated Role Text === -->
  <script>
    const roles = ["Data Analyst", "Automation Specialist"];
    let roleIndex = 0;
    let charIndex = 0;
    const roleElement = document.getElementById("role");

    function typeRole() {
      if (charIndex < roles[roleIndex].length) {
        roleElement.textContent += roles[roleIndex].charAt(charIndex);
        charIndex++;
        setTimeout(typeRole, 150);
      } else {
        setTimeout(eraseRole, 2000);
      }
    }

    function eraseRole() {
      if (charIndex > 0) {
        roleElement.textContent = roles[roleIndex].substring(0, charIndex - 1);
        charIndex--;
        setTimeout(eraseRole, 100);
      } else {
        roleIndex = (roleIndex + 1) % roles.length;
        setTimeout(typeRole, 200);
      }
    }

    document.addEventListener("DOMContentLoaded", typeRole);
  </script>
</body>
</html>
