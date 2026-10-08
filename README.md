<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Research & Excellence (RE) | Research Foundation Center</title>
  
  <!-- Academic & Khmer Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Kantumruy+Pro:wght@400;600;700&family=Merriweather:ital,wght@0,300;0,400;0,700;1,300&display=swap" rel="stylesheet">
  
  <!-- FontAwesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    :root {
      --bg-dark: #080c16;
      --bg-card: #0f172a;
      --bg-card-hover: #162038;
      --navy-deep: #0a192f;
      --navy-bright: #1e3a8a;
      --gold-primary: #d4af37;
      --gold-light: #f59e0b;
      --gold-gradient: linear-gradient(135deg, #d4af37 0%, #fef08a 50%, #b45309 100%);
      --text-main: #f8fafc;
      --text-muted: #94a3b8;
      --border-color: rgba(212, 175, 55, 0.25);
      --font-sans: 'Inter', sans-serif;
      --font-serif: 'Merriweather', Georgia, serif;
      --font-khmer: 'Kantumruy Pro', sans-serif;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: var(--font-sans);
      background-color: var(--bg-dark);
      color: var(--text-main);
      line-height: 1.6;
      overflow-x: hidden;
    }

    /* Top Institutional Bar */
    .top-bar {
      background: #05080f;
      border-bottom: 1px solid rgba(212, 175, 55, 0.15);
      padding: 8px 5%;
      font-size: 0.85rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      color: var(--gold-primary);
    }
    .khmer-badge {
      font-family: var(--font-khmer);
      color: #cbd5e1;
      font-weight: 600;
    }

    /* Main Navigation */
    header {
      background: rgba(15, 23, 42, 0.95);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid var(--border-color);
      position: sticky;
      top: 0;
      z-index: 1000;
      padding: 12px 5%;
    }
    .nav-container {
      max-width: 1200px;
      margin: auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .brand {
      display: flex;
      align-items: center;
      gap: 16px;
      text-decoration: none;
      color: white;
    }
    .logo-container {
      width: 58px;
      height: 58px;
      position: relative;
      flex-shrink: 0;
    }
    .logo-img {
      width: 100%;
      height: 100%;
      object-fit: contain;
      display: none;
      border-radius: 8px;
    }
    .brand-text h1 {
      font-size: 1.25rem;
      font-weight: 700;
      letter-spacing: 1px;
      background: var(--gold-gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-transform: uppercase;
    }
    .brand-text p {
      font-size: 0.72rem;
      color: var(--text-muted);
      letter-spacing: 1.8px;
      text-transform: uppercase;
    }
    .nav-links {
      display: flex;
      gap: 22px;
      list-style: none;
      align-items: center;
    }
    .nav-links a {
      color: #cbd5e1;
      text-decoration: none;
      font-size: 0.9rem;
      font-weight: 500;
      transition: color 0.2s;
    }
    .nav-links a:hover {
      color: var(--gold-primary);
    }
    .btn-gold {
      background: linear-gradient(135deg, #d4af37, #b45309);
      color: #05080f !important;
      padding: 8px 18px;
      border-radius: 6px;
      font-weight: 700 !important;
      border: none;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: transform 0.2s, box-shadow 0.2s;
      text-decoration: none;
    }
    .btn-gold:hover {
      transform: translateY(-2px);
      box-shadow: 0 4px 15px rgba(212, 175, 55, 0.4);
    }

    /* Hero Section */
    .hero {
      position: relative;
      padding: 90px 5% 70px;
      background: radial-gradient(circle at 50% 20%, rgba(30, 58, 138, 0.25) 0%, rgba(8, 12, 22, 1) 75%);
      text-align: center;
      border-bottom: 1px solid rgba(212, 175, 55, 0.15);
    }
    .hero-container {
      max-width: 900px;
      margin: auto;
    }
    .hero-badge {
      display: inline-block;
      padding: 6px 16px;
      background: rgba(212, 175, 55, 0.1);
      border: 1px solid var(--gold-primary);
      border-radius: 50px;
      color: var(--gold-primary);
      font-size: 0.82rem;
      font-weight: 600;
      margin-bottom: 24px;
      letter-spacing: 1px;
    }
    .hero-title {
      font-family: var(--font-serif);
      font-size: 2.8rem;
      line-height: 1.25;
      margin-bottom: 20px;
      color: #ffffff;
    }
    .hero-title span {
      background: var(--gold-gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
    .hero-subtitle {
      font-size: 1.15rem;
      color: var(--text-muted);
      max-width: 750px;
      margin: 0 auto 35px;
      font-weight: 300;
    }
    .motto-strip {
      display: flex;
      justify-content: center;
      gap: 30px;
      font-size: 0.9rem;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: var(--gold-primary);
      font-weight: 600;
    }

    /* Container */
    .container {
      max-width: 1200px;
      margin: 60px auto;
      padding: 0 5%;
    }
    .section-header {
      margin-bottom: 35px;
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      border-bottom: 1px solid rgba(212, 175, 55, 0.2);
      padding-bottom: 15px;
    }
    .section-title {
      font-family: var(--font-serif);
      font-size: 1.8rem;
      color: #fff;
    }
    .section-title span {
      color: var(--gold-primary);
    }
    .section-desc {
      color: var(--text-muted);
      font-size: 0.95rem;
    }

    /* Research Tool: Biostatistical Calculator */
    .tool-box {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: 12px;
      padding: 30px;
      margin-bottom: 70px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.4);
    }
    .calc-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 30px;
      margin-top: 20px;
    }
    .input-group label {
      display: block;
      font-size: 0.85rem;
      color: var(--gold-primary);
      margin-bottom: 8px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }
    textarea, select, input {
      width: 100%;
      background: #070b14;
      border: 1px solid rgba(212, 175, 55, 0.3);
      padding: 12px;
      border-radius: 6px;
      color: #fff;
      font-family: var(--font-sans);
      font-size: 0.95rem;
      outline: none;
    }
    textarea:focus, select:focus, input:focus {
      border-color: var(--gold-primary);
    }
    .stat-results {
      background: #070b14;
      border: 1px solid rgba(255,255,255,0.08);
      border-radius: 8px;
      padding: 20px;
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 15px;
    }
    .stat-item {
      border-left: 2px solid var(--gold-primary);
      padding-left: 12px;
    }
    .stat-label {
      font-size: 0.75rem;
      color: var(--text-muted);
      text-transform: uppercase;
    }
    .stat-val {
      font-size: 1.4rem;
      font-weight: 700;
      color: #ffffff;
      font-family: var(--font-sans);
    }

    /* Blog Articles Grid */
    .blog-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
      gap: 25px;
    }
    .blog-card {
      background: var(--bg-card);
      border: 1px solid rgba(255, 255, 255, 0.08);
      border-radius: 10px;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      transition: transform 0.25s, border-color 0.25s;
    }
    .blog-card:hover {
      transform: translateY(-4px);
      border-color: var(--gold-primary);
      background: var(--bg-card-hover);
    }
    .card-banner {
      height: 140px;
      background: linear-gradient(135deg, #0f172a, #1e3a8a);
      position: relative;
      padding: 16px;
      display: flex;
      align-items: flex-end;
    }
    .category-tag {
      background: rgba(8, 12, 22, 0.85);
      border: 1px solid var(--gold-primary);
      color: var(--gold-primary);
      font-size: 0.75rem;
      padding: 4px 10px;
      border-radius: 4px;
      font-weight: 600;
      text-transform: uppercase;
    }
    .card-body {
      padding: 24px;
      display: flex;
      flex-direction: column;
      flex-grow: 1;
    }
    .card-meta {
      font-size: 0.8rem;
      color: var(--text-muted);
      margin-bottom: 10px;
      display: flex;
      gap: 15px;
    }
    .card-title {
      font-family: var(--font-serif);
      font-size: 1.25rem;
      color: #fff;
      margin-bottom: 12px;
      line-height: 1.4;
    }
    .card-excerpt {
      font-size: 0.9rem;
      color: var(--text-muted);
      margin-bottom: 20px;
      flex-grow: 1;
    }
    .card-footer {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding-top: 15px;
      border-top: 1px solid rgba(255, 255, 255, 0.08);
    }
    .read-btn {
      background: transparent;
      border: none;
      color: var(--gold-primary);
      font-weight: 600;
      font-size: 0.85rem;
      cursor: pointer;
      display: flex;
      align-items: center;
      gap: 6px;
      padding: 0;
    }
    .read-btn:hover {
      text-decoration: underline;
    }

    /* Reading Modal */
    .modal-overlay {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.85);
      backdrop-filter: blur(5px);
      z-index: 2000;
      overflow-y: auto;
      padding: 40px 15px;
    }
    .modal-content {
      background: var(--bg-card);
      border: 1px solid var(--gold-primary);
      border-radius: 12px;
      max-width: 820px;
      margin: auto;
      padding: 40px;
      position: relative;
    }
    .close-modal {
      position: absolute;
      top: 20px;
      right: 25px;
      font-size: 1.8rem;
      color: var(--text-muted);
      cursor: pointer;
      background: none;
      border: none;
    }
    .close-modal:hover {
      color: var(--gold-primary);
    }
    .modal-body {
      font-family: var(--font-serif);
      color: #e2e8f0;
      line-height: 1.8;
      font-size: 1.05rem;
      margin-top: 20px;
    }
    .modal-body h4 {
      font-family: var(--font-sans);
      color: var(--gold-primary);
      margin: 25px 0 10px;
    }
    .citation-box {
      margin-top: 30px;
      background: #070b14;
      border: 1px dashed var(--gold-primary);
      padding: 16px;
      border-radius: 6px;
      font-family: var(--font-sans);
      font-size: 0.85rem;
      color: var(--text-muted);
    }

    /* Footer */
    footer {
      background: #04060a;
      border-top: 1px solid rgba(212, 175, 55, 0.2);
      padding: 50px 5% 30px;
      margin-top: 80px;
      font-size: 0.9rem;
    }
    .footer-grid {
      max-width: 1200px;
      margin: auto;
      display: grid;
      grid-template-columns: 2fr 1fr 1fr;
      gap: 40px;
      margin-bottom: 40px;
    }
    .footer-about p {
      color: var(--text-muted);
      font-size: 0.85rem;
      margin-top: 12px;
      line-height: 1.7;
    }
    .footer-links h4 {
      color: var(--gold-primary);
      margin-bottom: 16px;
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }
    .footer-links ul {
      list-style: none;
    }
    .footer-links li {
      margin-bottom: 8px;
    }
    .footer-links a {
      color: var(--text-muted);
      text-decoration: none;
    }
    .footer-links a:hover {
      color: var(--gold-primary);
    }
    .footer-bottom {
      max-width: 1200px;
      margin: auto;
      padding-top: 20px;
      border-top: 1px solid rgba(255,255,255,0.06);
      display: flex;
      justify-content: space-between;
      color: var(--text-muted);
      font-size: 0.8rem;
    }

    @media (max-width: 768px) {
      .calc-grid, .footer-grid {
        grid-template-columns: 1fr;
      }
      .hero-title {
        font-size: 2rem;
      }
      .nav-links {
        display: none;
      }
    }
  </style>
</head>
<body>

  <!-- Institutional Bar -->
  <div class="top-bar">
    <div class="khmer-badge">
      <i class="fa-solid fa-flask-vial"></i> មជ្ឈមណ្ឌលស្រាវជ្រាវ និងឧត្តមភាពវិទ្យាសាស្ត្រ (Research Foundation Center)
    </div>
    <div>
      <span style="font-size: 0.75rem; letter-spacing: 1px;">PEER-REVIEW & OPEN SCIENCE PORTAL</span>
    </div>
  </div>

  <!-- Header Navigation -->
  <header>
    <div class="nav-container">
      <a href="#" class="brand">
        <!-- Exact Emblem Vector Implementation with Automatic Local Image Fallback -->
        <div class="logo-container" id="logoBox">
          <img id="customLogo" class="logo-img" src="1000053667.png" alt="RE Logo" onerror="handleLogoError()">
          <svg id="vectorLogo" viewBox="0 0 500 500" width="100%" height="100%">
            <!-- Golden Khmer Pagoda Crown Crest -->
            <g fill="url(#goldGradient)" stroke="#854d0e" stroke-width="2">
              <path d="M250,55 L257,80 L268,82 L260,95 L263,115 L250,105 L237,115 L240,95 L232,82 L243,80 Z" />
              <path d="M250,105 C265,115 285,120 300,140 C285,145 275,142 270,150 L275,160 C260,155 255,162 250,165 C245,162 240,155 225,160 L230,150 C225,142 215,145 200,140 C215,120 235,115 250,105 Z" />
              <rect x="235" y="158" width="30" height="6" rx="2" fill="#fef08a" />
            </g>
            <!-- Bilateral Laurel Wreath Branches -->
            <g fill="none" stroke="url(#goldGradient)" stroke-width="4" stroke-linecap="round">
              <path d="M125,330 C90,260 100,180 140,145" />
              <path d="M375,330 C410,260 400,180 360,145" />
            </g>
            <g fill="url(#goldGradient)">
              <!-- Left Wreath Leaves -->
              <ellipse cx="118" cy="300" rx="9" ry="16" transform="rotate(-30 118 300)" />
              <ellipse cx="103" cy="255" rx="9" ry="16" transform="rotate(-15 103 255)" />
              <ellipse cx="106" cy="210" rx="9" ry="16" transform="rotate(10 106 210)" />
              <ellipse cx="125" cy="170" rx="9" ry="16" transform="rotate(35 125 170)" />
              <!-- Right Wreath Leaves -->
              <ellipse cx="382" cy="300" rx="9" ry="16" transform="rotate(30 382 300)" />
              <ellipse cx="397" cy="255" rx="9" ry="16" transform="rotate(15 397 255)" />
              <ellipse cx="394" cy="210" rx="9" ry="16" transform="rotate(-10 394 210)" />
              <ellipse cx="375" cy="170" rx="9" ry="16" transform="rotate(-35 375 170)" />
            </g>
            <!-- Monogram Letters: Deep Navy 'R' & Golden 'E' -->
            <defs>
              <linearGradient id="navyGradient" x1="0%" y1="0%" x2="100%" y2="100%">
                <stop offset="0%" stop-color="#1e3a8a" />
                <stop offset="60%" stop-color="#0f265c" />
                <stop offset="100%" stop-color="#081430" />
              </linearGradient>
              <linearGradient id="goldGradient" x1="0%" y1="0%" x2="100%" y2="100%">
                <stop offset="0%" stop-color="#d4af37" />
                <stop offset="50%" stop-color="#fef08a" />
                <stop offset="100%" stop-color="#b45309" />
              </linearGradient>
            </defs>
            <!-- Golden 'E' in background -->
            <path d="M260,175 L360,175 L360,205 L295,205 L295,235 L345,235 L345,262 L295,262 L295,295 L365,295 L365,325 L260,325 Z" fill="url(#goldGradient)" stroke="#854d0e" stroke-width="2" />
            <!-- Deep Navy 'R' overlapping -->
            <path d="M150,165 L245,165 C285,165 305,185 305,215 C305,238 290,253 268,260 L320,335 L280,335 L235,268 L188,268 L188,335 L150,335 Z M188,198 L188,238 L240,238 C255,238 266,230 266,218 C266,205 255,198 240,198 Z" fill="url(#navyGradient)" stroke="url(#goldGradient)" stroke-width="3" />
            <!-- Open Foundation Book at the base -->
            <g fill="#0b1736" stroke="url(#goldGradient)" stroke-width="3">
              <path d="M130,345 Q250,330 250,360 Q250,330 370,345 L360,375 Q250,360 250,385 Q250,360 140,375 Z" />
              <!-- Inner book pages -->
              <path d="M145,355 Q250,342 250,368" stroke="#fef08a" stroke-width="1.5" fill="none" />
              <path d="M355,355 Q250,342 250,368" stroke="#fef08a" stroke-width="1.5" fill="none" />
            </g>
          </svg>
        </div>
        <div class="brand-text">
          <h1>Research & Excellence</h1>
          <p>Foundation Center</p>
        </div>
      </a>
      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#biostats">Statistical Suite</a></li>
        <li><a href="#articles">Research Articles</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="#biostats" class="btn-gold"><i class="fa-solid fa-calculator"></i> Run Analysis</a></li>
      </ul>
    </div>
  </header>

  <!-- Hero Banner -->
  <section class="hero">
    <div class="hero-container">
      <span class="hero-badge"><i class="fa-solid fa-certificate"></i> OPEN ACCESS METHODOLOGY HUB</span>
      <h2 class="hero-title">Empowering Scientific Inquiry Through <span>Methodological Rigor</span></h2>
      <p class="hero-subtitle">
        Bridging agricultural microbiology, bioprocess engineering, and biostatistical software analysis into practical scientific workflows.
      </p>
      <div class="motto-strip">
        <span>Knowledge</span> • <span>Innovation</span> • <span>Impact</span>
      </div>
    </div>
  </section>

  <!-- Main Content Container -->
  <div class="container">

    <!-- Interactive Tool: Biostatistical Experimental Summary Suite -->
    <section id="biostats" class="tool-box">
      <div class="section-header" style="margin-bottom: 20px;">
        <div>
          <h3 class="section-title">Experimental <span>Data Analyzer</span></h3>
          <p class="section-desc">Instantly compute Replicate metrics, Standard Error (SE), and CV% for laboratory & field trials</p>
        </div>
        <button class="btn-gold" onclick="exportAnalysisCSV()"><i class="fa-solid fa-download"></i> Export CSV</button>
      </div>

      <div class="calc-grid">
        <div>
          <div class="input-group">
            <label for="trialName">Experiment Title / Response Variable:</label>
            <input type="text" id="trialName" value="Trichoderma Inhibition Assay - Colony Diameter (mm)">
          </div>
          <div class="input-group" style="margin-top: 15px;">
            <label for="sampleData">Replicate Observations (Comma or Space separated):</label>
            <textarea id="sampleData" rows="4" placeholder="e.g. 24.5, 25.1, 23.8, 24.9, 25.4">24.5, 25.2, 23.9, 24.8, 25.5, 24.1</textarea>
          </div>
          <button class="btn-gold" style="margin-top: 15px; width: 100%; justify-content: center;" onclick="calculateStats()">
            <i class="fa-solid fa-microchip"></i> Compute Biostatistics
          </button>
        </div>

        <div class="stat-results">
          <div class="stat-item">
            <div class="stat-label">Replicates (n)</div>
            <div class="stat-val" id="resN">6</div>
          </div>
          <div class="stat-item">
            <div class="stat-label">Sample Mean (x̄)</div>
            <div class="stat-val" id="resMean">24.67</div>
          </div>
          <div class="stat-item">
            <div class="stat-label">Std. Deviation (SD)</div>
            <div class="stat-val" id="resSD">0.63</div>
          </div>
          <div class="stat-item">
            <div class="stat-label">Std. Error (SE)</div>
            <div class="stat-val" id="resSE">0.26</div>
          </div>
          <div class="stat-item" style="grid-column: span 2;">
            <div class="stat-label">Coefficient of Variation (CV %)</div>
            <div class="stat-val" id="resCV" style="color: var(--gold-light);">2.56%</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Articles / Blog Section -->
    <section id="articles">
      <div class="section-header">
        <div>
          <h3 class="section-title">Research Dispatches & <span>Methodologies</span></h3>
          <p class="section-desc">Practical laboratory guidelines, statistical reviews, and ecological assessments</p>
        </div>
      </div>

      <div class="blog-grid">
        <!-- Post 1 -->
        <article class="blog-card">
          <div class="card-banner">
            <span class="category-tag">Biostatistics</span>
          </div>
          <div class="card-body">
            <div class="card-meta">
              <span><i class="fa-regular fa-calendar"></i> October 2026</span>
              <span><i class="fa-regular fa-clock"></i> 6 min read</span>
            </div>
            <h4 class="card-title">Selecting Post-Hoc Tests: Tukey HSD vs. Duncan's Multiple Range Test</h4>
            <p class="card-excerpt">
              A comprehensive evaluation of Type I error rates across biological treatment comparisons in Completely Randomized Designs (CRD).
            </p>
            <div class="card-footer">
              <span style="font-size: 0.8rem; color: var(--gold-primary);">Dr. I. Sokra et al.</span>
              <button class="read-btn" onclick="openArticle(1)">Read Guide <i class="fa-solid fa-arrow-right"></i></button>
            </div>
          </div>
        </article>

        <!-- Post 2 -->
        <article class="blog-card">
          <div class="card-banner" style="background: linear-gradient(135deg, #064e3b, #0f172a);">
            <span class="category-tag">Microbiology</span>
          </div>
          <div class="card-body">
            <div class="card-meta">
              <span><i class="fa-regular fa-calendar"></i> September 2026</span>
              <span><i class="fa-regular fa-clock"></i> 8 min read</span>
            </div>
            <h4 class="card-title">Trichoderma spp. as Antagonistic Biocontrol Agents in Subtropical Crops</h4>
            <p class="card-excerpt">
              In vitro dual-culture assay protocols, volatile metabolite quantification, and mycelial inhibition evaluation methods.
            </p>
            <div class="card-footer">
              <span style="font-size: 0.8rem; color: var(--gold-primary);">Applied Biotech Lab</span>
              <button class="read-btn" onclick="openArticle(2)">Read Guide <i class="fa-solid fa-arrow-right"></i></button>
            </div>
          </div>
        </article>

        <!-- Post 3 -->
        <article class="blog-card">
          <div class="card-banner" style="background: linear-gradient(135deg, #78350f, #0f172a);">
            <span class="category-tag">Ecology</span>
          </div>
          <div class="card-body">
            <div class="card-meta">
              <span><i class="fa-regular fa-calendar"></i> August 2026</span>
              <span><i class="fa-regular fa-clock"></i> 5 min read</span>
            </div>
            <h4 class="card-title">Quantifying Wetland Floral Diversity: Shannon-Wiener vs. Simpson Indices</h4>
            <p class="card-excerpt">
              Standardized mathematical models for assessing species richness and evenness across seasonal Cambodian floodplains.
            </p>
            <div class="card-footer">
              <span style="font-size: 0.8rem; color: var(--gold-primary);">Ecology Unit</span>
              <button class="read-btn" onclick="openArticle(3)">Read Guide <i class="fa-solid fa-arrow-right"></i></button>
            </div>
          </div>
        </article>
      </div>
    </section>

    <!-- About Section -->
    <section id="about" style="margin-top: 80px;">
      <div class="tool-box">
        <h3 class="section-title" style="margin-bottom: 15px;">About <span>Research & Excellence</span></h3>
        <p style="color: var(--text-muted); font-size: 1rem; line-height: 1.8; margin-bottom: 20px;">
          The **Research Foundation Center** was established to support researchers, university lecturers, and thesis scholars in Cambodia and Southeast Asia. We focus on bridging rigorous academic methodologies with open computational tools—ranging from our desktop analytics suites to published peer-reviewed manuals in biotechnology and bioprocess engineering.
        </p>
        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px; margin-top: 25px;">
          <div style="border-left: 2px solid var(--gold-primary); padding-left: 15px;">
            <strong style="color: #fff; display: block;">Open Science</strong>
            <span style="color: var(--text-muted); font-size: 0.85rem;">Free access to methodologies, analysis protocols, and research manuals.</span>
          </div>
          <div style="border-left: 2px solid var(--gold-primary); padding-left: 15px;">
            <strong style="color: #fff; display: block;">Empirical Rigor</strong>
            <span style="color: var(--text-muted); font-size: 0.85rem;">Adhering to international peer-review standards and APA 7th scientific reporting.</span>
          </div>
          <div style="border-left: 2px solid var(--gold-primary); padding-left: 15px;">
            <strong style="color: #fff; display: block;">Applied Impact</strong>
            <span style="color: var(--text-muted); font-size: 0.85rem;">Connecting laboratory biotechnology with regional sustainable agriculture.</span>
          </div>
        </div>
      </div>
    </section>

  </div>

  <!-- Interactive Article Reading Modal -->
  <div id="readModal" class="modal-overlay">
    <div class="modal-content">
      <button class="close-modal" onclick="closeModal()">&times;</button>
      <div style="display: flex; gap: 10px; margin-bottom: 10px;">
        <span id="modalCategory" class="category-tag">Methodology</span>
      </div>
      <h2 id="modalTitle" style="font-family: var(--font-serif); font-size: 1.8rem; color: #fff; margin-bottom: 15px;">Article Title</h2>
      <div style="font-size: 0.85rem; color: var(--gold-primary); margin-bottom: 25px;" id="modalAuthor">By Dr. I. Sokra | Published Under Open Access</div>
      <div id="modalBody" class="modal-body">
        <!-- Injected via JavaScript -->
      </div>
      <div class="citation-box" id="modalCitation">
        <strong>Suggested Citation (APA 7th):</strong><br>
        <span id="citationText"></span>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer id="contact">
    <div class="footer-grid">
      <div class="footer-about">
        <h3 style="color: #fff; font-size: 1.1rem; text-transform: uppercase; letter-spacing: 1px;">Research & Excellence (RE)</h3>
        <p>
          Dedicated to advancing regional scientific inquiry, open-access biostatistical analysis, and sustainable agricultural biotechnology.
        </p>
        <p style="margin-top: 10px; font-family: var(--font-khmer); color: #cbd5e1;">
          ខេត្តក្រចេះ, ព្រះរាជាណាចក្រកម្ពុជា (Kratie Province, Cambodia)
        </p>
      </div>
      <div class="footer-links">
        <h4>Methodologies</h4>
        <ul>
          <li><a href="#biostats">Statistical Suite</a></li>
          <li><a href="#articles">Post-Hoc Modeling</a></li>
          <li><a href="#articles">Biocontrol Bioassays</a></li>
          <li><a href="#articles">Wetland Diversity</a></li>
        </ul>
      </div>
      <div class="footer-links">
        <h4>Resources</h4>
        <ul>
          <li><a href="https://github.com" target="_blank"><i class="fa-brands fa-github"></i> GitHub Repository</a></li>
          <li><a href="#about">APA 7th Formatting</a></li>
          <li><a href="#about">Research Foundation Guide</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <div>&copy; 2026 Research Foundation Center. All rights reserved.</div>
      <div>Knowledge • Innovation • Impact</div>
    </div>
  </footer>

  <script>
    // Automatic Logo Error Handling:
    // If 1000053667.png is found in the GitHub repo, it will display.
    // If not found yet, the inline SVG emblem renders seamlessly with 0 broken image icons.
    function handleLogoError() {
      const img = document.getElementById('customLogo');
      const svg = document.getElementById('vectorLogo');
      img.style.display = 'none';
      svg.style.display = 'block';
    }

    // Try loading custom logo image
    window.addEventListener('DOMContentLoaded', () => {
      const img = document.getElementById('customLogo');
      const svg = document.getElementById('vectorLogo');
      
      // Check if image loads properly
      img.onload = () => {
        img.style.display = 'block';
        svg.style.display = 'none';
      };
      // If error or missing, keep vector active
      img.onerror = () => {
        handleLogoError();
      };
      
      calculateStats();
    });

    // Biostatistics Calculator Logic
    function calculateStats() {
      const rawInput = document.getElementById('sampleData').value;
      const values = rawInput
        .split(/[\s,]+/)
        .map(v => parseFloat(v))
        .filter(v => !isNaN(v));

      if (values.length < 2) {
        alert("Please provide at least 2 numeric replicate values.");
        return;
      }

      const n = values.length;
      const sum = values.reduce((a, b) => a + b, 0);
      const mean = sum / n;
      
      const variance = values.reduce((acc, val) => acc + Math.pow(val - mean, 2), 0) / (n - 1);
      const sd = Math.sqrt(variance);
      const se = sd / Math.sqrt(n);
      const cv = (sd / mean) * 100;

      document.getElementById('resN').innerText = n;
      document.getElementById('resMean').innerText = mean.toFixed(2);
      document.getElementById('resSD').innerText = sd.toFixed(2);
      document.getElementById('resSE').innerText = se.toFixed(2);
      document.getElementById('resCV').innerText = cv.toFixed(2) + "%";
    }

    // Export Analysis to CSV
    function exportAnalysisCSV() {
      const title = document.getElementById('trialName').value || "Trial_Analysis";
      const n = document.getElementById('resN').innerText;
      const mean = document.getElementById('resMean').innerText;
      const sd = document.getElementById('resSD').innerText;
      const se = document.getElementById('resSE').innerText;
      const cv = document.getElementById('resCV').innerText;

      const csvContent = "data:text/csv;charset=utf-8," 
        + "Variable / Treatment,Replicates (n),Mean,Std Deviation,Std Error,CV (%)\n"
        + `"${title}",${n},${mean},${sd},${se},"${cv}"\n`;

      const encodedUri = encodeURI(csvContent);
      const link = document.createElement("a");
      link.setAttribute("href", encodedUri);
      link.setAttribute("download", `${title.replace(/[^a-z0-9]/gi, '_').toLowerCase()}_stats.csv`);
      document.body.appendChild(link);
      link.click();
      document.body.removeChild(link);
    }

    // Modal Knowledge Base Content
    const articles = {
      1: {
        category: "Biostatistics & Experimental Design",
        title: "Selecting Post-Hoc Tests: Tukey HSD vs. Duncan's Multiple Range Test",
        author: "Research Foundation Center • Statistical Unit",
        body: `
          <p>In agricultural and microbial research, ANOVA establishes whether significant variance exists between treatment means. However, identifying specific pairwise differences requires post-hoc comparisons.</p>
          <h4>1. Tukey’s Honestly Significant Difference (HSD)</h4>
          <p>Tukey's HSD strictly controls the experiment-wise Type I error rate (α = 0.05). It is recommended by leading international peer-reviewed journals when all possible pairwise mean comparisons are evaluated.</p>
          <h4>2. Duncan's Multiple Range Test (DMRT)</h4>
          <p>While historically favored in agronomy for its higher statistical power in detecting marginal differences, DMRT does not control the experiment-wise error rate at the nominal alpha level, increasing the likelihood of false positives (Type I error).</p>
          <h4>Methodological Recommendation:</h4>
          <p>For publication in high-impact biotechnology and food science journals, prefer <strong>Tukey's HSD</strong> or <strong>Bonferroni</strong> adjustments over DMRT to ensure empirical reproducibility.</p>
        `,
        citation: "Research Foundation Center. (2026). Comparative evaluation of post-hoc pairwise multiple comparison tests in agricultural bioassays. Research & Excellence Reports, 4(1), 12-18."
      },
      2: {
        category: "Microbial Biotechnology",
        title: "Trichoderma spp. as Antagonistic Biocontrol Agents in Subtropical Crops",
        author: "Research Foundation Center • Life Sciences Unit",
        body: `
          <p>Fungal plant pathogens pose significant threats to cash crop yields. Biological control utilizing antagonistic fungi like <em>Trichoderma harzianum</em> and <em>Trichoderma viride</em> offers an eco-friendly alternative to synthetic fungicides.</p>
          <h4>Mechanisms of Antagonism</h4>
          <p>Dual-culture assays reveal three primary antagonistic modes: mycoparasitism, nutrient competition, and the secretion of hydrolytic enzymes (chitinases, β-1,3-glucanases).</p>
          <h4>Evaluation Protocol</h4>
          <p>Colony radial growth inhibition percentage (PIRG) is calculated using the standard formula:</p>
          <p style="background: rgba(255,255,255,0.05); padding: 10px; border-radius: 4px; font-family: monospace;">PIRG (%) = [(R1 - R2) / R1] × 100</p>
          <p>Where <em>R1</em> represents the control colony radius and <em>R2</em> represents the colony radius toward the antagonist.</p>
        `,
        citation: "Research Foundation Center. (2026). In vitro bioassay protocols for screening antagonistic Trichoderma strains against phytopathogenic fungi. Journal of Applied Bioprocess Engineering, 2(3), 45-52."
      },
      3: {
        category: "Ecology & Environmental Science",
        title: "Quantifying Wetland Floral Diversity: Shannon-Wiener vs. Simpson Indices",
        author: "Research Foundation Center • Environmental Analytics",
        body: `
          <p>Wetland habitats along the Mekong basin exhibit seasonal hydrological shifts that drive rapid changes in plant community structures.</p>
          <h4>Index Comparisons</h4>
          <p><strong>Shannon-Wiener Index (H'):</strong> Emphasizes species richness and is sensitive to rare species within sample transects.</p>
          <p><strong>Simpson’s Dominance Index (D):</strong> Weights abundant species more heavily, quantifying the probability that two randomly selected individuals belong to the same species.</p>
          <h4>Best Practice for Regional Surveys</h4>
          <p>Report both <em>H'</em> and Pielou's Evenness Index (<em>J'</em>) to ensure clear differentiation between sheer species count and structural dominance.</p>
        `,
        citation: "Research Foundation Center. (2026). Biodiversity assessment protocols for seasonal wetland conservation zones. Environmental Management Monographs, 1(2), 77-84."
      }
    };

    function openArticle(id) {
      const art = articles[id];
      if (!art) return;
      document.getElementById('modalCategory').innerText = art.category;
      document.getElementById('modalTitle').innerText = art.title;
      document.getElementById('modalAuthor').innerText = art.author;
      document.getElementById('modalBody').innerHTML = art.body;
      document.getElementById('citationText').innerText = art.citation;
      document.getElementById('readModal').style.display = 'block';
      document.body.style.overflow = 'hidden';
    }

    function closeModal() {
      document.getElementById('readModal').style.display = 'none';
      document.body.style.overflow = 'auto';
    }

    // Close modal on outside click
    window.onclick = function(event) {
      const modal = document.getElementById('readModal');
      if (event.target === modal) {
        closeModal();
      }
    };
  </script>
</body>
</html>
