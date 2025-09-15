<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Harsh | Data Portfolio</title>
  <link href="https://fonts.googleapis.com/css?family=Montserrat:700,400&display=swap" rel="stylesheet">
  <style>
    body {
      background: #141b2d;
      color: #fff;
      font-family: 'Montserrat', Arial, sans-serif;
      margin: 0;
    }
    /* Navbar */
    .navbar {
      position: fixed;
      top: 0;
      width: 100%;
      background: #141b2d;
      color: #fff;
      z-index: 1000;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 26px 6vw 12px 6vw;
      box-sizing: border-box;
    }
    .nav-logo {
      font-weight: bold;
      font-size: 2.1rem;
      letter-spacing: 0.5px;
      color: #fff;
    }
    .nav-menu {
      display: flex;
      align-items: center;
      gap: 34px;
      font-size: 1.13rem;
    }
    .nav-menu a {
      color: #fff;
      text-decoration: none;
      transition: color 0.2s;
      padding: 4px 12px;
    }
    .nav-menu a:hover {
      color: #21c4fe;
    }
    .nav-contact-btn {
      font-weight: bold;
      background: #21c4fe;
      color: #fff;
      border: none;
      border-radius: 8px;
      padding: 10px 28px;
      margin-left: 18px;
      font-size: 1.16rem;
      text-decoration: none;
      box-shadow: 0 2px 8px #21c4fe30;
      cursor: pointer;
      transition: background 0.18s;
    }
    .nav-contact-btn:hover {
      background: #1693b3;
    }
    /* Content Wrapper */
    .main-content {
      padding-top: 95px;
      padding-left: 6vw;
      padding-right: 6vw;
      width: 100%;
      box-sizing: border-box;
      min-height: 100vh;
    }
    /* Hero */
    .hero-section {
      display: flex;
      flex-wrap: wrap;
      gap: 48px;
      margin-top: 18px;
      align-items: center;
      justify-content: space-between;
    }
    .hero-text {
      flex: 2;
      min-width: 320px;
      max-width: 640px;
      text-align: left;
    }
    .hero-text h1 {
      font-size: 3.1rem;
      font-weight: bold;
      margin-bottom: 10px;
    }
    .hero-text h2 {
      font-size: 2.1rem;
      font-weight: 500;
      margin-bottom: 22px;
      color: #21c4fe;
    }
    .hero-text p {
      margin-bottom: 32px;
      font-size: 1.16rem;
      color: #cdd9ed;
    }
    .hero-links {
      display: flex;
      gap: 17px;
      margin-top: 10px;
    }
    .hero-links a {
      color: #fff;
      font-size: 1.7rem;
      transition: color 0.18s;
      text-decoration: none;
    }
    .hero-links a:hover { color: #21c4fe; }
.hero-img {
      flex: 1;
      min-width: 260px;
      display: flex;
      align-items: center;
      justify-content: flex-end;
    }
    .hero-img img {
      width: 330px;
      height: auto;
      border-radius: 14px;
      box-shadow: 0 4px 24px #21c4fe22;
      background: #181f2b;
      object-fit: cover;
    }
    /* Section Titles */
    .section-title {
      text-align: left;
      font-size: 2.2rem;
      font-weight: bold;
      color: #21c4fe;
      margin-top: 70px;
      margin-bottom: 36px;
    }
    /* About Me Section */
    .about-section {
      display: flex;
      gap: 44px;
      align-items: flex-start;
      margin-bottom: 48px;
    }
    .about-img img {
      width: 440px;
      max-width: 96vw;
      border-radius: 16px;
      box-shadow: 0 2px 32px #e9407540;
      object-fit: cover;
    }
    .about-text {
      flex: 2;
      color: #fff;
      font-size: 1.15rem;
      text-align: left;
    }
    .about-text h2 {
      font-size: 2rem;
      font-weight: bold;
      color: #fff;
      margin-bottom: 20px;
    }
    /* Skills Grid */
    .skills-section {}
    .skills-group-title {
      color: #21c4fe;
      font-size: 1.25rem;
      font-weight: 600;
      text-align: left;
      margin-bottom: 15px;
      margin-top: 30px;
    }
    .skills-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 28px;
      margin-bottom: 10px;
      justify-content: flex-start;
    }
    .skill-card {
      background: #192344;
      border-radius: 14px;
      padding: 26px 10px 13px 10px;
      width: 200px;
      box-shadow: 0 2px 20px #0002;
      display: flex;
      flex-direction: column;
      align-items: center;
      transition: box-shadow 0.2s, transform 0.18s;
      font-size: 1.15rem;
    }
    .skill-card:hover {
      box-shadow: 0 4px 28px #21c4fe50;
      transform: translateY(-2px) scale(1.03);
    }
    .skill-icon {
      font-size: 2.6rem;
      margin-bottom: 8px;
      color: #21c4fe;
    }
    /* Projects Grid */
    .projects-section {}
    .projects-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 38px;
      margin-bottom: 35px;
      justify-content: flex-start;
    }
    .project-card {
      background: #18203c;
      border-radius: 13px;
      width: 340px;
      min-width: 280px;
      box-shadow: 0 2px 20px #21c4fe13;
      padding: 30px 18px 18px 18px;
      display: flex;
      flex-direction: column;
      margin-bottom: 26px;
      justify-content: space-between;
      transition: box-shadow 0.18s, transform 0.16s;
    }
    .project-card:hover {
      box-shadow: 0 3px 30px #21c4fe50;
      transform: scale(1.03);
    }
    .project-title {
      font-size: 2.4rem;
      color: #21c4fe;
      font-weight: bold;
      margin-bottom: 17px;
    }
    .project-desc {
      font-size: 1.08rem;
      color: #cdd9ed;
      margin-bottom: 5px;
    }
    .project-link {
      color: #21c4fe;
      text-decoration: none;
      font-weight: bold;
      margin-top: 10px;
      font-size: 1.1rem;
      display: inline-block;
      transition: color 0.18s;
    }
    .project-link:hover { color: #fff; }
    /* Contact Section */
    .contact-section {
      margin-bottom: 56px;
    }
    .contact-title {
      text-align: center;
      font-size: 2.1rem;
      font-weight: bold;
      margin-bottom: 18px;
    }
    .contact-desc {
      text-align: center;
      color: #d8e3f3;
      margin-bottom: 38px;
      font-size: 1.15rem;
    }
    .contact-form {
      background: #202b47;
      border-radius: 15px;
      padding: 28px 28px 22px 28px;
      max-width: 440px;
      margin: 0 auto 24px auto;
      display: flex;
      align-items: center;
      gap: 16px;
    }
    .contact-form input {
      flex: 2;
      padding: 13px 12px;
      border-radius: 8px;
      border: none;
      background: #243052;
      color: #fff;
      font-size: 1.05rem;
      outline: none;
      margin-right: 8px;
    }
    .contact-form button {
      flex: 1;
      background: #21c4fe;
      border: none;
      border-radius: 7px;
      color: #fff;
      font-weight: bold;
      padding: 12px 17px;
      font-size: 1.09rem;
      cursor: pointer;
      box-shadow: 0 2px 6px #21c4fe2f;
      transition: background 0.16s;
    }
    .contact-form button:hover {
      background: #1b9cce;
    }
    .contact-wait {
      color: #fff;
      font-size: 1.13rem;
      margin-left: 12px;
    }
    .say-hello-btn {
      display: block;
      margin: 0 auto;
      margin-top: 24px;
      font-size: 1.23rem;
      background: #21c4fe;
      color: #fff;
      border: none;
      border-radius: 21px;
      font-weight: bold;
      padding: 20px 38px;
      box-shadow: 0 2px 8px #21c4fe25;
      cursor: pointer;
      transition: background 0.18s;
      text-decoration: none;
    }
    .say-hello-btn:hover {
      background: #1693b3;
    }
    @media (max-width: 980px) {
      .main-content, .navbar { padding-left: 3vw; padding-right: 3vw;}
      .hero-section, .about-section { flex-direction: column;}
      .hero-img img, .about-img img { width: 95vw; max-width: 95vw;}
      .hero-img { justify-content: center; margin-top: 24px;}
    }
    @media (max-width: 600px) {
      .hero-text h1 { font-size: 2.1rem;}
      .hero-text h2 { font-size: 1.2rem;}
      .section-title { font-size: 1.3rem;}
      .project-title { font-size: 1.5rem;}
      .project-card { width: 98vw;}
      .skills-grid, .projects-grid { gap: 14px;}
      .skill-card, .project-card { width: 98vw;}
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar">
    <div class="nav-logo">Harsh.</div>
    <div class="nav-menu">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact" class="nav-contact-btn">Contact</a>
    </div>
  </nav>

  <div class="main-content">
    <!-- Hero -->
    <section class="hero-section" id="home">
      <div class="hero-text">
        <h1>Hi, I'm Harsh</h1>
        <h2>I'm a <span style="color:#21c4fe;">Data Analyst</span></h2>
        <p>
          I see data not just as a record of the past, but as the blueprint for the future. By applying AI and machine learning, I make that blueprint interactive. I turn raw numbers into predictive insights and strategic action, revealing the 'why' behind the 'what' to automate solutions and drive intelligent growth.
        </p>
        <div class="hero-links">
          <a href="#">🔗</a>
          <a href="#">🐙</a>
          <a href="#">📷</a>
        </div>
      </div>
      <div class="hero-img">
        <img src="https://raw.github.com/harsh-bca/portfolio-assets/blob/main/github_profile_pic.jpg" alt="Profile Photo"/>
      </div>
    </section>
<!-- About Me -->
    <section class="about-section" id="about">
      <div class="about-img">
        <img src="about.img" alt="Desk setup"/>
      </div>
      <div class="about-text">
        <h2>About Me</h2>
        <p>
          My passion lies at the intersection of data and intelligence. As a data and AI professional, I specialize in architecting end-to-end intelligent systems. I transform complex datasets into predictive models and build autonomous agentic workflows designed to solve real-world business challenges.<br><br>
          In the fast-paced world of AI, continuous learning is my core principle. When I'm not building models, you'll find me fine-tuning the latest LLMs, contributing to open-source AI frameworks, or exploring novel approaches to data visualization. Let's connect and build the future of intelligent automation together!
        </p>
      </div>
    </section>
<!-- Skills Section -->
    <div class="section-title" id="skills">My Skills</div>
    <div class="skills-group-title">Agentic AI & Transformers</div>
    <div class="skills-grid">
      <div class="skill-card"><span class="skill-icon">😊</span>Hugging Face</div>
      <div class="skill-card"><span class="skill-icon">🔁</span>Transformers</div>
      <div class="skill-card"><span class="skill-icon">👥</span>AutoGen</div>
      <div class="skill-card"><span class="skill-icon">👥</span>CrewAI</div>
      <div class="skill-card"><span class="skill-icon">📦</span>Google ADK</div>
    </div>
    <div class="skills-group-title">Data Analysis & Data Science</div>
    <div class="skills-grid">
      <div class="skill-card"><span class="skill-icon">🐍</span>Python</div>
      <div class="skill-card"><span class="skill-icon">🗄️</span>SQL</div>
      <div class="skill-card"><span class="skill-icon">🧠</span>Pandas & NumPy</div>
      <div class="skill-card"><span class="skill-icon">⚙️</span>Scikit-learn</div>
      <div class="skill-card"><span class="skill-icon">🤖</span>TensorFlow</div>
      <div class="skill-card"><span class="skill-icon">🦾</span>PyTorch</div>
    </div>
    <div class="section-title">Visualization Tools</div>
    <div class="skills-grid">
      <div class="skill-card"><span class="skill-icon">📊</span>Excel</div>
      <div class="skill-card"><span class="skill-icon">🗂️</span>Spreadsheets</div>
      <div class="skill-card"><span class="skill-icon">📉</span>Looker</div>
      <div class="skill-card"><span class="skill-icon">🧩</span>Power BI</div>
    </div>
    <div class="section-title">Cloud & Tools</div>
    <div class="skills-grid">
      <div class="skill-card"><span class="skill-icon">🌐</span>GCP</div>
      <div class="skill-card"><span class="skill-icon">☁️</span>Azure</div>
      <div class="skill-card"><span class="skill-icon">💎</span>Jira</div>
      <div class="skill-card"><span class="skill-icon">🐙</span>GitHub</div>
    </div>
<!-- Projects Section -->
    <div class="section-title" id="projects">My Projects</div>
    <div class="projects-grid">
      <div class="project-card">
        <div class="Youth Trends Analysis">GemBots</div>
        <div class="project-desc">
          An end-to-end data analytics project that uncovers the pulse of Gen Z India.
From digital habits to career dreams, this project dives deep into the real voices of today's youth using modern tools and smart visual storytelling.
        </div>
        <a href="#" class="https://github.com/harsh-bca/Youth-Trends-Analysis">View Project →</a>
      </div>
      <div class="project-card">
        <div class="EDA on Job Market Dataset">PipeGate</div>
        <div class="project-desc">
          Welcome to my analysis of the data job market, focusing on data analyst roles. This project was created out of a desire to navigate and understand the job market more effectively. It delves into the top-paying and in-demand skills to help find optimal job opportunities for data analysts.
        </div>
        <span style="color:#21c4fe;font-size:1rem;font-weight:500;">Under Process <span style="display:inline-block;width:50px;height:10px;background:#21c4fe;border-radius:6px;margin-left:8px;"></span></span>
        <a href="#" class="https://github.com/harsh-bca/EDA-Project">View Project →</a>
      </div>
      <div class="project-card">
        <div class="College Fee Dashboard">Portfolio</div>
        <div class="project-desc">
          The College Fee Dashboard is an interactive, real-time financial monitoring tool designed for educational institutions to streamline fee tracking, payment status monitoring, and automated reminders. Built using Looker Studio with data sourced from Excel sheets, the dashboard enables administrators to gain instant insights into fee collections, pending payments, and overall financial health.
        </div>
        <a href="#" class="https://github.com/harsh-bca/College-Fee-Dashboard">View Project →</a>
      </div>
    </div>
<!-- Contact Section -->
    <section class="contact-section" id="contact">
      <div class="contact-title">Get In Touch</div>
      <div class="contact-desc">
        I'm currently open to new opportunities and collaborations. Feel free to send me a message about anything you want to discuss!
      </div>
      <div class="contact-form">
        <span>Need help drafting a message?</span>
        <input type="text" placeholder="Enter keywords (e.g., 'AI project collaboration')"/>
        <button>✨ Draft</button>
        <span class="contact-wait">wait 5 seconds</span>
      </div>
      <a href="mailto:harsh.tripati21@gmail.com" class="say-hello-btn">Say Hello 📨</a>
    </section>
  </div>
</body>
</html>
