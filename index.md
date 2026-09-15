---
layout: default
title: Varun Reddy
---

# Hey, I’m Varun Reddy 👋

<style>
  :root {
    --bg-0: #f5f5f7;
    --label: #1d1d1f;
    --secondary: rgba(29, 29, 31, 0.64);
    --tertiary: rgba(29, 29, 31, 0.42);
    --fill: rgba(118, 118, 128, 0.12);
    --stroke: rgba(0, 0, 0, 0.08);
    --stroke-strong: rgba(0, 0, 0, 0.14);
    --glass: rgba(255, 255, 255, 0.72);
    --link: #0071e3;
    --shadow: 0 18px 50px rgba(15, 23, 42, 0.08);
    --radius-lg: 24px;
    --radius-md: 16px;
    --radius-sm: 12px;
  }

  #skip-to-content {
    color: var(--label);
  }

  .page-header {
    display: none;
  }

  html {
    color-scheme: light;
    background: var(--bg-0);
  }

  html,
  body {
    min-height: 100%;
    background-color: var(--bg-0) !important;
    background-image:
      radial-gradient(ellipse 110% 62% at 50% -8%, rgba(186, 214, 255, 0.55), transparent 56%),
      radial-gradient(ellipse 48% 38% at 92% 22%, rgba(255, 196, 214, 0.32), transparent 52%),
      radial-gradient(ellipse 46% 34% at 6% 82%, rgba(186, 232, 214, 0.34), transparent 50%),
      linear-gradient(180deg, #fbfbfd 0%, #f5f5f7 38%, #eef1f6 72%, #f5f5f7 100%) !important;
    color: var(--label) !important;
    font-family: -apple-system, BlinkMacSystemFont, "SF Pro Display", "SF Pro Text", "Segoe UI", Helvetica, Arial, sans-serif !important;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  body::before {
    content: "";
    pointer-events: none;
    position: fixed;
    inset: 0;
    background: radial-gradient(circle at 50% 0%, rgba(255, 255, 255, 0.85), transparent 38%);
    mask-image: linear-gradient(180deg, #000 0%, transparent 55%);
    -webkit-mask-image: linear-gradient(180deg, #000 0%, transparent 55%);
    z-index: 0;
  }

  .main-content {
    position: relative;
    z-index: 1;
    max-width: 840px;
    margin: 0 auto;
    padding: 4.5rem 1.5rem 5rem;
    background: transparent !important;
    color: var(--label) !important;
    font-size: 17px;
    line-height: 1.47;
    letter-spacing: -0.022em;
  }

  .main-content h1,
  .main-content h2,
  .main-content h3,
  .main-content h4,
  .main-content h5,
  .main-content h6 {
    color: var(--label) !important;
    font-weight: 600;
    letter-spacing: -0.03em;
  }

  .main-content > h1 {
    margin: 0 0 1.75rem;
    font-size: clamp(40px, 7vw, 56px);
    line-height: 1.05;
    letter-spacing: -0.042em;
    text-align: left;
  }

  .main-content a {
    color: var(--link);
    text-decoration: none;
  }

  .main-content a:hover {
    text-decoration: underline;
  }

  .site-footer {
    position: relative;
    z-index: 1;
    border-top: 1px solid var(--stroke);
    color: var(--tertiary) !important;
    font-size: 13px;
  }

  .site-footer-owner,
  .site-footer-credits,
  .site-footer a {
    color: var(--tertiary) !important;
  }

  .ai-profile {
    background: transparent;
    color: var(--label);
    border: none;
    border-radius: 0;
    padding: 0;
    margin-top: 8px;
    font-family: inherit;
    box-shadow: none;
  }

  .profile-header {
    display: flex;
    align-items: center;
    gap: 24px;
    flex-wrap: wrap;
    margin-bottom: 18px;
  }

  .profile-image {
    border-radius: 50%;
    object-fit: cover;
    width: 140px;
    height: 140px;
    border: 1px solid var(--stroke-strong);
    box-shadow: 0 16px 40px rgba(15, 23, 42, 0.12);
  }

  .profile-text {
    max-width: 650px;
  }

  .role {
    margin: 0;
    font-size: 1.12em;
    letter-spacing: -0.02em;
    color: var(--label);
  }

  .tagline {
    margin: 8px 0 0;
    color: var(--secondary);
  }

  .bio {
    margin: 16px 0;
    line-height: 1.55;
    color: var(--secondary);
  }

  .contact {
    margin: 0 0 8px;
    color: var(--secondary);
  }

  .section-tabs {
    display: flex;
    width: fit-content;
    max-width: 100%;
    gap: 4px;
    flex-wrap: wrap;
    margin: 0 0 28px;
    padding: 4px;
    background: var(--fill);
    border: 1px solid var(--stroke);
    border-radius: 14px;
  }

  .tab-button {
    padding: 8px 14px;
    border-radius: 10px;
    border: 0;
    background: transparent;
    color: var(--label);
    cursor: pointer;
    font: inherit;
    font-size: 14px;
    font-weight: 500;
    letter-spacing: -0.016em;
    transition: background 0.16s ease, box-shadow 0.16s ease, color 0.16s ease;
  }

  .tab-button:hover {
    background: rgba(255, 255, 255, 0.55);
  }

  .tab-button.active {
    background: #ffffff;
    color: var(--label);
    box-shadow: 0 1px 2px rgba(0, 0, 0, 0.06), 0 8px 18px rgba(15, 23, 42, 0.08);
  }

  .tab-panel {
    display: none;
  }

  .tab-panel.active {
    display: block;
  }

  .ai-profile h2 {
    font-size: 21px;
    color: var(--label);
    margin: 36px 0 16px;
    border-left: 0;
    padding-left: 0;
    letter-spacing: -0.03em;
  }

  .ai-profile h2:first-child {
    margin-top: 8px;
  }

  .ai-profile ul {
    list-style: none;
    margin: 0 0 10px;
    padding: 0;
    background: var(--glass);
    backdrop-filter: saturate(180%) blur(28px);
    -webkit-backdrop-filter: saturate(180%) blur(28px);
    border: 1px solid var(--stroke);
    border-radius: var(--radius-lg);
    overflow: hidden;
    box-shadow: var(--shadow);
  }

  .ai-profile li {
    margin: 0;
    padding: 16px 20px;
    line-height: 1.55;
    color: var(--label);
    border-bottom: 1px solid var(--stroke);
  }

  .ai-profile li:last-child {
    border-bottom: 0;
  }

  .entry {
    margin-bottom: 14px;
    line-height: 1.55;
    padding: 18px 20px;
    background: var(--glass);
    backdrop-filter: saturate(180%) blur(28px);
    -webkit-backdrop-filter: saturate(180%) blur(28px);
    border: 1px solid var(--stroke);
    border-radius: var(--radius-md);
    box-shadow: 0 10px 28px rgba(15, 23, 42, 0.05);
    color: var(--secondary);
  }

  .entry strong {
    color: var(--label);
    font-weight: 600;
  }

  .project-card {
    background: var(--glass);
    backdrop-filter: saturate(180%) blur(28px);
    -webkit-backdrop-filter: saturate(180%) blur(28px);
    border: 1px solid var(--stroke);
    border-radius: var(--radius-lg);
    padding: 28px;
    margin: 8px 0 0;
    box-shadow: var(--shadow);
  }

  .project-card .eyebrow {
    margin: 0 0 10px;
    color: var(--tertiary);
    font-size: 13px;
    font-weight: 600;
    letter-spacing: 0.16em;
    text-transform: uppercase;
  }

  .project-card h3 {
    margin: 0 0 12px;
    font-size: 28px;
    letter-spacing: -0.035em;
    line-height: 1.15;
  }

  .project-card h3 a {
    color: var(--label) !important;
  }

  .project-card h3 a:hover {
    color: var(--link) !important;
    text-decoration: none;
  }

  .project-link {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    margin-top: 16px;
    font-size: 15px;
    font-weight: 500;
    letter-spacing: -0.016em;
  }

  .project-blurb {
    margin: 0;
    color: var(--secondary);
    font-size: 17px;
    line-height: 1.5;
    letter-spacing: -0.02em;
  }

  @media (max-width: 640px) {
    .main-content {
      padding: 2.75rem 1.15rem 4rem;
    }

    .section-tabs {
      width: 100%;
    }

    .tab-button {
      flex: 1 1 calc(50% - 4px);
      text-align: center;
    }

    .project-card {
      padding: 22px 18px;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    .tab-button {
      transition: none;
    }
  }
</style>

<div class="ai-profile">
  <div class="section-tabs" role="tablist" aria-label="Profile sections">
    <button id="tab-about" class="tab-button active" type="button" role="tab" aria-selected="true" aria-controls="about-section" data-tab-target="about-section">
      About
    </button>
    <button id="tab-experience" class="tab-button" type="button" role="tab" aria-selected="false" aria-controls="experience-section" data-tab-target="experience-section">
      Experience
    </button>
    <button id="tab-education" class="tab-button" type="button" role="tab" aria-selected="false" aria-controls="education-section" data-tab-target="education-section">
      Education &amp; Awards
    </button>
    <button id="tab-projects" class="tab-button" type="button" role="tab" aria-selected="false" aria-controls="projects-section" data-tab-target="projects-section">
      Projects
    </button>
  </div>

  <section id="about-section" class="tab-panel active" role="tabpanel" aria-labelledby="tab-about">
    <div class="profile-header">
      <img src="profile.jpg" alt="Varun Reddy" class="profile-image" />

      <div class="profile-text">
        <p class="role">
          <strong>Senior Technical Sourcer @
          <a href="https://www.youtube.com/watch?v=7T7SyMZihwo" target="_blank">Datadog</a></strong>
        </p>
        <p class="tagline">
          Sourcing exceptional <strong>AI Research</strong> talent in New York and Paris for Datadog.
        </p>
      </div>
    </div>

    <p class="bio">
      I hold a master’s degree in Human Resource Management from Trinity College Dublin and a bachelor’s degree in Urban Planning from SPA Bhopal. Recipient of the Trinity Business School Scholarship and the Proficiency Gold Medal in recognition of academic merit.
    </p>

    <p class="contact">
      <a href="mailto:varunreddy5455@gmail.com">varunreddy5455@gmail.com</a> |
      <a href="https://www.linkedin.com/in/varun-m-r/" target="_blank">LinkedIn</a>
    </p>

    <h2>Latest News</h2>
    <ul>
      <li>
        <strong>[May 2026]</strong> We released <a href="https://www.datadoghq.com/blog/ai/toto-2/">Toto 2.0</a>, a family of open-weights time series forecasting models that proves scaling works, with bigger models consistently performing better all the way up to 2.5B parameters.
      </li>

      <li>
        <strong>[Feb 2026]</strong> We’re introducing <a href="https://www.datadoghq.com/blog/ai/toto-exogenous-covariates/">fine-tuning and exogenous covariate support for Toto</a>, enabling teams to adapt the model to their own data and incorporate known future signals to produce more accurate time-series forecasts.
      </li>

      <li>
        <strong>[May 2025]</strong> We unveiled the first two launches (open source under the Apache 2.0 license) from Datadog AI Research!
        <a href="https://huggingface.co/Datadog/Toto-Open-Base-1.0" target="_blank">Toto</a>, a new SOTA (by a wide margin!) time series foundation model, and
        <a href="https://huggingface.co/datasets/Datadog/BOOM" target="_blank"> BOOM</a>, the largest benchmark of observability metrics.
      </li>

      <li>
        We are expanding our AI Research team in New York and Paris! Check out our open
        <a href="https://careers.datadoghq.com/detail/6572669/?gh_jid=6572669" target="_blank">AI Researcher role</a>.
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

    <h2>Fun facts</h2>
    <ul>
      <li>I'm a trained Carnatic classical singer.</li>
      <li>I ran a YouTube channel called <a href="https://www.youtube.com/@AllAboutPlanning" target="_blank">All About Planning</a> where I shared content related to urban planning.</li>
    </ul>
  </section>

  <section id="experience-section" class="tab-panel" role="tabpanel" aria-labelledby="tab-experience">
    <h2>Experience</h2>

    <p class="entry"><strong>Datadog</strong><br>
    Senior Technical Sourcer (AI Research) <em>(Apr 2026 – Present)</em><br>
    Technical Sourcer II (AI Research and Applied AI) <em>(Apr 2024 – April 2026)</em></p>

    <p class="entry"><strong>Azon Recruitment Group</strong><br>
    Principal IT Recruitment Consultant <em>(Sep 2022 – Apr 2024)</em><br>
    Senior IT Recruitment Consultant <em>(Mar 2022 – Sep 2022)</em><br>
    IT Recruitment Consultant <em>(May 2021 – Mar 2022)</em></p>

    <p class="entry"><strong>Next Generation Recruitment</strong><br>
    IT Recruitment Associate <em>(Nov 2019 – May 2021)</em></p>

    <p class="entry"><strong>Temple Recruitment</strong><br>
    Recruitment Consultant <em>(Aug 2019 – Nov 2019)</em></p>
  </section>

  <section id="education-section" class="tab-panel" role="tabpanel" aria-labelledby="tab-education">
    <h2>Education</h2>

    <p class="entry"><strong>Trinity College Dublin</strong><br>
    Master's Degree, Human Resource Management <em>(2018 – 2019)</em></p>

    <p class="entry"><strong>School of Planning and Architecture, Bhopal</strong><br>
    Bachelor's Degree, Urban Planning <em>(2014 – 2018)</em></p>

    <h2>Honors and Awards</h2>

    <p class="entry"><strong>Proficiency Gold Medal for 1st Rank in B. Plan</strong><br>
    Issued by School of Planning and Architecture, Bhopal – Oct 2018</p>

    <p class="entry"><strong>Trinity Business School Scholarship 2018/19</strong><br>
    Issued by Trinity Business School – Oct 2018</p>

    <p class="entry"><strong>3rd Best Thesis Award</strong><br>
    Issued by Institute of Town Planners, Madhya Pradesh Chapter – Aug 2018<br>
    Thesis: Assessing and Planning for Airport Induced Land Uses – A Case of Cochin</p>

    <p class="entry"><strong>South India Zonal Level First Position</strong><br>
    Issued by IT Akshaya Prathiba – Feb 2010<br>
    IT Competition on Library Database Management using MS Access</p>

    <p class="entry"><strong>Karnataka State Level 7th Rank</strong><br>
    Issued by 2nd International Level Science Talent Search Examination – Aug 2007</p>
  </section>

  <section id="projects-section" class="tab-panel" role="tabpanel" aria-labelledby="tab-projects">
    <h2>Personal projects</h2>

    <article class="project-card">
      <p class="eyebrow">Web app</p>
      <h3>
        <a href="https://varunreddy5455.github.io/QuickCopy/" target="_blank" rel="noopener noreferrer">QuickCopy</a>
      </h3>
      <p class="project-blurb">
        <a href="https://varunreddy5455.github.io/QuickCopy/" target="_blank" rel="noopener noreferrer">QuickCopy</a>
        is a lightweight template manager I built to keep reusable writing in one place. You can create and customize templates, save them for later, and copy them across email, docs, and other tools so you never have to rebuild the same message on every platform.
      </p>
      <a class="project-link" href="https://varunreddy5455.github.io/QuickCopy/" target="_blank" rel="noopener noreferrer">Open QuickCopy ↗</a>
    </article>
  </section>
</div>

<script>
  (function () {
    var tabButtons = document.querySelectorAll(".tab-button");
    var tabPanels = document.querySelectorAll(".tab-panel");

    function setActiveTab(targetId) {
      tabButtons.forEach(function (button) {
        var isActive = button.getAttribute("data-tab-target") === targetId;
        button.classList.toggle("active", isActive);
        button.setAttribute("aria-selected", String(isActive));
      });

      tabPanels.forEach(function (panel) {
        var isActive = panel.id === targetId;
        panel.classList.toggle("active", isActive);
      });
    }

    tabButtons.forEach(function (button) {
      button.addEventListener("click", function () {
        setActiveTab(button.getAttribute("data-tab-target"));
      });
    });

    setActiveTab("about-section");
  })();
</script>
