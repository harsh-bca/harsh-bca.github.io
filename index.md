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

<!-- ✅ Top Navigation -->
<div class="top-nav">
  <a href="#my-work">My Work</a>
  <a href="#certificates">Certificates</a>
  <a href="#contact">Contact</a>
</div>

<h2 class="animated-heading">📢 Data Tells The Truth</h2>

---

## 🎥 Meet Harsh – Beyond the Resume
<!-- Your existing intro content remains here -->

---

## 💼 Featured Projects <a id="my-work"></a>
<!-- Your existing project section stays same -->

---

## 🧾 Certifications <a id="certificates"></a>
<!-- Your certifications grid stays same -->

---

## 📬 Contact <a id="contact"></a>

- 📧 [harsh.tripati21@gmail.com](mailto:harsh.tripati21@gmail.com)  
- 🌐 [LinkedIn](https://www.linkedin.com/in/harsh-tripathi-64376333a/)  
- 📷 [Instagram](https://www.instagram.com/harshanalyst2025?igsh=aTNyN2d4eXl1aTg=)  

<!-- Simple Email Form -->
<div style="max-width:500px; margin:20px auto; background:#f9f9f9; padding:20px; border-radius:10px; box-shadow:0px 4px 10px rgba(0,0,0,0.1);">
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
