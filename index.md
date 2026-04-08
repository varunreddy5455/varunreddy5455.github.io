---
layout: default
title: Varun Reddy
---

<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');

  .page-header {
    display: none;
  }

  *, *::before, *::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  html {
    scroll-behavior: smooth;
  }

  body {
    background: #000000;
    color: #e0e0e0;
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    overflow-x: hidden;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  body, body * {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  }

  ::selection {
    background: rgba(255, 255, 255, 0.15);
    color: #ffffff;
  }

  .bg-grid {
    position: fixed;
    top: 0; left: 0; right: 0; bottom: 0;
    z-index: 0;
    pointer-events: none;
    background-image:
      linear-gradient(rgba(255,255,255,0.02) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255,255,255,0.02) 1px, transparent 1px);
    background-size: 60px 60px;
    mask-image: radial-gradient(ellipse at 50% 0%, black 0%, transparent 70%);
    -webkit-mask-image: radial-gradient(ellipse at 50% 0%, black 0%, transparent 70%);
  }

  .bg-glow {
    position: fixed;
    top: -200px;
    left: 50%;
    transform: translateX(-50%);
    width: 800px;
    height: 600px;
    background: radial-gradient(ellipse, rgba(255,255,255,0.03) 0%, transparent 70%);
    z-index: 0;
    pointer-events: none;
  }

  /* ---- Top Bar ---- */
  .top-bar {
    position: fixed;
    top: 0; left: 0; right: 0;
    z-index: 1000;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 16px;
    padding: 14px 24px;
    background: rgba(0, 0, 0, 0.7);
    border-bottom: 1px solid rgba(255, 255, 255, 0.06);
    backdrop-filter: blur(20px) saturate(180%);
    -webkit-backdrop-filter: blur(20px) saturate(180%);
    transition: background 0.3s ease;
  }

  .brand {
    color: #ffffff;
    font-weight: 600;
    font-size: 1rem;
    letter-spacing: -0.01em;
    position: relative;
    padding: 6px 0;
  }

  .brand::after {
    content: '';
    position: absolute;
    bottom: 2px;
    left: 0;
    width: 100%;
    height: 1px;
    background: linear-gradient(90deg, rgba(255,255,255,0.4), transparent);
    opacity: 0;
    transition: opacity 0.3s ease;
  }

  .brand:hover::after {
    opacity: 1;
  }

  .top-nav {
    display: flex;
    align-items: center;
    gap: 6px;
    flex-wrap: wrap;
    justify-content: flex-end;
  }

  .top-link {
    text-decoration: none;
    color: rgba(255, 255, 255, 0.5);
    border-radius: 8px;
    padding: 8px 16px;
    font-size: 0.875rem;
    font-weight: 500;
    transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
    position: relative;
    letter-spacing: -0.005em;
  }

  .top-link:hover {
    color: rgba(255, 255, 255, 0.9);
    background: rgba(255, 255, 255, 0.06);
  }

  .top-link.active {
    color: #ffffff;
    background: rgba(255, 255, 255, 0.1);
  }

  /* ---- Main Content ---- */
  .main-content {
    max-width: 720px;
    margin: 0 auto;
    padding: 120px 24px 100px;
    position: relative;
    z-index: 1;
  }

  .ai-profile {
    color: #d4d4d4;
  }

  .ai-profile a {
    color: #ffffff;
    text-decoration: none;
    border-bottom: 1px solid rgba(255, 255, 255, 0.2);
    transition: border-color 0.25s ease, color 0.25s ease;
  }

  .ai-profile a:hover {
    color: #ffffff;
    border-bottom-color: rgba(255, 255, 255, 0.6);
  }

  /* ---- Section Blocks ---- */
  .section-block {
    scroll-margin-top: 96px;
    display: none;
  }

  .section-block.active {
    display: block;
    animation: fadeReveal 0.5s cubic-bezier(0.4, 0, 0.2, 1) forwards;
  }

  @keyframes fadeReveal {
    0% { opacity: 0; transform: translateY(12px); }
    100% { opacity: 1; transform: translateY(0); }
  }

  .section-title {
    margin: 0 0 40px;
    font-size: 0.75rem;
    font-weight: 600;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: rgba(255, 255, 255, 0.35);
    position: relative;
    padding-bottom: 16px;
  }

  .section-title::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 32px;
    height: 1px;
    background: rgba(255, 255, 255, 0.2);
  }

  /* ---- Profile Header ---- */
  .profile-header {
    display: flex;
    align-items: flex-start;
    gap: 24px;
    margin-bottom: 32px;
    animation: fadeReveal 0.6s cubic-bezier(0.4, 0, 0.2, 1) 0.1s both;
  }

  .profile-image-wrap {
    position: relative;
    flex-shrink: 0;
  }

  .profile-image-wrap::before {
    content: '';
    position: absolute;
    inset: -3px;
    border-radius: 50%;
    background: linear-gradient(135deg, rgba(255,255,255,0.15), rgba(255,255,255,0.03));
    z-index: -1;
  }

  .profile-image {
    border-radius: 50%;
    object-fit: cover;
    width: 88px;
    height: 88px;
    border: 2px solid rgba(255, 255, 255, 0.08);
    filter: grayscale(20%);
    transition: filter 0.4s ease;
  }

  .profile-image:hover {
    filter: grayscale(0%);
  }

  .profile-text {
    padding-top: 4px;
  }

  .profile-name {
    font-size: 1.5rem;
    font-weight: 700;
    color: #ffffff;
    margin: 0 0 6px;
    letter-spacing: -0.025em;
    line-height: 1.2;
  }

  .role {
    margin: 0;
    font-size: 0.95rem;
    font-weight: 400;
    color: rgba(255, 255, 255, 0.5);
    line-height: 1.5;
  }

  .role strong {
    color: rgba(255, 255, 255, 0.7);
    font-weight: 500;
  }

  .tagline {
    margin: 12px 0 0;
    line-height: 1.7;
    color: rgba(255, 255, 255, 0.55);
    font-size: 0.95rem;
  }

  .tagline strong {
    color: rgba(255, 255, 255, 0.8);
    font-weight: 500;
  }

  /* ---- Bio ---- */
  .bio {
    margin: 0 0 24px;
    line-height: 1.8;
    color: rgba(255, 255, 255, 0.6);
    font-size: 0.95rem;
    animation: fadeReveal 0.6s cubic-bezier(0.4, 0, 0.2, 1) 0.2s both;
  }

  .contact {
    margin: 0 0 48px;
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
    animation: fadeReveal 0.6s cubic-bezier(0.4, 0, 0.2, 1) 0.3s both;
  }

  .contact-link {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    color: rgba(255, 255, 255, 0.5) !important;
    font-size: 0.875rem;
    padding: 8px 16px;
    border: 1px solid rgba(255, 255, 255, 0.08) !important;
    border-radius: 8px;
    border-bottom: 1px solid rgba(255, 255, 255, 0.08) !important;
    transition: all 0.25s ease !important;
    background: rgba(255, 255, 255, 0.02);
  }

  .contact-link:hover {
    color: #ffffff !important;
    background: rgba(255, 255, 255, 0.06) !important;
    border-color: rgba(255, 255, 255, 0.15) !important;
  }

  .divider {
    width: 100%;
    height: 1px;
    background: rgba(255, 255, 255, 0.06);
    margin: 8px 0 40px;
    border: none;
  }

  /* ---- Subheading ---- */
  .subheading {
    font-size: 0.875rem;
    font-weight: 600;
    color: rgba(255, 255, 255, 0.8);
    margin: 0 0 20px;
    letter-spacing: -0.005em;
  }

  /* ---- News Items ---- */
  .ai-profile ul {
    list-style: none;
    margin: 0 0 40px;
    padding: 0;
  }

  .ai-profile li {
    margin-bottom: 0;
    padding: 16px 20px;
    font-size: 0.9rem;
    line-height: 1.75;
    color: rgba(255, 255, 255, 0.55);
    border-left: 1px solid rgba(255, 255, 255, 0.06);
    transition: all 0.3s ease;
    position: relative;
  }

  .ai-profile li::before {
    content: '';
    position: absolute;
    left: -1px;
    top: 0;
    width: 1px;
    height: 100%;
    background: rgba(255, 255, 255, 0.3);
    transform: scaleY(0);
    transition: transform 0.3s ease;
    transform-origin: top;
  }

  .ai-profile li:hover {
    color: rgba(255, 255, 255, 0.75);
    background: rgba(255, 255, 255, 0.02);
  }

  .ai-profile li:hover::before {
    transform: scaleY(1);
  }

  /* ---- Experience Entries ---- */
  .entry {
    margin: 0 0 0;
    line-height: 1.8;
    font-size: 0.925rem;
    color: rgba(255, 255, 255, 0.55);
  }

  .entry strong {
    color: #ffffff;
    font-weight: 600;
    font-size: 0.95rem;
  }

  .entry em {
    color: rgba(255, 255, 255, 0.3);
    font-style: normal;
    font-size: 0.85rem;
  }

  .entry-card {
    padding: 24px;
    border: 1px solid rgba(255, 255, 255, 0.05);
    border-radius: 12px;
    background: rgba(255, 255, 255, 0.02);
    margin-bottom: 16px;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  }

  .entry-card:hover {
    background: rgba(255, 255, 255, 0.04);
    border-color: rgba(255, 255, 255, 0.1);
  }

  /* ---- Role Cards ---- */
  .roles-list {
    display: grid;
    gap: 12px;
  }

  .role-card {
    border: 1px solid rgba(255, 255, 255, 0.06);
    border-radius: 12px;
    padding: 20px 24px;
    background: rgba(255, 255, 255, 0.02);
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    position: relative;
    overflow: hidden;
  }

  .role-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(135deg, rgba(255,255,255,0.03), transparent);
    opacity: 0;
    transition: opacity 0.3s ease;
  }

  .role-card:hover {
    border-color: rgba(255, 255, 255, 0.12);
    transform: translateY(-1px);
  }

  .role-card:hover::before {
    opacity: 1;
  }

  .role-card-title {
    margin: 0 0 6px;
    font-size: 0.925rem;
    line-height: 1.5;
    position: relative;
    z-index: 1;
  }

  .role-card-title a {
    color: #ffffff !important;
    border-bottom: none !important;
    font-weight: 500;
  }

  .role-card-title a:hover {
    border-bottom: 1px solid rgba(255, 255, 255, 0.3) !important;
  }

  .role-location {
    margin: 0;
    color: rgba(255, 255, 255, 0.35);
    font-size: 0.85rem;
    position: relative;
    z-index: 1;
  }

  .role-location-icon {
    display: inline-block;
    margin-right: 4px;
    opacity: 0.5;
  }

  /* ---- Stagger animations for child elements ---- */
  .section-block.active .entry-card:nth-child(1) { animation: fadeReveal 0.4s ease 0.05s both; }
  .section-block.active .entry-card:nth-child(2) { animation: fadeReveal 0.4s ease 0.1s both; }
  .section-block.active .entry-card:nth-child(3) { animation: fadeReveal 0.4s ease 0.15s both; }
  .section-block.active .entry-card:nth-child(4) { animation: fadeReveal 0.4s ease 0.2s both; }
  .section-block.active .entry-card:nth-child(5) { animation: fadeReveal 0.4s ease 0.25s both; }
  .section-block.active .entry-card:nth-child(6) { animation: fadeReveal 0.4s ease 0.3s both; }

  .section-block.active .role-card:nth-child(1) { animation: fadeReveal 0.4s ease 0.05s both; }
  .section-block.active .role-card:nth-child(2) { animation: fadeReveal 0.4s ease 0.1s both; }
  .section-block.active .role-card:nth-child(3) { animation: fadeReveal 0.4s ease 0.15s both; }
  .section-block.active .role-card:nth-child(4) { animation: fadeReveal 0.4s ease 0.2s both; }
  .section-block.active .role-card:nth-child(5) { animation: fadeReveal 0.4s ease 0.25s both; }

  .section-block.active li:nth-child(1) { animation: fadeReveal 0.4s ease 0.05s both; }
  .section-block.active li:nth-child(2) { animation: fadeReveal 0.4s ease 0.1s both; }
  .section-block.active li:nth-child(3) { animation: fadeReveal 0.4s ease 0.15s both; }
  .section-block.active li:nth-child(4) { animation: fadeReveal 0.4s ease 0.2s both; }
  .section-block.active li:nth-child(5) { animation: fadeReveal 0.4s ease 0.25s both; }

  /* ---- AI Cursor blink ---- */
  .cursor-blink {
    display: inline-block;
    width: 2px;
    height: 1em;
    background: rgba(255, 255, 255, 0.6);
    margin-left: 4px;
    vertical-align: text-bottom;
    animation: blink 1s steps(1) infinite;
  }

  @keyframes blink {
    0%, 50% { opacity: 1; }
    51%, 100% { opacity: 0; }
  }

  /* ---- Status indicator ---- */
  .status-dot {
    display: inline-block;
    width: 6px;
    height: 6px;
    background: rgba(255, 255, 255, 0.4);
    border-radius: 50%;
    margin-right: 8px;
    animation: pulse 2s ease-in-out infinite;
  }

  @keyframes pulse {
    0%, 100% { opacity: 0.4; }
    50% { opacity: 1; }
  }

  /* ---- Footer ---- */
  .site-footer {
    text-align: center;
    padding: 48px 24px;
    color: rgba(255, 255, 255, 0.2);
    font-size: 0.8rem;
    position: relative;
    z-index: 1;
  }

  .site-footer::before {
    content: '';
    display: block;
    width: 40px;
    height: 1px;
    background: rgba(255, 255, 255, 0.06);
    margin: 0 auto 24px;
  }

  /* ---- Responsive ---- */
  @media (max-width: 640px) {
    .top-bar {
      padding: 12px 16px;
    }

    .brand {
      font-size: 0.9rem;
    }

    .top-link {
      font-size: 0.8rem;
      padding: 6px 12px;
    }

    .main-content {
      padding: 100px 16px 64px;
    }

    .profile-header {
      gap: 16px;
    }

    .profile-image {
      width: 64px;
      height: 64px;
    }

    .profile-name {
      font-size: 1.25rem;
    }

    .entry-card {
      padding: 18px;
    }

    .role-card {
      padding: 16px 18px;
    }
  }

  /* ---- Scrollbar ---- */
  ::-webkit-scrollbar {
    width: 6px;
  }

  ::-webkit-scrollbar-track {
    background: #000000;
  }

  ::-webkit-scrollbar-thumb {
    background: rgba(255, 255, 255, 0.1);
    border-radius: 3px;
  }

  ::-webkit-scrollbar-thumb:hover {
    background: rgba(255, 255, 255, 0.2);
  }
