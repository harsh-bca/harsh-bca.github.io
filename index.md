<!-- === Hero Section === -->
<section class="hero">
  <div class="hero-text">
    <h1>Harsh | Data Analyst Portfolio</h1>
    <p>✨ Welcome to my portfolio ✨</p>
  </div>
  <div class="hero-image">
    <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" 
         alt="Harsh Profile Pic">
  </div>
</section>

<style>
/* Hero Section */
.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 40px;
  max-width: 1100px;
  margin: auto;
  gap: 30px;
  flex-wrap: wrap; /* Responsive stacking */
}

/* Left Text */
.hero-text h1 {
  font-size: 2rem;
  margin-bottom: 10px;
}

.hero-text p {
  font-size: 1.2rem;
  color: #666;
}

/* Profile Picture */
.hero-image img {
  width: 250px;        /* control size */
  height: auto;
  border-radius: 50%;  /* circle pic */
  object-fit: cover;
  border: 4px solid #eee;
  box-shadow: 0 6px 15px rgba(0,0,0,0.2);
}
</style>
