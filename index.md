<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Harsh Tripathi | Portfolio</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: #fff;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
      height: 100vh;
      overflow: hidden;
        <style>
    <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: #fff;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
      height: 100vh;
      overflow: hidden;
    }
/* ✅ Certifications Styling */
    .certificates ul {
      list-style: none;
      padding: 0;
    }
.certificates li {
      margin: 10px 0;
    }
.certificates a {
      display: inline-block;
      padding: 8px 14px;
      border-radius: 8px;
      text-decoration: none;
      background: linear-gradient(135deg, #6a11cb, #2575fc);
      color: #fff;
      font-weight: 500;
      transition: 0.3s;
    }
.certificates a:hover {
      background: linear-gradient(135deg, #2575fc, #6a11cb);
    }
/* Top Row Layout */
.top-row {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 40px;             /* spacing between profile and video */
  flex-wrap: wrap;       /* stack on smaller screens */
  margin-bottom: 40px;
}
/* Profile Image */
.profile-image img {
  max-width: 180px;
  width: 100%;
  height: auto;
  border-radius: 50%;
  object-fit: cover;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
}
/* Video Container */
.video-container iframe {
  max-width: 480px;
  width: 100%;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
}
}
/* Tabs */
    .tabs {
      display: flex;
      margin-top: 20px;
      gap: 20px;
    }
.tab {
      padding: 10px 20px;
      border-radius: 20px;
      background: rgba(255, 255, 255, 0.1);
      cursor: pointer;
      font-weight: bold;
      transition: all 0.3s ease;
    }
.tab.active {
      background: #0077b6;
    }
/* Content */
    .content {
      margin-top: 20px;
      width: 80%;
      max-width: 900px;
      text-align: center;
      background: rgba(255, 255, 255, 0.05);
      border-radius: 15px;
      padding: 20px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    }
.tab-content {
      display: none;
    }
    .tab-content.active {
      display: block;
    }
.card {
      background: rgba(255,255,255,0.1);
      margin: 10px;
      padding: 15px;
      border-radius: 12px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.3);
    }
.card img {
      width: 40px;
      height: 40px;
      border-radius: 5px;
    }
.skills img {
      width: 60px;
      margin: 10px;
      filter: drop-shadow(0 2px 5px rgba(0,0,0,0.4));
    }
/* Contact */
    .contact {
      position: absolute;
      bottom: 15px;
      text-align: center;
    }
.contact a {
      margin: 0 10px;
      color: #fff;
      text-decoration: none;
      font-size: 24px;
      transition: 0.3s;
    }
   .contact a:hover {
      color: #00b4d8;
    }
  </style>
</head>
<body>

  <!-- Top Row -->
  <div class="top-row">
  
  <!-- Profile Image -->
  <div class="profile-image">
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" 
         alt="Harsh Tripathi">
  </div>

  <!-- Intro Video -->
  <div class="video-container">
    <iframe src="https://drive.google.com/file/d/1nYuJfaCucRcubVW8LNzWMyibpHnZTDif/preview"
            width="480" height="270"
            frameborder="0" allow="autoplay"></iframe>
  </div>

</div>


  <!-- Tabs -->
  <div class="tabs">
    <div class="tab active" onclick="showTab('projects')">Projects</div>
    <div class="tab" onclick="showTab('certifications')">Certifications</div>
    <div class="tab" onclick="showTab('skills')">Skills</div>
  </div>

  <!-- Content Area -->
  <div class="content">
    <!-- Projects -->
    <div id="projects" class="tab-content active">
      <h2>Featured Projects</h2>
      <div class="card">
        <h3>Youth Trends Analysis</h3>
        <p>Survey-based analysis with Excel, Python & Power BI.</p>
        <a href="https://github.com/harsh-bca/Youth-Trends-Analysis">Open README / Dashboard</a>
      </div>
      <div class="card">
        <h3>Global Job Market EDA</h3>
        <p>EDA + visual insights for hiring trends.</p>
        <a href="https://github.com/harsh-bca/EDA-Project">Open README / Dashboard</a>
      </div>
    </div>

  <div class="certificates">
  <h2>Certifications</h2>
  <ul>
    <li><a href="https://github.com/harsh-bca/portfolio-assets/blob/main/grastech%20certificate.jpg" target="_blank">Data Science & AI – Grastech</a></li>
    <li><a href="https://github.com/harsh-bca/portfolio-assets/blob/main/wadhwani%20foundation%20certificate%20_page-0001.jpg" target="_blank">Soft Skills – Wadhwani Foundation</a></li>
    <li><a href="https://github.com/harsh-bca/portfolio-assets/blob/main/SQL%20certification%20_page-0001.jpg" target="_blank">SQL Certification</a></li>
    <li><a href="https://github.com/harsh-bca/portfolio-assets/blob/main/CertificateOfCompletion_Career%20Essentials%20in%20Data%20Analysis%20by%20Microsoft%20and%20LinkedIn_page-0001.jpg" target="_blank">Data Analysis Certification</a></li>
  </ul>
</div>

    <!-- Skills -->
  <div id="skills" class="tab-content skills">
      <h2>Skills</h2>
      <img src="python-logo.png" alt="Python">
      <img src="sql-logo.png" alt="SQL">
      <img src="powerbi-logo.png" alt="Power BI">
      <img src="tableau-logo.png" alt="Tableau">
      <img src="excel-logo.png" alt="Excel">
    </div>
  </div>

  <!-- Contact -->
  <div class="contact">
    <a href="mailto:harsh.tripati21@gmail.com">📧</a>
    <a href="https://www.linkedin.com/in/YOUR-LINKEDIN" target="_blank">🔗</a>
  </div>

  <!-- Script -->
  <script>
    function showTab(tabId) {
      document.querySelectorAll('.tab-content').forEach(el => el.classList.remove('active'));
      document.querySelectorAll('.tab').forEach(el => el.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
      event.target.classList.add('active');
    }
  </script>
</body>
</html>
