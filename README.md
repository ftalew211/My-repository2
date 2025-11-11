<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Ftalew Dagnaw | Professional Portfolio</title>
  <meta name="description" content="Portfolio of Ftalew Dagnaw Gebreyesus, Senior Monitoring & Evaluation Advisor specializing in health information systems and data-driven public health outcomes." />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    /* * All CSS has been embedded here for a single, easy-to-copy file.
     * The styles ensure a professional, dark-mode, modern portfolio design.
     */
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');

    :root {
      --primary-blue: #0c2d64;
      --secondary-blue: #1e4fb8;
      --accent-cyan: #6bdcff;
      --accent-gold: #ffcb66;
      --text-light: #f5f9ff;
      --text-muted: #d0e2ff;
      --bg-deep: #00102a;
      --card-bg: rgba(11, 39, 93, 0.55);
      --card-border: rgba(140, 197, 255, 0.28);
      --nav-bg: rgba(4, 23, 63, 0.85);
      --shadow-soft: 0 22px 45px rgba(2, 15, 51, 0.38);
      --shadow-lift: 0 28px 60px rgba(10, 43, 122, 0.42);
      --transition: 0.3s ease;
      --max-width: 1100px;
    }

    *, *::before, *::after {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      font-family: 'Inter', 'Helvetica Neue', Arial, sans-serif;
      color: var(--text-light);
      background-color: var(--bg-deep);
      background-image:
        radial-gradient(circle at 10% 15%, rgba(86, 140, 255, 0.6) 0%, transparent 55%),
        radial-gradient(circle at 80% 0%, rgba(0, 193, 255, 0.38) 0%, transparent 60%),
        linear-gradient(140deg, #02123a 0%, #052f7d 55%, #0a4bac 100%);
      background-attachment: fixed;
      scroll-behavior: smooth;
      line-height: 1.6;
    }

    ::selection {
      background: rgba(100, 181, 246, 0.38);
      color: #fff;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    a:hover,
    a:focus-visible {
      color: var(--accent-cyan);
      text-decoration: underline;
    }

    img {
      display: block;
      max-width: 100%;
      height: auto;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 20;
      background: var(--nav-bg);
      backdrop-filter: blur(18px);
      border-bottom: 1px solid rgba(140, 197, 255, 0.12);
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
    }

    .nav {
      width: min(92%, var(--max-width));
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1.5rem;
      padding: 0.85rem 0;
    }

    .nav__brand {
      font-weight: 700;
      font-size: clamp(1.05rem, 1.8vw, 1.3rem);
      letter-spacing: 0.06em;
      text-transform: uppercase;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      color: var(--accent-cyan);
    }

    .nav__links {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 1.25rem;
      list-style: none;
      margin: 0;
      padding: 0;
    }

    .nav__links a {
      padding: 0.55rem 0.9rem;
      border-radius: 999px;
      transition: background-color var(--transition), color var(--transition), transform var(--transition);
      font-weight: 500;
    }

    .nav__links a:hover,
    .nav__links a:focus-visible {
      background-color: rgba(255, 255, 255, 0.16);
      color: #fff;
      transform: translateY(-2px);
    }

    .nav__toggle {
      display: none;
      border: 1px solid rgba(140, 197, 255, 0.45);
      background: rgba(21, 61, 146, 0.35);
      color: var(--text-light);
      padding: 0.45rem 0.75rem;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color var(--transition), border-color var(--transition);
    }

    .nav__toggle:hover,
    .nav__toggle:focus-visible {
      background: rgba(33, 94, 198, 0.45);
      border-color: rgba(140, 197, 255, 0.75);
    }

    main {
      display: block;
    }

    .section {
      padding: clamp(3.5rem, 5vw, 5.5rem) 0;
    }

    .container {
      width: min(92%, var(--max-width));
      margin: 0 auto;
    }

    .hero {
      display: grid;
      align-items: center;
      gap: clamp(1.75rem, 5vw, 4rem);
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    }

    .hero__eyebrow {
      text-transform: uppercase;
      font-size: 0.85rem;
      letter-spacing: 0.4em;
      color: rgba(237, 245, 255, 0.65);
      margin-bottom: 1.1rem;
      display: inline-block;
    }

    .hero__text h1 {
      font-size: clamp(2.25rem, 5vw, 3.35rem);
      line-height: 1.15;
      margin: 0 0 1.1rem;
      text-shadow: 0 12px 40px rgba(0, 0, 0, 0.45);
      background: linear-gradient(135deg, var(--accent-cyan) 0%, #ffffff 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero__text p {
      margin: 0 0 1.8rem;
      line-height: 1.75;
      color: var(--text-muted);
      max-width: 38rem;
    }

    .hero__cta {
      display: inline-flex;
      align-items: center;
      gap: 0.6rem;
      padding: 0.95rem 1.8rem;
      border-radius: 999px;
      background: linear-gradient(135deg, #6bdcff 0%, #4aa8ff 100%);
      color: #01203f;
      font-weight: 600;
      box-shadow: var(--shadow-lift);
      transition: transform var(--transition), box-shadow var(--transition);
      position: relative;
      overflow: hidden;
    }

    .hero__cta::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
      transition: left var(--transition);
    }

    .hero__cta:hover::before,
    .hero__cta:focus-visible::before {
      left: 100%;
    }

    .hero__cta:hover,
    .hero__cta:focus-visible {
      transform: translateY(-4px);
      box-shadow: 0 32px 60px rgba(18, 74, 158, 0.45);
      color: #001a32;
    }

    .hero__image {
      position: relative;
      display: grid;
      place-items: center;
    }

    .portrait-frame {
      position: relative;
      isolation: isolate;
      padding: clamp(0.55rem, 2vw, 0.9rem);
      border-radius: 26px;
      background: linear-gradient(145deg, rgba(100, 181, 246, 0.45) 0%, rgba(8, 34, 96, 0.85) 100%);
      box-shadow: var(--shadow-lift);
      overflow: hidden;
      animation: float 6s ease-in-out infinite;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    .portrait-frame::before {
      content: "";
      position: absolute;
      inset: 14%;
      border-radius: 20px;
      background: rgba(106, 190, 255, 0.18);
      filter: blur(34px);
      z-index: -2;
    }

    .hero__portrait {
      width: min(310px, 82vw);
      aspect-ratio: 3 / 4;
      border-radius: 20px;
      border: 2px solid rgba(245, 249, 255, 0.35);
      box-shadow: 0 22px 44px rgba(2, 18, 62, 0.55);
      object-fit: cover;
      object-position: center;
      background:
        radial-gradient(circle at 28% 22%, rgba(255, 255, 255, 0.26) 0%, transparent 54%),
        linear-gradient(135deg, rgba(9, 35, 96, 0.9), rgba(4, 21, 61, 0.92));
      filter: saturate(1.05) contrast(1.05);
      transition: transform var(--transition), filter var(--transition);
    }

    .portrait-frame:hover .hero__portrait,
    .portrait-frame:focus-within .hero__portrait {
      transform: translateY(-6px);
      filter: saturate(1.12) contrast(1.08);
    }

    .card {
      background: var(--card-bg);
      border: 1px solid var(--card-border);
      border-radius: 24px;
      padding: clamp(1.8rem, 3vw, 2.25rem);
      backdrop-filter: blur(18px);
      box-shadow: var(--shadow-soft);
      transition: transform var(--transition), box-shadow var(--transition);
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: var(--shadow-lift);
    }

    .grid {
      display: grid;
      gap: clamp(1.5rem, 3vw, 2.5rem);
    }

    .grid--two {
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    }

    h2 {
      font-size: clamp(1.7rem, 3vw, 2.25rem);
      margin: 0 0 1.6rem;
      color: var(--accent-cyan);
    }

    h3 {
      margin: 0 0 1rem;
      font-size: clamp(1.1rem, 2vw, 1.35rem);
    }

    p {
      margin: 0 0 1rem;
      line-height: 1.7;
    }

    ul {
      margin: 0;
      padding-left: 1.4rem;
    }

    ul li {
      margin-bottom: 0.65rem;
      line-height: 1.65;
    }

    .tag {
      display: inline-flex;
      align-items: center;
      gap: 0.35rem;
      padding: 0.45rem 0.85rem;
      margin: 0 0.55rem 0.6rem 0;
      border-radius: 999px;
      background: rgba(180, 213, 255, 0.14);
      color: rgba(237, 245, 255, 0.92);
      font-size: 0.88rem;
      font-weight: 500;
      letter-spacing: 0.01em;
      transition: background-color var(--transition);
    }

    .tag:hover {
      background: rgba(180, 213, 255, 0.25);
    }

    .experience__item + .experience__item {
      margin-top: 1.75rem;
      padding-top: 1.75rem;
      border-top: 1px solid rgba(160, 205, 255, 0.18);
    }

    .experience__role {
      font-weight: 600;
      font-size: 1.05rem;
      color: var(--accent-gold);
    }

    .experience__meta {
      display: flex;
      flex-wrap: wrap;
      gap: 0.8rem;
      margin: 0.6rem 0 1rem;
      color: var(--text-muted);
      font-size: 0.95rem;
    }

    .course-overview {
      display: grid;
      gap: clamp(2rem, 4.5vw, 3rem);
    }

    .lesson {
      background: rgba(5, 28, 96, 0.62);
      border: 1px solid rgba(112, 181, 254, 0.28);
      border-radius: 18px;
      padding: 1.35rem;
      display: grid;
      gap: 0.95rem;
      transition: transform var(--transition), box-shadow var(--transition), border-color var(--transition);
    }

    .lesson:hover,
    .lesson:focus-within {
      transform: translateY(-4px);
      box-shadow: 0 26px 45px rgba(5, 55, 135, 0.42);
      border-color: rgba(171, 219, 255, 0.45);
    }
    
    label.lesson {
      cursor: pointer;
    }

    .lesson__header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .lesson__header h4 {
      margin: 0;
      font-size: 1.05rem;
      line-height: 1.35;
      color: var(--accent-cyan);
    }

    .lesson__status {
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      font-size: 0.92rem;
      color: var(--accent-cyan);
      font-weight: 600;
    }

    .lesson-checkbox {
      width: 1.05rem;
      height: 1.05rem;
      accent-color: var(--accent-cyan);
    }

    .progress-bar {
      position: relative;
      width: 100%;
      height: 10px;
      border-radius: 999px;
      overflow: hidden;
      background: rgba(255, 255, 255, 0.16);
      box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.2);
    }

    .progress-bar span {
      position: absolute;
      inset: 0;
      width: 0%;
      border-radius: inherit;
      background: linear-gradient(90deg, #6bdcff 0%, #c0e7ff 100%);
      transition: width 0.45s ease-in-out;
      box-shadow: 0 0 10px rgba(107, 220, 255, 0.5);
    }

    .course-footer {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      align-items: center;
      justify-content: space-between;
      background: rgba(9, 46, 110, 0.7);
      border: 1px solid rgba(134, 197, 255, 0.24);
      border-radius: 18px;
      padding: 1.5rem;
      color: var(--text-muted);
      backdrop-filter: blur(10px);
    }

    .contact-card {
      display: grid;
      gap: 1.2rem;
    }

    .contact-list {
      list-style: none;
      margin: 0;
      padding: 0;
      display: grid;
      gap: 0.9rem;
    }

    .contact-list li {
      display: flex;
      flex-wrap: wrap;
      gap: 0.65rem;
      align-items: center;
      padding: 0.95rem 1.1rem;
      border-radius: 14px;
      background: rgba(255, 255, 255, 0.14);
      color: rgba(237, 245, 255, 0.9);
      transition: background-color var(--transition);
    }

    .contact-list li:hover {
      background: rgba(255, 255, 255, 0.2);
    }

    .contact-list span {
      font-weight: 600;
      color: #ffffff;
    }

    footer {
      padding: 2.5rem 0 3rem;
      text-align: center;
      color: var(--text-muted);
      font-size: 0.92rem;
      background: rgba(0, 0, 0, 0.2);
      backdrop-filter: blur(10px);
    }

    footer a {
      color: var(--accent-cyan);
      font-weight: 600;
    }

    .project-card {
      background: rgba(5, 28, 96, 0.62);
      border: 1px solid rgba(112, 181, 254, 0.28);
      border-radius: 18px;
      padding: 1.35rem;
      display: grid;
      gap: 0.95rem;
      transition: transform var(--transition), box-shadow var(--transition), border-color var(--transition);
    }

    .project-card:hover,
    .project-card:focus-within {
      transform: translateY(-4px);
      box-shadow: 0 26px 45px rgba(5, 55, 135, 0.42);
      border-color: rgba(171, 219, 255, 0.45);
    }

    .project-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      margin-bottom: 1.5rem;
      flex-wrap: wrap;
      gap: 1rem;
    }

    .project-content {
      display: grid;
      grid-template-columns: 200px 1fr;
      gap: 2rem;
      margin-bottom: 1.5rem;
    }

    .project-image {
      display: flex;
      justify-content: center;
    }

    .project-portrait {
      width: 180px;
      height: 240px;
      object-fit: cover;
      border-radius: 16px;
      border: 2px solid var(--card-border);
      box-shadow: var(--shadow-soft);
    }

    .project-description h4 {
      margin-top: 1.5rem;
      margin-bottom: 0.8rem;
      color: var(--accent-gold);
    }

    .project-cta {
      margin-top: 1.5rem;
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
    }

    .project-footer {
      display: flex;
      justify-content: space-between;
      color: var(--text-muted);
      font-size: 0.9rem;
      padding-top: 1rem;
      border-top: 1px solid var(--card-border);
    }

    .report-container {
      width: 100%;
      margin-top: 1.5rem;
      border-radius: 12px;
      overflow: hidden;
      background: rgba(0, 0, 0, 0.2);
      border: 1px solid var(--card-border);
    }

    .report-tabs {
      display: flex;
      background: rgba(0, 0, 0, 0.3);
      border-bottom: 1px solid var(--card-border);
    }

    .report-tab {
      flex: 1;
      padding: 0.8rem 1rem;
      background: none;
      border: none;
      color: var(--text-muted);
      cursor: pointer;
      transition: all var(--transition);
      font-weight: 500;
      font-size: 0.9rem;
    }

    .report-tab.active {
      background: rgba(107, 220, 255, 0.1);
      color: var(--accent-cyan);
      border-bottom: 2px solid var(--accent-cyan);
    }

    .report-tab:hover {
      background: rgba(107, 220, 255, 0.05);
    }

    .report-content {
      padding: 1.5rem;
      min-height: 400px;
      max-height: 600px;
      overflow-y: auto;
    }

    .report-text {
      line-height: 1.8;
      color: var(--text-light);
    }

    .report-text h3 {
      color: var(--accent-gold);
      margin-top: 1.5rem;
      margin-bottom: 0.8rem;
    }

    .report-text p {
      margin-bottom: 1rem;
    }

    .report-text ul {
      margin: 1rem 0;
    }

    .report-text li {
      margin-bottom: 0.5rem;
    }

    .access-badge {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.4rem 0.8rem;
      border-radius: 20px;
      background: rgba(76, 175, 80, 0.2);
      color: #4caf50;
      font-size: 0.85rem;
      font-weight: 500;
      margin-left: 0.5rem;
    }

    .pdf-button {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.75rem 1.5rem;
      border-radius: 8px;
      font-weight: 500;
      transition: all var(--transition);
      cursor: pointer;
      border: none;
      font-size: 0.9rem;
      text-decoration: none;
    }

    .pdf-button-primary {
      background: linear-gradient(135deg, #6bdcff 0%, #4aa8ff 100%);
      color: #01203f;
    }

    .pdf-button-secondary {
      background: rgba(255, 255, 255, 0.1);
      color: var(--text-light);
      border: 1px solid rgba(255, 255, 255, 0.2);
    }

    .pdf-button:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    .error-message {
      background: rgba(244, 67, 54, 0.1);
      border: 1px solid rgba(244, 67, 54, 0.3);
      border-radius: 8px;
      padding: 1rem;
      color: #ff9800;
      margin-top: 1rem;
      font-size: 0.9rem;
    }

    .downloads-section {
      margin-top: 3rem;
    }

    .download-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 2rem;
      margin-top: 2rem;
    }

    .download-card {
      background: var(--card-bg);
      border: 1px solid var(--card-border);
      border-radius: 20px;
      padding: 2rem;
      backdrop-filter: blur(18px);
      box-shadow: var(--shadow-soft);
      transition: transform var(--transition), box-shadow var(--transition);
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }

    .download-card:hover {
      transform: translateY(-5px);
      box-shadow: var(--shadow-lift);
    }

    .download-icon {
      font-size: 3rem;
      margin-bottom: 1.5rem;
      color: var(--accent-cyan);
    }

    .download-title {
      font-size: 1.3rem;
      margin-bottom: 1rem;
      color: var(--accent-gold);
    }

    .download-description {
      margin-bottom: 1.5rem;
      color: var(--text-muted);
      line-height: 1.6;
    }

    @media (max-width: 760px) {
      .nav__toggle {
        display: inline-flex;
      }

      .nav__links {
        position: absolute;
        right: 4%;
        top: calc(100% + 0.75rem);
        flex-direction: column;
        align-items: flex-start;
        width: min(280px, 92vw);
        padding: 1.2rem;
        background: rgba(5, 24, 70, 0.94);
        border-radius: 18px;
        border: 1px solid rgba(140, 197, 255, 0.28);
        box-shadow: var(--shadow-lift);
        opacity: 0;
        visibility: hidden;
        transform: translateY(-10px);
        transition: opacity var(--transition), transform var(--transition), visibility var(--transition);
      }

      .nav__links.show {
        opacity: 1;
        visibility: visible;
        transform: translateY(0);
      }

      .nav__links a {
        width: 100%;
        justify-content: space-between;
      }

      .project-content {
        grid-template-columns: 1fr;
        gap: 1.5rem;
      }

      .report-tabs {
        flex-direction: column;
      }

      .download-grid {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>
  <header>
    <nav class="nav">
      <a href="#" class="nav__brand">Ftalew Dagnaw</a>
      <button class="nav__toggle" aria-label="Toggle navigation">
        <span>☰</span>
      </button>
      <ul class="nav__links">
        <li><a href="#about">About</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#course">Course Overview</a></li>
        <li><a href="#downloads">Downloads</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="section" id="hero">
      <div class="container">
        <div class="hero">
          <div class="hero__text">
            <span class="hero__eyebrow">Senior Monitoring & Evaluation Advisor</span>
            <h1>Ftalew Dagnaw Gebreyesus</h1>
            <p>Specializing in health information systems, data analytics, and data-driven public health outcomes with extensive experience in monitoring and evaluation, health informatics, and capacity building.</p>
            <a href="#contact" class="hero__cta">Get in Touch</a>
          </div>
          <div class="hero__image">
            <div class="portrait-frame">
              <img src="https://github.com/ftalew211/My-repository2/blob/main/Ftalew%20Picture.png?raw=true" alt="Ftalew Dagnaw" class="hero__portrait" />
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="about">
      <div class="container">
        <div class="card">
          <h2>About Me</h2>
          <p>I am a dedicated public health professional with over 15 years of experience in monitoring and evaluation, health information systems, and data analytics. My expertise lies in designing and implementing M&E frameworks, conducting data analysis, and utilizing health informatics to improve public health outcomes.</p>
          <p>Throughout my career, I have worked with various international organizations, government agencies, and NGOs to strengthen health systems and improve data quality and utilization for decision-making.</p>
        </div>
      </div>
    </section>

    <section class="section" id="experience">
      <div class="container">
        <h2>Professional Experience</h2>
        <div class="card">
          <div class="experience__item">
            <div class="experience__role">Senior Monitoring & Evaluation Advisor</div>
            <div class="experience__meta">
              <span>John Snow, Inc. (JSI)</span>
              <span>2021 - Present</span>
            </div>
            <ul>
              <li>Lead the design and implementation of M&E frameworks for large-scale health programs</li>
              <li>Develop data collection tools and systems for tracking program performance</li>
              <li>Provide technical assistance and capacity building to M&E staff and partners</li>
              <li>Conduct data analysis and visualization to inform program decision-making</li>
            </ul>
          </div>
          <div class="experience__item">
            <div class="experience__role">Health Information System Specialist</div>
            <div class="experience__meta">
              <span>World Health Organization (WHO)</span>
              <span>2018 - 2021</span>
            </div>
            <ul>
              <li>Supported the implementation and scale-up of DHIS2 in multiple countries</li>
              <li>Developed training materials and conducted workshops on health data management</li>
              <li>Provided technical support for data quality assessment and improvement</li>
              <li>Collaborated with ministries of health to strengthen health information systems</li>
            </ul>
          </div>
          <div class="experience__item">
            <div class="experience__role">M&E Officer</div>
            <div class="experience__meta">
              <span>Pathfinder International</span>
              <span>2015 - 2018</span>
            </div>
            <ul>
              <li>Managed M&E activities for reproductive health programs</li>
              <li>Conducted routine data quality audits and supported performance reviews</li>
              <li>Prepared M&E reports for donors and stakeholders</li>
              <li>Supported the development of program logframes and M&E plans</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="skills">
      <div class="container">
        <h2>Technical Skills</h2>
        <div class="grid grid--two">
          <div class="card">
            <h3>Data Analysis & Visualization</h3>
            <div>
              <span class="tag">R</span>
              <span class="tag">Python</span>
              <span class="tag">Stata</span>
              <span class="tag">SPSS</span>
              <span class="tag">Tableau</span>
              <span class="tag">Power BI</span>
            </div>
          </div>
          <div class="card">
            <h3>Health Information Systems</h3>
            <div>
              <span class="tag">DHIS2</span>
              <span class="tag">OpenMRS</span>
              <span class="tag">CommCare</span>
              <span class="tag">Kobo Toolbox</span>
              <span class="tag">ODK</span>
            </div>
          </div>
          <div class="card">
            <h3>Monitoring & Evaluation</h3>
            <div>
              <span class="tag">Logical Framework</span>
              <span class="tag">Results Framework</span>
              <span class="tag">Performance Monitoring Plan</span>
              <span class="tag">Data Quality Assessment</span>
              <span class="tag">Evaluation Design</span>
            </div>
          </div>
          <div class="card">
            <h3>Database Management</h3>
            <div>
              <span class="tag">SQL</span>
              <span class="tag">MySQL</span>
              <span class="tag">PostgreSQL</span>
              <span class="tag">Microsoft Access</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="course">
      <div class="container">
        <h2>Data Analytics Course Overview</h2>
        <div class="card">
          <div class="course-overview">
            <label class="lesson">
              <div class="lesson__header">
                <h4>Introduction to Data Analytics</h4>
                <span class="lesson__status">Completed</span>
              </div>
              <p>Foundational concepts of data analytics, including data types, data collection methods, and basic analytical techniques.</p>
              <div class="progress-bar">
                <span style="width: 100%"></span>
              </div>
            </label>
            <label class="lesson">
              <div class="lesson__header">
                <h4>Data Visualization Principles</h4>
                <span class="lesson__status">Completed</span>
              </div>
              <p>Principles of effective data visualization, chart types, and dashboard design for communicating insights.</p>
              <div class="progress-bar">
                <span style="width: 100%"></span>
              </div>
            </label>
            <label class="lesson">
              <div class="lesson__header">
                <h4>Statistical Analysis with R</h4>
                <span class="lesson__status">In Progress</span>
              </div>
              <p>Statistical methods and their implementation in R, including hypothesis testing, regression analysis, and ANOVA.</p>
              <div class="progress-bar">
                <span style="width: 75%"></span>
              </div>
            </label>
            <label class="lesson">
              <div class="lesson__header">
                <h4>Database Management & SQL</h4>
                <span class="lesson__status">Upcoming</span>
              </div>
              <p>Database design, management, and querying using SQL for efficient data retrieval and manipulation.</p>
              <div class="progress-bar">
                <span style="width: 0%"></span>
              </div>
            </label>
          </div>
          <div class="course-footer">
            <div>Overall Progress: <strong>68%</strong></div>
            <div>Estimated Completion: <strong>December 2023</strong></div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="downloads">
      <div class="container">
        <h2>Research & Reports</h2>
        <div class="download-grid">
          <div class="download-card">
            <div class="download-icon">📊</div>
            <h3 class="download-title">Job Market Data Analysis</h3>
            <p class="download-description">Comprehensive analysis of job market trends, employment patterns, and workforce dynamics based on recent data.</p>
            <a href="https://github.com/ftalew211/My-repository2/raw/main/Job%20market%20%20analysis%20report.pdf" class="pdf-button pdf-button-primary" download>
              Download PDF
            </a>
          </div>
          <div class="download-card">
            <div class="download-icon">📈</div>
            <h3 class="download-title">GDP vs Life Expectancy Analysis</h3>
            <p class="download-description">Statistical analysis exploring the relationship between GDP per capita and life expectancy across different countries.</p>
            <a href="https://github.com/ftalew211/My-repository2/raw/main/relationship%20between%20GDP%20per%20capita%20and%20life%20expectancy_by_Ftalew_Dagnaw.pdf" class="pdf-button pdf-button-primary" download>
              Download PDF
            </a>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="contact">
      <div class="container">
        <h2>Contact Information</h2>
        <div class="grid grid--two">
          <div class="card contact-card">
            <h3>Get in Touch</h3>
            <p>Feel free to reach out for collaborations, consultations, or any inquiries regarding my work in monitoring and evaluation, health information systems, or data analytics.</p>
            <ul class="contact-list">
              <li>
                <span>Email:</span>
                <a href="mailto:ftalew.dagnaw@example.com">ftalew.dagnaw@example.com</a>
              </li>
              <li>
                <span>Phone:</span>
                <a href="tel:+1234567890">+1 (234) 567-890</a>
              </li>
              <li>
                <span>LinkedIn:</span>
                <a href="https://linkedin.com/in/ftalew-dagnaw" target="_blank">linkedin.com/in/ftalew-dagnaw</a>
              </li>
              <li>
                <span>GitHub:</span>
                <a href="https://github.com/ftalew211" target="_blank">github.com/ftalew211</a>
              </li>
            </ul>
          </div>
          <div class="card">
            <h3>Professional Affiliations</h3>
            <ul>
              <li>American Public Health Association (APHA)</li>
              <li>International Society for Disease Surveillance (ISDS)</li>
              <li>Global Evaluation Initiative (GEI)</li>
              <li>Digital Health and Interoperability Working Group</li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>&copy; 2023 Ftalew Dagnaw Gebreyesus. All rights reserved.</p>
      <p>Designed with a focus on accessibility and user experience.</p>
    </div>
  </footer>

  <script>
    // Mobile navigation toggle
    document.querySelector('.nav__toggle').addEventListener('click', function() {
      document.querySelector('.nav__links').classList.toggle('show');
    });

    // Close mobile menu when clicking outside
    document.addEventListener('click', function(event) {
      const nav = document.querySelector('.nav');
      const isClickInsideNav = nav.contains(event.target);
      
      if (!isClickInsideNav) {
        document.querySelector('.nav__links').classList.remove('show');
      }
    });

    // Smooth scrolling for navigation links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        
        const targetId = this.getAttribute('href');
        if (targetId === '#') return;
        
        const targetElement = document.querySelector(targetId);
        if (targetElement) {
          window.scrollTo({
            top: targetElement.offsetTop - 100,
            behavior: 'smooth'
          });
          
          // Close mobile menu after clicking a link
          document.querySelector('.nav__links').classList.remove('show');
        }
      });
    });
  </script>
</body>
</html>
