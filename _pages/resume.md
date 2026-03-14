---
layout: page
title: Resume
permalink: /resume/
---

<style>
  .resume-wrapper {
    max-width: 1000px;
    margin: 0 auto;
    color: var(--text, #333);
    font-family: var(--font-body, system-ui, -apple-system, sans-serif);
    line-height: 1.6;
  }
  
  /* Header */
  .resume-header {
    border-bottom: 2px solid var(--border, #eaeaea);
    padding-bottom: 2rem;
    margin-bottom: 3rem;
  }
  .resume-name {
    font-size: 2.75rem;
    font-weight: 800;
    margin: 0 0 0.5rem 0;
    letter-spacing: -0.02em;
    line-height: 1.1;
  }
  .resume-subtitle {
    font-size: 1.35rem;
    color: var(--text-muted, #555);
    margin: 0 0 1.25rem 0;
    font-weight: 400;
    max-width: 800px;
    line-height: 1.4;
  }
  .resume-contact {
    display: flex;
    flex-wrap: wrap;
    gap: 1.5rem;
    font-size: 0.95rem;
    color: var(--text-muted, #666);
  }
  .resume-contact a {
    color: inherit;
    text-decoration: none;
    border-bottom: 1px solid currentColor;
    transition: color 0.2s, border-color 0.2s;
  }
  .resume-contact a:hover {
    color: var(--accent, #0056b3);
    border-color: var(--accent, #0056b3);
  }

  /* Layout */
  .resume-grid {
    display: grid;
    gap: 4rem;
  }
  @media (min-width: 800px) {
    .resume-grid {
      grid-template-columns: 2fr 1fr;
    }
  }

  /* Sections */
  .resume-section {
    margin-bottom: 3rem;
  }
  .resume-section-title {
    font-size: 1.25rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    border-bottom: 1px solid var(--border, #eaeaea);
    padding-bottom: 0.5rem;
    margin-bottom: 1.5rem;
    color: var(--text, #111);
  }

  /* Typography / Content */
  .resume-main p {
    margin-bottom: 1.25rem;
    font-size: 1.05rem;
    color: var(--text-muted, #444);
  }

  /* Focus Grid */
  .focus-grid {
    display: grid;
    gap: 1.5rem;
  }
  @media (min-width: 600px) {
    .focus-grid {
      grid-template-columns: 1fr 1fr;
    }
  }
  .focus-item h4 {
    margin: 0 0 0.5rem 0;
    font-size: 1.05rem;
    font-weight: 600;
    color: var(--text, #222);
  }
  .focus-item p {
    margin: 0;
    font-size: 0.95rem;
  }

  /* Experience Items */
  .exp-item {
    margin-bottom: 2.5rem;
  }
  .exp-header {
    margin-bottom: 0.75rem;
  }
  .exp-company {
    font-size: 1.3rem;
    font-weight: 700;
    margin: 0;
    color: var(--text, #111);
  }
  .exp-role-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: baseline;
    margin-top: 0.25rem;
    gap: 0.5rem;
  }
  .exp-role {
    font-weight: 600;
    font-size: 1.1rem;
    color: var(--text-muted, #555);
    margin: 0;
  }
  .exp-meta {
    font-size: 0.9rem;
    color: var(--text-muted, #777);
    font-family: var(--font-mono, ui-monospace, SFMono-Regular, Consolas, monospace);
  }
  .exp-desc {
    font-size: 1rem;
    color: var(--text-muted, #444);
  }
  .exp-desc p {
    margin-bottom: 0.75rem;
    font-size: 1rem;
  }
  .exp-desc ul {
    padding-left: 1.25rem;
    margin-top: 0.5rem;
    margin-bottom: 0;
    list-style-type: square;
  }
  .exp-desc li {
    margin-bottom: 0.35rem;
  }

  /* Sidebar styling */
  .resume-sidebar .resume-section-title {
    font-size: 1.05rem;
    border-bottom: none;
    padding-bottom: 0;
    margin-bottom: 1.25rem;
    color: var(--text-muted, #555);
  }
  .sidebar-block {
    margin-bottom: 2.5rem;
  }
  .sidebar-list {
    list-style: none;
    padding: 0;
    margin: 0;
    font-size: 0.95rem;
    color: var(--text-muted, #444);
  }
  .sidebar-list li {
    margin-bottom: 0.75rem;
    padding-bottom: 0.75rem;
    border-bottom: 1px solid var(--border-light, #f0f0f0);
    line-height: 1.5;
  }
  .sidebar-list li:last-child {
    border-bottom: none;
    margin-bottom: 0;
    padding-bottom: 0;
  }
  
  /* Skills/Tags style for lists */
  .tag-list {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .tag-list li {
    background: var(--bg-alt, #f5f5f5);
    border: 1px solid var(--border, #eaeaea);
    padding: 0.35rem 0.75rem;
    border-radius: 6px;
    font-size: 0.9rem;
    color: var(--text-muted, #444);
  }

  .resume-footer {
    margin-top: 4rem;
    padding-top: 2rem;
    border-top: 1px solid var(--border, #eaeaea);
    text-align: center;
    font-size: 0.95rem;
    color: var(--text-muted, #777);
  }
  .resume-footer a {
    color: inherit;
    text-decoration: underline;
  }
</style>

<div class="resume-wrapper">
  
  <header class="resume-header">
    <h1 class="resume-name">Paul D. Hobson</h1>
    <h2 class="resume-subtitle">Technology leader, systems thinker, and builder of complex digital platforms.</h2>
    <div class="resume-contact">
      <span>📍 Calgary, Alberta, Canada</span>
      <a href="https://linkedin.com/in/pauldhobson" target="_blank" rel="noopener noreferrer">LinkedIn Profile</a>
    </div>
  </header>

  <div class="resume-grid">
    
    <!-- MAIN COLUMN -->
    <main class="resume-main">
      
      <section class="resume-section">
        <h3 class="resume-section-title">Profile</h3>
        <p>I work at the intersection of technology platforms, operational systems, and organizational change.</p>
        <p>Over the past two decades I have led technology architecture, infrastructure modernization, and digital platform development across energy, aviation, higher education, and research institutions. My work focuses on designing systems that connect people, data, and infrastructure in reliable and resilient ways.</p>
        <p>My approach blends deep technical grounding with systems thinking: understanding how platforms, organizations, and processes interact over time. I am particularly interested in complex operational environments where software, infrastructure, and physical systems intersect.</p>
        <p>Earlier in my career I worked in geospatial analysis and earth observation research in collaboration with international space agencies, developing expertise in large-scale data analysis and scientific computing.</p>
        <p>Today my work focuses on platform engineering, enterprise architecture, and technology strategy &mdash; building technology foundations that enable organizations to operate, adapt, and evolve.</p>
      </section>

      <section class="resume-section">
        <h3 class="resume-section-title">Areas of Focus</h3>
        <div class="focus-grid">
          <div class="focus-item">
            <h4>Technology Platforms</h4>
            <p>Design and modernization of enterprise technology platforms including cloud infrastructure, operational systems, integration architecture, and distributed data environments.</p>
          </div>
          <div class="focus-item">
            <h4>Systems Thinking</h4>
            <p>Applying architectural and systems approaches to complex environments where technology, operations, and organizations intersect.</p>
          </div>
          <div class="focus-item">
            <h4>Enterprise Architecture</h4>
            <p>Designing long-term technology frameworks that align infrastructure, applications, and data systems into coherent operating models.</p>
          </div>
          <div class="focus-item">
            <h4>Platform Engineering</h4>
            <p>Building internal platforms that enable teams to deliver software and services more reliably and efficiently.</p>
          </div>
          <div class="focus-item">
            <h4>Operational Technology</h4>
            <p>Working across IT and operational environments where digital platforms interact with physical infrastructure and real-world processes.</p>
          </div>
          <div class="focus-item">
            <h4>Technology Strategy</h4>
            <p>Helping organizations translate strategic goals into practical technology roadmaps and implementation programs.</p>
          </div>
        </div>
      </section>

      <section class="resume-section">
        <h3 class="resume-section-title">Professional Experience</h3>
        
        <div class="exp-item">
          <div class="exp-header">
            <h4 class="exp-company">Plains</h4>
            <div class="exp-role-row">
              <span class="exp-role">Technology Platforms Leader</span>
              <span class="exp-meta">Calgary, Canada &nbsp;|&nbsp; 2025 &ndash; Present</span>
            </div>
          </div>
          <div class="exp-desc">
            <p>Responsible for technology platform strategy supporting large-scale operational environments across North America. The work centers on evolving large technology ecosystems while maintaining reliability and operational continuity.</p>
            <ul>
              <li>Platform architecture and infrastructure modernization</li>
              <li>Enterprise platform strategy and operating models</li>
              <li>Technology resilience and reliability engineering</li>
              <li>Integration of enterprise and operational technology systems</li>
              <li>Technology governance and architectural standards</li>
            </ul>
          </div>
        </div>

        <div class="exp-item">
          <div class="exp-header">
            <h4 class="exp-company">Plains</h4>
            <div class="exp-role-row">
              <span class="exp-role">Head of Business Engagement &amp; Architecture</span>
              <span class="exp-meta">Calgary, Canada &nbsp;|&nbsp; 2023 &ndash; 2025</span>
            </div>
          </div>
          <div class="exp-desc">
            <p>Led enterprise architecture and technology engagement across operational and corporate business domains, translating complex operational requirements into coherent technology strategy.</p>
            <ul>
              <li>Developing enterprise technology roadmaps</li>
              <li>Aligning technology initiatives with operational needs</li>
              <li>Improving integration across distributed systems and platforms</li>
              <li>Strengthening architectural governance and technical standards</li>
            </ul>
          </div>
        </div>

        <div class="exp-item">
          <div class="exp-header">
            <h4 class="exp-company">WestJet</h4>
            <div class="exp-role-row">
              <span class="exp-role">Head of Technology Strategy &amp; Enterprise Services</span>
              <span class="exp-meta">Calgary, Canada &nbsp;|&nbsp; 2022 &ndash; 2023</span>
            </div>
          </div>
          <div class="exp-desc">
            <p>Led technology strategy and platform services supporting airline operations and corporate systems.</p>
            <ul>
              <li>Development of enterprise technology strategy and operating models</li>
              <li>Improvement of platform reliability and operational resilience</li>
              <li>Alignment of technology investment with operational priorities</li>
              <li>Technology governance and architectural oversight</li>
            </ul>
          </div>
        </div>

        <div class="exp-item">
          <div class="exp-header">
            <h4 class="exp-company">WestJet</h4>
            <div class="exp-role-row">
              <span class="exp-role">Head of Architecture</span>
              <span class="exp-meta">Calgary, Canada &nbsp;|&nbsp; 2018 &ndash; 2022</span>
            </div>
          </div>
          <div class="exp-desc">
            <p>Led enterprise architecture and technology governance for a large and complex operational environment.</p>
            <ul>
              <li>Establishing enterprise architecture practices across the organization</li>
              <li>Developing long-term technology modernization roadmaps</li>
              <li>Improving system reliability through architectural governance</li>
              <li>Leading architecture teams across multiple technical domains</li>
            </ul>
          </div>
        </div>

        <div class="exp-item">
          <div class="exp-header">
            <h4 class="exp-company">University of British Columbia</h4>
            <div class="exp-role-row">
              <span class="exp-role">Director of Enterprise Architecture</span>
              <span class="exp-meta">Vancouver, Canada &nbsp;|&nbsp; 2011 &ndash; 2018</span>
            </div>
          </div>
          <div class="exp-desc">
            <p>Led enterprise architecture for one of Canada’s largest universities. Focused on aligning technology investments with institutional strategy while supporting a diverse ecosystem of research, academic, and administrative systems.</p>
            <ul>
              <li>Establishing enterprise architecture governance</li>
              <li>Supporting large-scale institutional technology transformation</li>
              <li>Developing business cases for major technology initiatives</li>
              <li>Enabling cross-campus collaboration on technology strategy</li>
            </ul>
          </div>
        </div>

        <div class="exp-item">
          <div class="exp-header">
            <h4 class="exp-company">Cardiff University</h4>
            <div class="exp-role-row">
              <span class="exp-role">Deputy Chief Technology Officer</span>
              <span class="exp-meta">Cardiff, United Kingdom &nbsp;|&nbsp; 2005 &ndash; 2011</span>
            </div>
            <div style="font-size: 0.95rem; font-weight: 500; color: var(--text-muted, #555); margin-top: 0.25rem;">
               Associate Director, Web Service Delivery <span>&nbsp;&middot;&nbsp;</span> Web and Portal Manager
            </div>
          </div>
          <div class="exp-desc">
            <p>Led early enterprise architecture initiatives and digital transformation programs for one of the UK’s major research universities. Participated in national research programs exploring enterprise architecture and service-oriented digital infrastructure for higher education.</p>
          </div>
        </div>

      </section>

      <section class="resume-section">
        <h3 class="resume-section-title">Early Career</h3>
        <p>Before moving into technology leadership roles, I worked in research computing and geospatial analysis. Research work included collaboration with international space and earth observation programs analyzing satellite data for environmental monitoring and large-scale geographic systems.</p>
        <p>This early experience developed my interest in complex data systems, distributed computing, and analytical modeling.</p>
      </section>

    </main>

    <!-- SIDEBAR COLUMN -->
    <aside class="resume-sidebar">
      
      <div class="sidebar-block">
        <h3 class="resume-section-title">Education</h3>
        <ul class="sidebar-list">
          <li>
            <strong style="color: var(--text, #222);">BSc (Hons) Geography</strong><br>
            University of Manchester<br>
            <span class="exp-meta">United Kingdom</span>
          </li>
        </ul>
      </div>

      <div class="sidebar-block">
        <h3 class="resume-section-title">Certifications</h3>
        <ul class="sidebar-list">
          <li>TOGAF Certified Enterprise Architecture</li>
          <li>ITIL Foundations</li>
          <li>AWS Cloud Practitioner</li>
          <li>Microsoft Azure Fundamentals</li>
          <li>Microsoft Azure Data Fundamentals</li>
          <li>Microsoft Azure AI Fundamentals</li>
        </ul>
      </div>

      <div class="sidebar-block">
        <h3 class="resume-section-title">Professional Memberships</h3>
        <ul class="sidebar-list">
          <li>Canadian Information Processing Society (CIPS)</li>
          <li>Association of Enterprise Architects</li>
          <li>Association for Computing Machinery</li>
          <li>Information Systems Audit and Control Association</li>
          <li>Data Management Association</li>
        </ul>
      </div>

      <div class="sidebar-block">
        <h3 class="resume-section-title">Personal Interests</h3>
        <ul class="tag-list">
          <li>Complex systems &amp; modeling</li>
          <li>Geography &amp; environments</li>
          <li>Open technology ecosystems</li>
          <li>Experimental computing infrastructure</li>
        </ul>
      </div>

    </aside>

  </div>
  
  <footer class="resume-footer">
    A full CV is available on request. For a full PDF, please use the <a href="/contact/">contact page</a>.
  </footer>

</div>
