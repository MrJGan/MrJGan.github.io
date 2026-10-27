---
layout: portfolio-home
permalink: /
---
<div class="site-shell">
  <header class="site-header">
    <a class="wordmark" href="/" aria-label="Jing Gan home">JING GAN<span class="mark-dot">.</span></a>
    <nav aria-label="Main navigation">
      <a href="/#projects">Projects</a>
      <a href="/teaching/">Teaching</a>
      <a href="/cv/">CV</a>
    </nav>
  </header>

  <main id="main-content">
    <section class="intro" aria-labelledby="intro-title">
      <div class="intro-main">
        <p class="eyebrow"><span class="status-line"></span> APPLIED ECONOMIST <span class="eyebrow-slash">/</span> QUANTITATIVE RESEARCHER</p>
        <h1 id="intro-title">Researching markets,<br><em>policy</em> &amp; firm behavior.</h1>
        <p class="intro-description">I'm Jing Gan, an applied economist with a Ph.D. in Resource Economics from UMass Amherst and an M.S. in Computer Science from Georgia Tech. I study how competition and public policy shape firms, markets, and consumer outcomes.</p>
      </div>
      <div class="intro-side">
        <img class="profile-portrait" src="{{ '/assets/images/jing-gan-portrait.jpg' | relative_url }}" alt="Portrait of Jing Gan" width="360" height="450" decoding="async" fetchpriority="high">
        <div class="intro-meta">
        <span class="tiny-label">RESEARCH AREAS</span>

        <p>
          Applied Microeconomics<br>
          Industrial Organization<br>
          Health Economics &amp; Policy
        </p>

        <span class="tiny-label side-bottom">
          PhD · September 2026
        </span>
        </div>
      </div>

    </section>

    <section class="dashboard" aria-label="Research, methods, and teaching overview">
      <div class="research-panel" id="research">
        <div class="panel-top"><span class="section-index">01 / RESEARCH</span><span class="panel-marker">SELECTED WORK</span></div>
        <h2>Research</h2>
        <p class="section-intro">Spatial competition, nutrition policy, and firm behavior.</p>
        <div class="research-list">
          <details class="research-item"><summary><span class="research-number">01</span><span class="research-title">US Restaurants' Quality and Spatial Competition<small>Job Market Paper · Spatial Industrial Organization</small></span><span class="research-action" aria-hidden="true">
  <span class="action-closed">VIEW</span>
  <span class="action-open">CLOSE</span>
  <span class="research-arrow">→</span>
</span></summary><div class="research-detail">This paper examines how quality differentiation, population concentration, and local market conditions shape restaurant location patterns across major U.S. cities. High-quality restaurants tend to be more spatially dispersed within their own quality group, while low-quality restaurants tend to be more concentrated.</div></details>
          <details class="research-item"><summary><span class="research-number">02</span><span class="research-title">Reactions to FDA Sodium Reduction Guidance: Demand and Supply<small>Selected Paper · 2023 AAEA Annual Meeting</small></span><span class="research-action" aria-hidden="true">
  <span class="action-closed">VIEW</span>
  <span class="action-open">CLOSE</span>
  <span class="research-arrow">→</span>
</span></summary><div class="research-detail">Using more than 400,000 chain-restaurant menu-item observations from 2016 to 2019, this paper evaluates responses to voluntary sodium reduction guidance. Fixed-effects and event-study analyses show selective reformulation, especially among limited-service restaurants and certain menu categories.</div></details>
          <details class="research-item"><summary><span class="research-number">03</span><span class="research-title">Local Competitive Density and Voluntary Policy Compliance<small>Health Economics · Local Market Competition</small></span><span class="research-action" aria-hidden="true">
  <span class="action-closed">VIEW</span>
  <span class="action-open">CLOSE</span>
  <span class="research-arrow">→</span>
