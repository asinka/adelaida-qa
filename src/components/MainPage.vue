<script setup lang="ts">
import ProjectsSection from './ProjectsSection.vue'

const toolkitPillars = [
  {
    number: '01', title: 'Quality Leadership', icon: 'pi-users', description: 'Building capable QA teams and aligning quality with product goals.', featured: true,
    groups: [
      { title: 'People leadership', skills: ['Team building', 'Hiring', 'Mentoring', 'Onboarding', 'Resource planning'] },
      { title: 'Quality leadership', skills: ['QA strategy', 'Process design', 'Cross-team alignment', 'Stakeholder management', 'Continuous improvement'] },
    ],
  },
  {
    number: '02', title: 'Quality Ecosystem', icon: 'pi-sitemap', description: 'Making quality visible, measurable, and repeatable throughout delivery.',
    groups: [
      { title: 'Testing foundations', skills: ['Test strategy', 'Test planning', 'Risk-based testing', 'Exploratory testing', 'Test design', 'Defect management'] },
      { title: 'Test operations', skills: ['Qase', 'Allure', 'Zephyr'] },
      { title: 'Delivery', skills: ['GitHub', 'GitLab', 'GitHub Actions', 'Jenkins', 'Bamboo CI', 'Jira', 'Linear'] },
    ],
  },
  {
    number: '03', title: 'Test Engineering', icon: 'pi-code', description: 'Technical depth to guide automation across UI, mobile, and APIs.',
    groups: [
      { title: 'Automation', skills: ['Playwright', 'Selenium', 'Cypress.io', 'Cucumber', 'Appium'] },
      { title: 'Languages', skills: ['TypeScript', 'JavaScript', 'Python', 'Java'] },
      { title: 'API testing', skills: ['REST API', 'GraphQL', 'gRPC', 'Postman'] },
    ],
  },
]

const experience = [
  {
    period: '07.2025 — Present', role: 'QA Automation Lead', company: 'Alix Inc', location: 'Remote', current: true,
    highlights: [
      "Joined as the company's first QA automation engineer and built the automation foundation from scratch.",
      'Established testing and automation processes for a fully distributed international engineering organization.',
      'Built the QA team and led hiring, onboarding, and team development.',
      'Lead six direct reports across five product teams, partnering with US-based managers and engineers worldwide.',
      'Developed E2E automation with Playwright and introduced Python-based tests for internal tools.',
      'Evolved delivery workflows with GitHub, GitHub Actions, Jira, and Linear.',
    ],
  },
  {
    period: '06.2024 — 05.2025', role: 'QA Fullstack Engineer', company: 'Vivid Money', location: 'Remote',
    highlights: [
      'Set up a QA process for a new product team from scratch.',
      'Expanded automated regression and feature test coverage using Playwright and TypeScript.',
      'Revived and scaled mobile test automation after years of inactivity.',
      'Evaluated AI-based tools for mobile E2E automation in collaboration with an external team.',
      'Increased gRPC API test coverage and manually tested new API and mobile features.',
      'Maintained up-to-date test documentation.',
    ],
  },
  {
    period: '02.2023 — 05.2024', role: 'QA Automation Engineer / Team Lead', company: 'Trak Services', location: 'Remote',
    highlights: [
      'Built test automation from the ground up as the first QA automation engineer on the team.',
      'Achieved 40–80% test coverage across multiple projects, leading one to 80% coverage under my guidance.',
      'Reduced regression testing time from two days to four hours through automation.',
      'Mentored manual testers in automation basics and onboarded new QA automation engineers.',
      'Conducted interviews and managed task planning and resource allocation for the automation team.',
      'Initiated regular QA team meetings and drove continuous process improvements.',
    ],
  },
  {
    period: '09.2022 — 01.2023', role: 'Software Developer in Test', company: 'Lightspeed', location: 'Tbilisi',
    highlights: [
      'Expanded E2E coverage with Playwright and Appium.',
      'Structured test runs and reports by feature for better traceability.',
      'Monitored and maintained automated test results for stability and relevance.',
      'Enhanced internal testing framework and infrastructure.',
    ],
  },
  {
    period: '10.2021 — 08.2022', role: 'QA Fullstack Engineer', company: 'Yandex', location: 'Moscow',
    highlights: [
      'Set up QA and release processes as the only QA on the team.',
      'Analyzed existing tests and features and created structured, prioritized test documentation.',
      'Developed automated tests using the Hermione framework based on WebdriverIO.',
      'Collaborated with cross-functional teams on integrations and joint releases.',
    ],
  },
  {
    period: '12.2018 — 09.2021', role: 'Software Developer in Test', company: 'Align Technology', location: 'Moscow',
    highlights: [
      'Developed automated tests for web and API services and designed supporting infrastructure.',
      'Refactored and modularized the test monorepository and introduced a new architecture.',
      'Mentored an intern to junior-level QA and wrote onboarding and technical documentation.',
    ],
  },
  {
    period: '08.2017 — 05.2018', role: 'Testing Department Consultant', company: 'National Payment Card System', location: 'Moscow',
    highlights: [
      'Contributed to the development of a new internal test automation framework.',
      'Managed testing team processes and supported a legacy test framework.',
      'Introduced and formalized git-flow practices within the team.',
    ],
  },
  {
    period: '12.2015 — 07.2017', role: 'Junior Software Developer in Test', company: 'Ingram Micro Cloud', location: 'Moscow',
    highlights: [
      'Implemented and maintained E2E and API test automation for new features.',
      'Analyzed test run results and compiled test reports.',
      'Created Jenkins pipelines and managed test environment deployments.',
    ],
  },
  {
    period: '03.2015 — 11.2015', role: 'Manual QA', company: 'Luxoft', location: 'Omsk',
    highlights: [
      'Performed smoke, regression, and integration testing.',
      'Created test designs, documented defects, and partnered with developers on resolution.',
    ],
  },
]
</script>