</style>

<div class="bg-grid"></div>
<div class="bg-glow"></div>

<header class="top-bar" aria-label="Primary navigation">
  <div class="brand">Varun Reddy</div>
  <nav class="top-nav">
    <a class="top-link active" href="#about-section" data-section="about-section">About</a>
    <a class="top-link" href="#experience-section" data-section="experience-section">Experience</a>
    <a class="top-link" href="#education-section" data-section="education-section">Education</a>
    <a class="top-link" href="#roles-section" data-section="roles-section">Open Roles</a>
  </nav>
</header>

<div class="ai-profile">
  <section id="about-section" class="section-block active" aria-label="About">
    <h2 class="section-title">About</h2>

    <div class="profile-header">
      <div class="profile-image-wrap">
        <img src="profile.jpg" alt="Varun Reddy" class="profile-image" />
      </div>
      <div class="profile-text">
        <p class="profile-name">Varun Reddy</p>
        <p class="role">
          Technical Sourcer @
          <a href="https://www.youtube.com/watch?v=7T7SyMZihwo" target="_blank"><strong>Datadog</strong></a>
        </p>
        <p class="tagline">
          Sourcing exceptional <strong>AI Research</strong> and <strong>Applied AI</strong> talent in Paris and New York.
        </p>
      </div>
    </div>

    <p class="bio">
      I hold a master's degree in Human Resource Management from Trinity College Dublin and a bachelor's degree in Urban Planning from SPA Bhopal. Recipient of the Trinity Business School Scholarship and the Proficiency Gold Medal in recognition of academic merit.
    </p>

    <div class="contact">
      <a href="mailto:varunreddy5455@gmail.com" class="contact-link">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
        Email
      </a>
      <a href="https://www.linkedin.com/in/varun-m-r/" target="_blank" class="contact-link">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
        LinkedIn
      </a>
    </div>

    <hr class="divider" />

    <h3 class="subheading"><span class="status-dot"></span>Latest News</h3>
    <ul>
      <li>
        We're introducing fine-tuning and exogenous covariate support for Toto, enabling teams to adapt the model to their own data and incorporate known future signals to produce more accurate time-series forecasts.
      </li>
      <li>
        We unveiled the first two launches (open source under the Apache 2.0 license) from Datadog AI Research!
        <a href="https://huggingface.co/Datadog/Toto-Open-Base-1.0" target="_blank">Toto</a>, a new SOTA time series foundation model, and
        <a href="https://huggingface.co/datasets/Datadog/BOOM" target="_blank">BOOM</a>, the largest benchmark of observability metrics.
      </li>
      <li>
        We are expanding our AI Research team in Paris! Check out our open
        <a href="https://careers.datadoghq.com/detail/6652564/?gh_jid=6652564" target="_blank">AI Researcher role</a>.
      </li>
      <li>
        <a href="https://www.datadoghq.com/blog/datadog-time-series-foundation-model/" target="_blank">Introducing Toto</a>:
        A state-of-the-art time series foundation model by Datadog.
      </li>
      <li>
        Want to work on exciting topics like
        <a href="https://www.datadoghq.com/blog/watchdog/" target="_blank">anomaly detection</a>,
        <a href="https://docs.datadoghq.com/logs/explorer/watchdog_insights/" target="_blank">error outliers</a>,
        and
        <a href="https://www.datadoghq.com/blog/faulty-deployment-detection/" target="_blank">faulty deployment analysis</a>?
        Check out our open
        <a href="https://careers.datadoghq.com/detail/6781197/?gh_jid=6781197" target="_blank">Senior Applied Scientist role</a> in Paris.
      </li>
    </ul>

    <h3 class="subheading">Fun facts</h3>
    <ul>
      <li>I'm a trained Carnatic classical singer.</li>
      <li>I ran a YouTube channel called <a href="https://www.youtube.com/@AllAboutPlanning" target="_blank">All About Planning</a> where I shared content related to urban planning.</li>
    </ul>
  </section>

  <section id="experience-section" class="section-block" aria-label="Experience">
    <h2 class="section-title">Experience</h2>

    <div class="entry-card">
      <p class="entry"><strong>Datadog</strong><br>
      Senior Technical Sourcer (AI Research and Applied AI) <em>Apr 2026 – Present</em><br>
      Technical Sourcer II (AI Research and Applied AI) <em>Apr 2024 – April 2026</em></p>
    </div>

    <div class="entry-card">
      <p class="entry"><strong>Azon Recruitment Group</strong><br>
      Principal IT Recruitment Consultant <em>Sep 2022 – Apr 2024</em><br>
      Senior IT Recruitment Consultant <em>Mar 2022 – Sep 2022</em><br>
      IT Recruitment Consultant <em>May 2021 – Mar 2022</em></p>
    </div>

    <div class="entry-card">
      <p class="entry"><strong>Next Generation Recruitment</strong><br>
      IT Recruitment Associate <em>Nov 2019 – May 2021</em></p>
    </div>

    <div class="entry-card">
      <p class="entry"><strong>Temple Recruitment</strong><br>
      Recruitment Consultant <em>Aug 2019 – Nov 2019</em></p>
    </div>
  </section>

  <section id="education-section" class="section-block" aria-label="Education and awards">
    <h2 class="section-title">Education & Awards</h2>

    <h3 class="subheading">Education</h3>

    <div class="entry-card">
      <p class="entry"><strong>Trinity College Dublin</strong><br>
      Master's Degree, Human Resource Management <em>2018 – 2019</em></p>
    </div>

    <div class="entry-card">
      <p class="entry"><strong>School of Planning and Architecture, Bhopal</strong><br>
      Bachelor's Degree, Urban Planning <em>2014 – 2018</em></p>
    </div>

    <h3 class="subheading" style="margin-top: 40px;">Honors and Awards</h3>

    <div class="entry-card">
      <p class="entry"><strong>Proficiency Gold Medal for 1st Rank in B. Plan</strong><br>
      Issued by School of Planning and Architecture, Bhopal <em>Oct 2018</em></p>
    </div>

    <div class="entry-card">
      <p class="entry"><strong>Trinity Business School Scholarship 2018/19</strong><br>
      Issued by Trinity Business School <em>Oct 2018</em></p>
    </div>

    <div class="entry-card">
      <p class="entry"><strong>3rd Best Thesis Award</strong><br>
      Issued by Institute of Town Planners, Madhya Pradesh Chapter <em>Aug 2018</em><br>
      Thesis: Assessing and Planning for Airport Induced Land Uses – A Case of Cochin</p>
    </div>

    <div class="entry-card">
      <p class="entry"><strong>South India Zonal Level First Position</strong><br>
      Issued by IT Akshaya Prathiba <em>Feb 2010</em><br>
      IT Competition on Library Database Management using MS Access</p>
    </div>

    <div class="entry-card">
      <p class="entry"><strong>Karnataka State Level 7th Rank</strong><br>
      Issued by 2nd International Level Science Talent Search Examination <em>Aug 2007</em></p>
    </div>
  </section>

  <section id="roles-section" class="section-block" aria-label="Open AI roles at Datadog">
    <h2 class="section-title">Open AI roles at Datadog</h2>

    <div class="roles-list">
      <div class="role-card">
        <p class="role-card-title"><strong><a href="https://careers.datadoghq.com/detail/6652564/?gh_jid=6652564" target="_blank">AI Research Scientist – Datadog AI Research (DAIR)</a></strong></p>
        <p class="role-location"><span class="role-location-icon">&#9679;</span> Paris, France</p>
      </div>

      <div class="role-card">
        <p class="role-card-title"><strong><a href="https://careers.datadoghq.com/detail/7194969/?gh_jid=7194969" target="_blank">AI Research Engineer - Datadog AI Research (DAIR)</a></strong></p>
        <p class="role-location"><span class="role-location-icon">&#9679;</span> Paris, France</p>
      </div>

      <div class="role-card">
        <p class="role-card-title"><strong><a href="https://careers.datadoghq.com/detail/6572669/?gh_jid=6572669" target="_blank">AI Research Scientist – Datadog AI Research (DAIR)</a></strong></p>
        <p class="role-location"><span class="role-location-icon">&#9679;</span> New York, New York, USA</p>
      </div>

      <div class="role-card">
        <p class="role-card-title"><strong><a href="https://careers.datadoghq.com/detail/7183013/?gh_jid=7183013" target="_blank">AI Research Engineer – Datadog AI Research (DAIR)</a></strong></p>
        <p class="role-location"><span class="role-location-icon">&#9679;</span> New York, New York, USA</p>
      </div>

      <div class="role-card">
        <p class="role-card-title"><strong><a href="https://careers.datadoghq.com/detail/6781197/?gh_jid=6781197" target="_blank">Senior Applied Scientist</a></strong></p>
        <p class="role-location"><span class="role-location-icon">&#9679;</span> Paris, France</p>
      </div>
    </div>
  </section>
</div>

<footer class="site-footer">
  <span style="opacity: 0.5;">&copy; 2026 Varun Reddy</span>
</footer>

<script>
  (function () {
    var links = Array.prototype.slice.call(document.querySelectorAll(".top-link"));
    var sections = links
      .map(function (link) {
        return document.getElementById(link.getAttribute("data-section"));
      })
      .filter(Boolean);

    function setActive(id) {
      links.forEach(function (link) {
        link.classList.toggle("active", link.getAttribute("data-section") === id);
      });
      sections.forEach(function (section) {
        if (section.id === id) {
          section.classList.remove("active");
          void section.offsetHeight;
          section.classList.add("active");
        } else {
          section.classList.remove("active");
        }
      });
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    links.forEach(function (link) {
      link.addEventListener("click", function (event) {
        event.preventDefault();
        var targetId = link.getAttribute("data-section");
        setActive(targetId);
      });
    });

    setActive("about-section");
  })();
</script>