</span></summary><div class="research-detail">Combining longitudinal menu data, store-level Yelp reviews, and spatial competition measures, this paper finds larger sodium reductions among chains more exposed to dense urban markets and stronger consumer-response associations in more competitive markets.</div></details>
        </div>
        <div class="working-note">
          <span class="note-title">WORK IN PROGRESS</span>
          
          <p>NYC Calorie Labeling Rule</p>
          <p>Entry Barriers in Food Industry Competition</p>
        </div>
      </div>

      <div class="side-panels">
        <section class="expertise-panel" id="expertise" aria-labelledby="expertise-title">
          <div class="panel-top"><span class="section-index">02 / METHODS &amp; TOOLS</span></div>
          <h2 id="expertise-title">A quantitative<br><em>toolkit</em></h2>
          <div class="skill-block"><span class="tiny-label">ECONOMETRICS</span><p>Causal inference, panel data, structural IO, discrete choice, spatial &amp; multilevel modeling</p></div>
          <div class="skill-block"><span class="tiny-label">COMPUTATIONAL METHODS</span><p>Data collection, record linkage, spatial &amp; text analysis, machine learning</p></div>
          <div class="skill-block"><span class="tiny-label">PROGRAMMING</span><p>Python <span>·</span> R <span>·</span> Stata <span>·</span> SQL <span>·</span> MATLAB <span>·</span> Java <span>·</span> C++ <span>·</span> LaTeX</p></div>
        </section>
        <a href="/teaching/" class="teaching-panel" aria-labelledby="teaching-title"><div class="panel-top">
  <span class="section-index">03 / TEACHING</span>
  <span class="teaching-top-link">
    VIEW TEACHING <span aria-hidden="true">↗</span>
  </span>
</div><h2 id="teaching-title">Teaching &amp;<br><em>mentorship</em></h2><p class="teaching-experience">
  <span>Instructor of Record · UMass Amherst</span>
  <span>Substitute Instructor · Smith College</span>
</p><div class="teaching-bottom"><span>Vijay Bhagavan Teaching Assistant of Distinction Award · 2022</span></div></a>
      </div>
    </section>
    <section class="projects-section" id="projects" aria-labelledby="projects-title">
      <div class="panel-top"><span class="section-index">04 / DATA PROJECTS</span><span class="panel-marker">INTERACTIVE RESEARCH</span></div>
      <h2 id="projects-title">Data &amp; computational projects</h2>
      <article class="project-feature">
        <div>
          <span class="tiny-label">URBAN SPATIAL ANALYTICS LAB</span>
          <h3>Boston: population density<br>and employment geography</h3>
          <p>How much does the choice of city center matter? An interactive study of population density gradients, employment cores, and the role of spatial scale.</p>
          <p class="project-meta">PYTHON · CENSUS ACS · LODES · SPATIAL ANALYSIS</p>
          <div class="project-links">
            <a href="{{ '/projects/boston/' | relative_url }}">Read the project <span aria-hidden="true">→</span></a>
            {% if site.data.urban_lab.app_url != "" and site.data.urban_lab.app_url %}<a href="{{ site.data.urban_lab.app_url | escape }}" target="_blank" rel="noopener noreferrer">Open interactive explorer <span aria-hidden="true">↗</span></a>{% endif %}
          </div>
        </div>
        <a href="{{ '/projects/boston/' | relative_url }}" aria-label="Read the Boston urban spatial analytics project">
          <img class="project-figure" src="{{ '/assets/projects/boston/density-radius.svg' | relative_url }}" alt="Fitted population density decline becomes smaller as the study radius grows; the three center definitions give similar results." width="960" height="480" loading="lazy">
        </a>
      </article>
    </section>
  </main>
  <footer class="site-footer"><span>© {{ 'now' | date: '%Y' }} JING GAN</span><div><a href="mailto:jinggan@umass.edu">Email ↗</a><a href="/cv/">Curriculum Vitae ↗</a></div></footer>
</div>
