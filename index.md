<style>
/* === 3-column layout === */
.page-layout {
  display: grid;
  grid-template-columns: 220px 1fr 250px; /* left | center | right */
  gap: 20px;
  margin: 40px;
}

/* Left Sidebar */
.left-sidebar {
  padding: 20px;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.left-sidebar img {
  width: 120px;
  border-radius: 50%;
  display: block;
  margin: 0 auto 15px;
}

.left-sidebar h3 {
  margin-top: 15px;
  font-size: 16px;
}

.left-sidebar p {
  font-size: 14px;
  color: #333;
  line-height: 1.4;
}

.left-sidebar ul {
  list-style: none;
  padding: 0;
  margin: 0;
  font-size: 14px;
}

.left-sidebar li {
  margin: 5px 0;
}

/* Main Content */
.main-content {
  padding: 20px;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

/* Right Sidebar */
.right-sidebar {
  padding: 20px;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}
</style>

<div class="page-layout">
  <!-- Left Sidebar -->
  <div class="left-sidebar">
    <!-- Profile Pic -->
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" 
         alt="Harsh Profile Pic" />
<!-- About Me -->
    <h3>👨‍💻 About Me</h3>
    <p>
      Hi, I’m <b>Harsh</b> — aspiring Data Analyst skilled in Python, SQL, Power BI, 
      and storytelling with data. Focused on EdTech, FinTech, E-commerce, and Healthcare.
    </p>
<!-- Contact -->
    <h3>📬 Contact</h3>
    <ul>
      <li>📧 <a href="mailto:harsh.tripati21@gmail.com">Email</a></li>
      <li>🔗 <a href="https://www.linkedin.com/in/harsh-tripathi-64376333a/">LinkedIn</a></li>
      <li>📷 <a href="https://www.instagram.com/harshanalyst2025?igsh=aTNyN2d4eXl1aTg=">Instagram</a></li>
    </ul>
  </div>

  <!-- Main Content -->
  <div class="main-content">
    <h1 style="text-align:center;">Harsh | Data Analyst Portfolio</h1>
    <p style="text-align:center;">✨ Welcome to my portfolio ✨</p>
  </div>

  <!-- Right Sidebar -->
  <div class="right-sidebar">
    <h3>📰 Updates</h3>
    <p>Add certifications, blogs, or news here.</p>
  </div>
</div>
