<!--
Filename: harsh_portfolio_tabbed.html
Description: Compact tabbed portfolio layout (one-screen friendly) for Harsh.
Instructions:
- Replace PROJECT README links with your Power BI "publish to web" iframe links when ready.
- Replace CERT image src and download hrefs with direct certificate file links in your repo or hosting.
- This is standalone HTML + CSS (no JS libraries). Save and open in browser to preview.
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Harsh Tripathi — Data Analyst</title>
  <style>
    :root{
      --accent:#007acc;
      --card-bg: rgba(255,255,255,0.9);
      --glass: rgba(255,255,255,0.06);
      --text:#0d1b2a;
      --muted:#485e75;
    }

  /* Page gradient background (full-screen) */
    html,body{height:100%; margin:0; font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;}
    body{
      background: linear-gradient(135deg, #0f172a 0%, #0b3b44 40%, #044e6c 100%);
      color:var(--text);
      -webkit-font-smoothing:antialiased;
      display:flex; align-items:center; justify-content:center; padding:24px;
    }

  /* Compact container that fits most screens */
    .container{
      width:100%; max-width:1150px; height:84vh; border-radius:14px; padding:18px; box-sizing:border-box;
      background: linear-gradient(180deg, rgba(255,255,255,0.03), rgba(255,255,255,0.02));
      box-shadow: 0 10px 40px rgba(2,6,23,0.6);
      display:grid; grid-template-columns: 260px 1fr; gap:18px; overflow:hidden;
      border: 1px solid rgba(255,255,255,0.06);
    }

  /* LEFT: Profile column */
    .profile{
      padding:18px; border-radius:10px; background:linear-gradient(180deg, rgba(255,255,255,0.03), rgba(255,255,255,0.01));
      display:flex; flex-direction:column; align-items:center; gap:12px; color:#e6f2ff; text-align:center;
    }
    .profile img{width:120px; height:120px; border-radius:50%; object-fit:cover; border:3px solid rgba(255,255,255,0.12);}    
    .name{font-size:18px; font-weight:700; color: #eaf6ff;}
    .role{font-size:13px; color:var(--muted);}    
    .cta{margin-top:6px; display:flex; gap:8px;}
    .btn{background:var(--accent); color:white; border:none; padding:8px 12px; border-radius:8px; text-decoration:none; font-weight:600; display:inline-block}
    .icon-link{background:transparent; border:1px solid rgba(255,255,255,0.06); padding:8px 10px; border-radius:8px; color:#dff6ff; text-decoration:none; font-weight:600}

/* CENTER + RIGHT: main area */
    .main{
      display:flex; flex-direction:column; gap:14px; overflow:hidden;
    }

/* Top area: video (center) + tiny intro line */
    .topbar{
      display:flex; gap:14px; align-items:center; justify-content:center; padding:6px; flex:0 0 280px;
    }
    .video-wrap{flex:1; border-radius:12px; overflow:hidden; min-height:150px; max-height:220px; box-shadow:0 8px 24px rgba(2,6,23,0.5);}
    .video-wrap iframe{width:100%; height:100%; border:0; display:block;}

  /* Tabs */
    .tabs{display:flex; gap:8px; align-items:center;}
    .tab-btn{background:transparent; border:0; color:#dff6ff; padding:10px 12px; border-radius:8px; cursor:pointer; font-weight:700}
    .tab-btn.active{background: linear-gradient(90deg,var(--accent), #00a3c4); box-shadow:0 6px 18px rgba(0,122,204,0.18);}

  /* Content area that changes with tabs */
    .content{
      background:var(--card-bg); border-radius:12px; padding:14px; overflow:auto; flex:1; min-height:0;
    }

  /* Compact cards inside content */
    .cards{display:grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap:12px;}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.98), rgba(255,255,255,0.96)); border-radius:10px; padding:12px; display:flex; gap:10px; align-items:center;}
    .card img.logo{width:44px; height:44px; border-radius:6px; object-fit:cover;}
    .card .meta{flex:1}
    .card h4{margin:0; font-size:15px; color:#06202b}
    .card p{margin:6px 0 0; font-size:13px; color:var(--muted)}
    .card a.link{font-weight:700; color:var(--accent); text-decoration:none; font-size:13px}

  /* Certifications grid: show badges in a compact row with download button */
    .cert-row{display:flex; gap:10px; align-items:center; flex-wrap:wrap}
    .cert-badge{width:140px; height:90px; border-radius:8px; overflow:hidden; display:flex; flex-direction:column; justify-content:center; align-items:center; background:#fff; box-shadow:0 6px 20px rgba(2,6,23,0.05)}
    .cert-badge img{max-width:110px; max-height:60px; object-fit:contain}
    .cert-actions{display:flex; gap:8px; margin-top:6px}

  /* Skills grid (logos only) */
    .skills{display:flex; gap:10px; flex-wrap:wrap; align-items:center}
    .skill{width:56px; height:56px; border-radius:10px; background:rgba(255,255,255,0.95); display:flex; align-items:center; justify-content:center}
    .skill img{width:36px; height:36px}

  /* Contact footer */
    .contact{display:flex; gap:10px; align-items:center}

  /* Make small screens stack nicely */
    @media (max-width:900px){
      .container{grid-template-columns:1fr; height:auto;}
      .profile{flex-direction:row; justify-content:center}
      .topbar{flex-direction:column}
    }
  </style>
</head>
<body>

  <div class="container" role="main"  <!-- LEFT: Profile -->
    <aside class="profile" aria-label="profile">
      <!-- Use your profile image hosted on GitHub raw link -->
      <img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/github_profile_pic.jpg" alt="Harsh Tripathi" />
      <div>
        <div class="name">Harsh Tripathi</div>
        <div class="role">Data Analyst • Power BI | SQL | Python</div>
        <div style="margin-top:10px; font-size:13px; color:#cfefff">EdTech · FinTech · E-commerce</div>

  <div class="cta">
          <a class="btn" href="https://github.com/harsh-bca/portfolio-assets/blob/main/Harsh_Tripathi_Data_Analyst_Resume.pdf" target="_blank">Resume</a>
          <a class="icon-link" href="https://www.linkedin.com/in/harsh-tripathi-64376333a/" target="_blank">LinkedIn</a>
        </div>
      </div>
    </aside>
<!-- RIGHT: Main area -->
    <section class="main">

<!-- TOP: Video centered -->
   <div class="topbar">
        <div style="flex:1; min-width:260px; text-align:center; color:#dff6ff">
          <div style="font-weight:700; font-size:14px; margin-bottom:8px">Intro Video</div>
          <div class="video-wrap">
            <!-- Placeholder: your Drive preview link. It shows inline on most browsers. Replace if needed. -->
            <iframe src="https://drive.google.com/file/d/1nYuJfaCucRcubVW8LNzWMyibpHnZTDif/preview" title="Intro Video" allowfullscreen></iframe>
          </div>
        </div>
      </div>

    <!-- Tabs -->
  <nav class="tabs" role="tablist" aria-label="portfolio tabs">
        <button class="tab-btn active" data-tab="projects">Projects</button>
        <button class="tab-btn" data-tab="certs">Certifications</button>
        <button class="tab-btn" data-tab="skills">Skills</button>
        <button class="tab-btn" data-tab="contact">Contact</button>
      </nav>

<!-- Content (tab panels) -->
  <div class="content">

    <!-- Projects Tab -->
  <div class="tab-panel" id="projects">
          <div style="display:flex; justify-content:space-between; align-items:center; margin-bottom:10px">
            <h3 style="margin:0">Featured Projects</h3>
            <small style="color:var(--muted)">Click a card to open the README / dashboard</small>
          </div>

  <div class="cards">

<!-- Project 1: Youth Trends -->
  <article class="card">
              <img class="logo" src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/Youth%20trends%20analysis%20banner.png" alt="Youth Trends" />
  <div class="meta">
                <h4>Youth Trends Analysis</h4>
                <p>Survey-based analysis with Python & Power BI.</p>
                <a class="link" href="https://github.com/harsh-bca/youth-trends-analysis" target="_blank">Open README / Dashboard</a>
              </div>
            </article>

    <!-- Project 2: EDA -->
  <article class="card">
              <img class="logo" src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/EDA%20project%20banner.png" alt="EDA" />
              <div class="meta">
                <h4>Global Job Market EDA</h4>
                <p>EDA + visual insights for hiring trends.</p>
                <a class="link" href="https://github.com/harsh-bca/EDA-Project" target="_blank">Open README / Dashboard</a>
              </div>
            </article>

  <!-- Project 3: NFHS -->
  <article class="card">
              <img class="logo" src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/NFHS%20data%20analysis%20banner.png" alt="NFHS" />
              <div class="meta">
                <h4>NFHS Health Survey</h4>
                <p>Large-scale health & demographic analysis in Power BI.</p>
                <a class="link" href="https://github.com/harsh-bca/National-Family-Health-Survey-Analysis" target="_blank">Open README / Dashboard</a>
              </div>
            </article>

  </div>

  </div>

  <!-- Certifications Tab -->
  <div class="tab-panel" id="certs" hidden>
          <div style="display:flex; justify-content:space-between; align-items:center; margin-bottom:10px">
            <h3 style="margin:0">Certifications</h3>
            <small style="color:var(--muted)">Click badge to view · Use download to save</small>
          </div>

  <div class="cert-row">
            <!-- Each badge links to the certificate image or file hosted on GitHub raw -->
            <div>
              <a href="https://github.com/harsh-bca/portfolio-assets/blob/main/google%20analytics%20certificate_page-0001.jpg" target="_blank" class="cert-badge">
                <img src="https://github.com/harsh-bca/portfolio-assets/blob/main/google%20analytics%20certificate_page-0001.jpg?raw=true" alt="Google Analytics" />
              </a>
              <div class="cert-actions">
                <a class="btn" href="https://github.com/harsh-bca/portfolio-assets/raw/main/google%20analytics%20certificate_page-0001.jpg" target="_blank">Download</a>
              </div>
            </div>

  <div>
              <a href="https://github.com/harsh-bca/portfolio-assets/blob/main/CertificateOfCompletion_Career%20Essentials%20in%20Data%20Analysis%20by%20Microsoft%20and%20LinkedIn_page-0001.jpg" target="_blank" class="cert-badge">
                <img src="https://github.com/harsh-bca/portfolio-assets/blob/main/CertificateOfCompletion_Career%20Essentials%20in%20Data%20Analysis%20by%20Microsoft%20and%20LinkedIn_page-0001.jpg?raw=true" alt="Career Essentials" />
              </a>
              <div class="cert-actions">
                <a class="btn" href="https://github.com/harsh-bca/portfolio-assets/raw/main/CertificateOfCompletion_Career%20Essentials%20in%20Data%20Analysis%20by%20Microsoft%20and%20LinkedIn_page-0001.jpg" target="_blank">Download</a>
              </div>
            </div>

  <div>
              <a href="https://github.com/harsh-bca/portfolio-assets/blob/main/wadhwani%20foundation%20certificate%20_page-0001.jpg" target="_blank" class="cert-badge">
                <img src="https://github.com/harsh-bca/portfolio-assets/blob/main/wadhwani%20foundation%20certificate%20_page-0001.jpg?raw=true" alt="Wadhwani" />
              </a>
              <div class="cert-actions">
                <a class="btn" href="https://github.com/harsh-bca/portfolio-assets/raw/main/wadhwani%20foundation%20certificate%20_page-0001.jpg" target="_blank">Download</a>
              </div>
            </div>

  </div>

  </div>

  <!-- Skills Tab -->
  <div class="tab-panel" id="skills" hidden>
          <div style="display:flex; justify-content:space-between; align-items:center; margin-bottom:10px">
            <h3 style="margin:0">Skills</h3>
            <small style="color:var(--muted)">Logos only — clean & compact</small>
          </div>

  <div class="skills">
            <div class="skill" title="Python"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python"/></div>
            <div class="skill" title="SQL"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" alt="SQL"/></div>
            <div class="skill" title="Power BI"><img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/powerbi_logo.png" alt="PowerBI"/></div>
            <div class="skill" title="Pandas"><img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/pandas_logo.png" alt="Pandas"/></div>
            <div class="skill" title="Matplotlib"><img src="https://raw.githubusercontent.com/harsh-bca/portfolio-assets/main/matplotlib_logo.png" alt="Matplotlib"/></div>
            <div class="skill" title="Azure"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/azure/azure-original.svg" alt="Azure"/></div>
          </div>

  </div>

<!-- Contact Tab -->
  <div class="tab-panel" id="contact" hidden>
          <h3 style="margin-top:0">Contact</h3>
          <div class="contact">
            <div style="font-weight:700">Email:</div>
            <div><a href="mailto:harsh.tripati21@gmail.com">harsh.tripati21@gmail.com</a></div>
          </div>
          <div style="margin-top:8px" class="contact">
            <div style="font-weight:700">LinkedIn:</div>
            <div><a href="https://www.linkedin.com/in/harsh-tripathi-64376333a/" target="_blank">harsh-tripathi-64376333a</a></div>
          </div>

  <div style="margin-top:12px; color:var(--muted); font-size:13px">© 2025 Harsh. Built with ❤️. Replace README links with Power BI embeds when ready.</div>
        </div>

  </div>

</section>

  </div>

  <script>
    // Tab switching (plain JS — tiny & dependency free)
    const tabs = document.querySelectorAll('.tab-btn');
    const panels = document.querySelectorAll('.tab-panel');
    tabs.forEach(btn => btn.addEventListener('click', ()=>{
      tabs.forEach(t=>t.classList.remove('active'));
      btn.classList.add('active');
      const id = btn.dataset.tab;
      panels.forEach(p=>{ p.hidden = p.id !== id; });
      // keep scroll at top of panel for quick scan
      document.querySelector('.content').scrollTop = 0;
    }));

    // Accessibility: allow first tab by default
    document.querySelector('.tab-btn.active').click();
  </script>

</body>
</html>
