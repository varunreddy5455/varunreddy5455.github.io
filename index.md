---
layout: default
title: Varun Reddy
---

<style>
  .page-header {
    display: none;
  }

  html {
    scroll-behavior: smooth;
  }

  body {
    background: linear-gradient(180deg, #f4f5f7 0%, #eceff3 52%, #e8ebf0 100%);
    color: #111111;
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  }

  .top-bar {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 16px;
    padding: 12px 18px;
    background: linear-gradient(135deg, #171a20 0%, #262d37 100%);
    border-bottom: 1px solid rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(8px);
  }

  .brand {
    color: #111111;
    background: rgba(255, 255, 255, 0.95);
    border-radius: 999px;
    padding: 8px 14px;
    font-weight: 600;
    letter-spacing: 0.01em;
    white-space: nowrap;
  }

  .top-nav {
    display: flex;
    align-items: center;
    gap: 10px;
    flex-wrap: wrap;
    justify-content: flex-end;
  }

  .top-link {
    text-decoration: none;
    color: #f2f5fb;
    background: rgba(255, 255, 255, 0.08);
    border: 1px solid rgba(255, 255, 255, 0.22);
    border-radius: 999px;
    padding: 7px 13px;
    font-size: 0.92rem;
    transition: all 120ms ease;
  }

  .top-link:hover {
    background: rgba(255, 255, 255, 0.2);
  }

  .top-link.active {
    color: #111111;
    background: #ffffff;
    border-color: #ffffff;
  }

  .main-content {
    max-width: 960px;
    margin: 0 auto;
    padding: 110px 28px 72px;
  }

  .ai-profile {
    color: #111111;
  }

  .ai-profile a {
    color: #111111;
    text-decoration: underline;
    text-underline-offset: 2px;
  }

  .ai-profile a:hover {
    color: #2c2c2c;
  }

  .section-block {
    scroll-margin-top: 96px;
    padding: 48px 0 36px;
  }

  .section-block + .section-block {
    margin-top: 92px;
    border-top: 2px solid rgba(17, 17, 17, 0.22);
    padding-top: 86px;
  }

  .section-title {
    margin: 0 0 22px;
    font-size: 1.42rem;
    font-weight: 600;
    letter-spacing: -0.01em;
  }

  .profile-header {
    display: flex;
    align-items: center;
    gap: 28px;
    flex-wrap: wrap;
    margin-bottom: 18px;
  }

  .profile-image {
    border-radius: 50%;
    object-fit: cover;
    width: 140px;
    height: 140px;
    border: none;
  }

  .profile-text {
    max-width: 680px;
  }

  .role {
    margin: 0;
    font-size: 1.06rem;
    font-weight: 600;
  }

  .tagline {
    margin: 10px 0 0;
    line-height: 1.8;
  }

  .bio {
    margin: 0 0 24px;
    line-height: 1.9;
    max-width: 860px;
  }

  .contact {
    margin: 0;
    line-height: 1.8;
  }

  .subheading {
    font-size: 1.1rem;
    margin: 48px 0 20px;
    font-weight: 600;
  }

  .ai-profile ul {
    margin: 0 0 8px;
    padding-left: 22px;
    line-height: 2;
  }

  .ai-profile li {
    margin-bottom: 20px;
  }

  .entry {
    margin: 0 0 46px;
    line-height: 2;
  }

  @media (max-width: 860px) {
    .top-bar {
      padding: 10px 12px;
    }

    .brand {
      padding: 7px 11px;
      font-size: 0.92rem;
    }

    .top-link {
      font-size: 0.86rem;
      padding: 6px 10px;
    }

    .main-content {
      padding: 124px 16px 56px;
    }

    .section-block + .section-block {
      margin-top: 64px;
      padding-top: 64px;
    }
  }
</style>

<header class="top-bar" aria-label="Primary navigation">
  <div class="brand">Varun Reddy</div>
  <nav class="top-nav">
    <a class="top-link active" href="#about-section" data-section="about-section">About</a>
    <a class="top-link" href="#experience-section" data-section="experience-section">Experience</a>
    <a class="top-link" href="#education-section" data-section="education-section">Education &amp; Awards</a>
  </nav>
</header>

<div class="ai-profile">
  <section id="about-section" class="section-block" aria-label="About">
    <h2 class="section-title">About</h2>

    <div class="profile-header">
      <img src="profile.jpg" alt="Varun Reddy" class="profile-image" />

      <div class="profile-text">
        <p class="role">
          Technical Sourcer @
          <a href="https://www.youtube.com/watch?v=7T7SyMZihwo" target="_blank">Datadog</a>
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

    <h3 class="subheading">Latest News</h3>
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

    <h3 class="subheading">Fun facts</h3>
    <ul>
      <li>I'm a trained Carnatic classical singer.</li>
      <li>I ran a YouTube channel called <a href="https://www.youtube.com/@AllAboutPlanning" target="_blank">All About Planning</a> where I shared content related to urban planning.</li>
    </ul>
  </section>

  <section id="experience-section" class="section-block" aria-label="Experience">
    <h2 class="section-title">Experience</h2>

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

  <section id="education-section" class="section-block" aria-label="Education and awards">
    <h2 class="section-title">Education &amp; Awards</h2>

    <h3 class="subheading">Education</h3>
    <p class="entry"><strong>Trinity College Dublin</strong><br>
    Master's Degree, Human Resource Management <em>(2018 – 2019)</em></p>

    <p class="entry"><strong>School of Planning and Architecture, Bhopal</strong><br>
    Bachelor's Degree, Urban Planning <em>(2014 – 2018)</em></p>

    <h3 class="subheading">Honors and Awards</h3>
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
    }

    links.forEach(function (link) {
      link.addEventListener("click", function (event) {
        event.preventDefault();
        var targetId = link.getAttribute("data-section");
        var target = document.getElementById(targetId);
        if (!target) return;
        setActive(targetId);
        target.scrollIntoView({ behavior: "smooth", block: "start" });
      });
    });

    if ("IntersectionObserver" in window) {
      var observer = new IntersectionObserver(
        function (entries) {
          entries.forEach(function (entry) {
            if (entry.isIntersecting) {
              setActive(entry.target.id);
            }
          });
        },
        {
          root: null,
          rootMargin: "-40% 0px -45% 0px",
          threshold: 0,
        }
      );

      sections.forEach(function (section) {
        observer.observe(section);
      });
    }

    setActive("about-section");
  })();
</script>