<template>
  <main>
    <nav class="nav shell" aria-label="Primary navigation">
      <a class="monogram" href="#top" aria-label="Back to top">AS</a>
      <div class="nav-links">
        <a href="#work">Work</a>
        <a href="#experience">Experience</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>

    <section id="top" class="hero shell">
      <div class="hero-copy">
        <p class="hero-name">Adelaida Sinikova <span>QA Automation Lead</span></p>
        <p class="eyebrow">TEAM LEADERSHIP · QUALITY STRATEGY · QA AUTOMATION</p>
        <h1>I build QA teams<br><span>that help products scale with confidence.</span></h1>
        <p class="intro">
          I build high-performing QA teams and turn testing into a reliable engineering practice.
          I set direction, grow people, and stay close enough to the technology to make pragmatic decisions.
        </p>
        <div class="hero-actions">
          <a class="button primary" href="#experience">Explore my experience <span>↓</span></a>
          <a class="button secondary" href="#contact">Let’s talk</a>
        </div>
      </div>
      <div class="portrait-wrap">
        <div class="portrait-glow"></div>
        <img src="/your-photo.webp" alt="Adelaida Sinikova" class="portrait" width="660" height="649" decoding="async" fetchpriority="high" />
        <div class="available"><span></span> Based in Spain · CET/CEST · Distributed teams worldwide</div>
      </div>
    </section>

    <section class="metrics shell" aria-label="Career highlights">
      <div><strong>11+</strong><span>years in QA</span></div>
      <div><strong>6</strong><span>direct reports across 5 product teams</span></div>
      <div><strong>9</strong><span>QA hires across my leadership roles</span></div>
      <div><strong>4h</strong><span>regression, down from 2 days</span></div>
    </section>

    <ProjectsSection id="work" />

    <section id="toolkit" class="section shell">
      <div class="section-heading">
        <p class="eyebrow">MY TOOLKIT</p>
        <h2>Leadership backed by engineering depth</h2>
        <p>I build strong QA teams, set a clear quality direction, and stay close enough to the technology to make pragmatic decisions.</p>
      </div>
      <div class="skill-grid">
        <article v-for="pillar in toolkitPillars" :key="pillar.title" class="skill-card" :class="{ featured: pillar.featured }">
          <div class="skill-card-header">
            <span class="skill-icon"><i class="pi" :class="pillar.icon"></i></span>
            <span class="skill-number">{{ pillar.number }}</span>
          </div>
          <h3>{{ pillar.title }}</h3>
          <p class="skill-description">{{ pillar.description }}</p>
          <div class="skill-groups">
            <div v-for="group in pillar.groups" :key="group.title" class="skill-group">
              <h4>{{ group.title }}</h4>
              <div class="tags"><span v-for="skill in group.skills" :key="skill">{{ skill }}</span></div>
            </div>
          </div>
        </article>
      </div>
    </section>

    <section id="experience" class="section shell experience-section">
      <div class="section-heading">
        <p class="eyebrow">CAREER JOURNEY</p>
        <h2>From hands-on testing to QA leadership</h2>
        <p>More than a decade of building automation, improving delivery, and growing people.</p>
      </div>
      <div class="timeline">
        <article v-for="job in experience" :key="`${job.company}-${job.period}`" class="timeline-item" :class="{ current: job.current }">
          <div class="timeline-date">{{ job.period }}</div>
          <div class="job-card">
            <div class="job-topline">
              <div class="job-identity">
                <div>
                  <h3>{{ job.role }}</h3>
                  <p class="company">{{ job.company }} <span>· {{ job.location }}</span></p>
                </div>
              </div>
              <span v-if="job.current" class="current-badge">CURRENT</span>
            </div>
            <ul><li v-for="item in job.highlights" :key="item">{{ item }}</li></ul>
          </div>
        </article>
      </div>
    </section>

    <section id="contact" class="contact shell">
      <div>
        <p class="eyebrow">LET’S CONNECT</p>
        <h2>Strong teams build quality<br>into everything they do.</h2>
      </div>
      <div class="contact-links">
        <a href="mailto:sinikowa@gmail.com"><i class="pi pi-envelope"></i><span>Email<small>sinikowa@gmail.com</small></span><b>↗</b></a>
        <a href="https://linkedin.com/in/adasinikova" target="_blank" rel="noopener noreferrer"><i class="pi pi-linkedin"></i><span>LinkedIn<small>in/adasinikova</small></span><b>↗</b></a>
        <a href="https://t.me/adasinikova" target="_blank" rel="noopener noreferrer"><i class="pi pi-telegram"></i><span>Telegram<small>@adasinikova</small></span><b>↗</b></a>
        <a href="https://github.com/asinka" target="_blank" rel="noopener noreferrer"><i class="pi pi-github"></i><span>GitHub<small>@asinka</small></span><b>↗</b></a>
      </div>
    </section>

    <footer class="shell"><span>© 2026 Adelaida Sinikova</span><span>Built with curiosity & care.</span></footer>
  </main>
</template>

<style scoped src="./MainPage.css"></style>
