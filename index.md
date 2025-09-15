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
  position: fixed;
  top: 30px;
  left: 30px;
  width: 200px;
}

/* Right Sidebar */
.right-sidebar {
  position: fixed;
  top: 30px;
  right: 30px;
  width: 220px;
}

/* Main Content */
.main-content {
  margin: 0 auto;
  max-width: 800px;
}
</style>

<div class="left-sidebar">
  <!-- Profile Pic -->
  <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" 
       alt="Harsh Profile Pic" style="width:120px; border-radius:50%; display:block; margin:auto;" />

  <!-- About Me -->
  <h3>👨‍💻 About Me</h3>
  <p style="font-size:14px; color:#333;">
    Hi, I’m <b>Harsh</b> — aspiring Data Analyst skilled in Python, SQL, Power BI, 
    and storytelling with data. Focused on EdTech, FinTech, E-commerce, and Healthcare.
  </p>

  <!-- Contact -->
  <h3>📬 Contact</h3>
  <ul style="list-style:none; padding:0;">
    <li>📧 <a href="mailto:harsh.tripati21@gmail.com">Email</a></li>
    <li>🔗 <a href="https://www.linkedin.com/in/harsh-tripathi-64376333a/">LinkedIn</a></li>
    <li>📷 <a href="https://www.instagram.com/harshanalyst2025?igsh=aTNyN2d4eXl1aTg=">Instagram</a></li>
  </ul>
</div>

