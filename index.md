---
layout: default
title: Varun Reddy
---

# Hey, I'm Varun 👋

<style>
  .ai-profile {
    background: linear-gradient(180deg, #0d1117 0%, #111827 100%);
    color: #dbe7ff;
    border: 1px solid #2b3550;
    border-radius: 16px;
    padding: 24px;
    margin-top: 18px;
    font-family: "IBM Plex Mono", "Fira Code", ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
    box-shadow: 0 12px 30px rgba(6, 12, 26, 0.4);
  }

  .ai-profile a {
    color: #7cc8ff;
  }

  .ai-profile a:hover {
    color: #a3ddff;
  }

  .profile-header {
    display: flex;
    align-items: center;
    gap: 24px;
    flex-wrap: wrap;
    margin-bottom: 14px;
  }

  .profile-image {
    border-radius: 50%;
    object-fit: cover;
    width: 140px;
    height: 140px;
    border: 2px solid #58a6ff;
  }

  .profile-text {
    max-width: 650px;
  }

  .role {
    margin: 0;
    font-size: 1.05em;
  }

  .tagline {
    margin: 8px 0 0;
  }

  .bio {
    margin: 14px 0;
    line-height: 1.65;
  }

  .contact {
    margin: 0 0 14px;
  }

  .section-tabs {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
    margin: 2px 0 20px;
  }

  .tab-button {
    padding: 8px 14px;
    border-radius: 8px;
    border: 1px solid #334066;
    background: #111b2f;
    color: #dbe7ff;
    cursor: pointer;
    font: inherit;
  }

  .tab-button:hover {
    border-color: #58a6ff;
  }

  .tab-button.active {
    background: #0f2a4a;
    border-color: #7cc8ff;
    color: #ecf6ff;
  }

  .tab-panel {
    display: none;
  }

  .tab-panel.active {
    display: block;
  }

  .ai-profile h2 {
    font-size: 1.28em;
    color: #e8f1ff;
    margin: 22px 0 12px;
    border-left: 3px solid #58a6ff;
    padding-left: 10px;
  }

  .ai-profile ul {
    margin: 0;
    padding-left: 20px;
    line-height: 1.6;
  }

  .ai-profile li {
    margin-bottom: 8px;
  }

  .entry {
    margin-bottom: 16px;
    line-height: 1.6;
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
  </div>

  <section id="about-section" class="tab-panel active" role="tabpanel" aria-labelledby="tab-about">
    <div class="profile-header">
      <img src="profile.jpg" alt="Varun Reddy" class="profile-image" />

      <div class="profile-text">
        <p class="role">
          <strong>Technical Sourcer @
          <a href="https://www.youtube.com/watch?v=7T7SyMZihwo" target="_blank">Datadog</a></strong>
        </p>
        <p class="tagline">
          Sourcing exceptional <strong>AI Research</strong>, and <strong>Applied AI</strong> talent in the US and EMEA for Datadog.
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
        We’re introducing fine-tuning and exogenous covariate support for Toto, enabling teams to adapt the model to their own data and incorporate known future signals to produce more accurate time-series forecasts.
      </li>

      <li>
        We unveiled the first two launches (open source under the Apache 2.0 license) from Datadog AI Research!
        <a href="https://huggingface.co/Datadog/Toto-Open-Base-1.0" target="_blank">Toto</a>, a new SOTA (by a wide margin!) time series foundation model, and
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

    <h2>Fun facts</h2>
    <ul>
      <li>I'm a trained Carnatic classical singer.</li>
      <li>I ran a YouTube channel called <a href="https://www.youtube.com/@AllAboutPlanning" target="_blank">All About Planning</a> where I shared content related to urban planning.</li>
    </ul>
  </section>

  <section id="experience-section" class="tab-panel" role="tabpanel" aria-labelledby="tab-experience">
    <h2>Experience</h2>

    <p class="entry"><strong>Datadog</strong><br>
    Technical Sourcer II (AI and Security) <em>(Apr 2024 – Present)</em></p>

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

