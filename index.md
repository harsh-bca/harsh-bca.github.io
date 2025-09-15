<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Harsh | Data Analyst Portfolio</title>
  <style>
    /* ===== Reset ===== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #f9f9f9;
      color: #333;
    }
/* ===== Navbar ===== */
    nav {
      display: flex;
      justify-content: center;
      gap: 30px;
      padding: 20px;
      background: white;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    nav a {
      text-decoration: none;
      color: #333;
      font-weight: 500;
      transition: 0.3s;
    }
    nav a:hover {
      color: #0077ff;
    }
/* ===== Hero Section ===== */
    .hero {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 80px 10%;
      min-height: 90vh;
    }
    .hero-text {
      max-width: 550px;
    }
    .hero-text h1 {
      font-size: 42px;
      font-weight: bold;
      margin-bottom: 10px;
    }
    .hero-text h2 {
      font-size: 24px;
      color: #0077ff;
      margin-bottom: 20px;
      white-space: nowrap;
      border-right: 2px solid;
      overflow: hidden;
      animation: typing 3.5s steps(30, end) infinite, blink 0.75s step-end infinite;
    }
    @keyframes typing {
      from { width: 0 }
      to { width: 100% }
    }
    @keyframes blink {
      50% { border-color: transparent }
    }
    .hero-text p {
      font-size: 16px;
      line-height: 1.6;
      margin-bottom: 20px;
    }
.btn {
      display: inline-block;
      padding: 10px 20px;
      margin: 10px 10px 0 0;
      font-size: 15px;
      border-radius: 6px;
      text-decoration: none;
      transition: 0.3s;
    }
    .btn-primary {
      background: #0077ff;
      color: white;
    }
    .btn-primary:hover {
      background: #005fcc;
    }
    .btn-outline {
      border: 2px solid #0077ff;
      color: #0077ff;
    }
    .btn-outline:hover {
      background: #0077ff;
      color: white;
    }
.social-links a {
      margin-right: 15px;
      text-decoration: none;
      font-size: 20px;
      color: #333;
    }
    .social-links a:hover {
      color: #0077ff;
    }/* Profile Pic Glow */
    .hero-image {
      position: relative;
      width: 300px;
      height: 300px;
    }
    .hero-image::before {
      content: "";
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 320px;
      height: 320px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(0,119,255,0.4), transparent 70%);
      z-index: 0;
      animation: pulse 3s infinite;
    }
    .hero-image img {
      position: relative;
      width: 100%;
      height: 100%;
      border-radius: 50%;
      border: 5px solid white;
      z-index: 1;
    }
    @keyframes pulse {
      0% { transform: translate(-50%, -50%) scale(1); opacity: 0.7; }
      50% { transform: translate(-50%, -50%) scale(1.1); opacity: 0.4; }
      100% { transform: translate(-50%, -50%) scale(1); opacity: 0.7; }
    }
/* ===== Services Section ===== */
    .services {
      padding: 80px 10%;
      text-align: center;
      background: #fff;
    }
    .services h2 {
      font-size: 36px;
      margin-bottom: 40px;
      color: #0077ff;
    }
    .service-cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }
    .card {
      background: #f9f9f9;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    }
    .card h3 {
      margin-top: 15px;
      font-size: 20px;
      color: #333;
    }
    .card p {
      font-size: 15px;
      margin-top: 10px;
      line-height: 1.6;
      color: #555;
    }
    .icon {
      font-size: 40px;
      color: #0077ff;
    }

  </style>
</head>
<body>

  <!-- ===== Navbar ===== -->
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>

  <!-- ===== Hero Section ===== -->
  <section class="hero" id="home">
    <div class="hero-text">
      <h1>Hi, I'm Harsh</h1>
      <h2>I am a Data Analyst / Automation Specialist</h2>
      <p>
        I see data not just as a record of the past, but as the blueprint for the future.
        By applying AI and machine learning, I make that blueprint interactive.
        I turn raw numbers into predictive insights and strategic action,
        revealing the 'why' behind the 'what' to automate solutions and drive intelligent growth.
      </p>
      <div class="social-links">
        <a href="https://www.linkedin.com/in/harsh-tripathi-64376333a/" target="_blank">🔗 LinkedIn</a>
        <a href="https://github.com/harsh-bca" target="_blank">💻 GitHub</a>
        <a href="https://www.instagram.com/harshanalyst2025" target="_blank">📷 Instagram</a>
      </div>
      <a href="https://github.com/harsh-bca/portfolio-assets/blob/main/Harsh_Tripathi_Data_Analyst_Resume.pdf" 
         target="_blank" class="btn btn-primary">📄 Download Resume</a>
      <a href="#contact" class="btn btn-outline">💬 Hire Me</a>
    </div>

  <div class="hero-image">
      <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" alt="Harsh Profile Pic">
    </div>
  </section>

  <!-- ===== Services Section ===== -->
  <section class="services" id="services">
    <h2>My Services</h2>
    <div class="service-cards">
      <div class="card">
        <div class="icon">📊</div>
        <h3>Dashboard Creation</h3>
        <p>Interactive dashboards in Power BI & Tableau to visualize KPIs and enable data-driven decision making.</p>
      </div>
      <div class="card">
        <div class="icon">⚙️</div>
        <h3>Automated Reporting</h3>
        <p>Automation of recurring reports using Python, SQL, and APIs to save time and reduce errors.</p>
      </div>
      <div class="card">
        <div class="icon">📈</div>
        <h3>Data Insights</h3>
        <p>Deep-dive analysis to uncover trends, optimize processes, and provide actionable business recommendations.</p>
      </div>
    </div>
  </section>

</body>
</html>
