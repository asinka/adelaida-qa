<script setup lang="ts">
const projects = [
  { number: '01', result: '1 → 6', label: 'QA team growth', title: 'Scaling QA through product growth', company: 'Alix Inc · 2025—Present', description: 'Joined as the first QA automation engineer when engineering operated as one large team with fragmented testing processes. Built the automation foundation, personally hired five QA engineers, and guided the QA side of the transition to five product teams—defining how testing ownership and resources were distributed across them.' },
  { number: '02', result: '2d → 4h', label: 'regression time', title: 'From first tests to team leadership', company: 'Trak Services · 2023—2024', description: 'Joined as the first QA automation engineer and built the initial framework and automated tests from scratch. Hired half of the automation team, then led its work as test coverage grew to 40–80% across projects and ongoing suite maintenance became a shared team responsibility.' },
  { number: '03', result: 'Intern → Junior', label: 'mentorship outcome', title: 'Technical leadership through enablement', company: 'Align Technology · 2018—2021', description: 'Refactored the test monorepo into a modular architecture and documented the new approach so others could work with it confidently. Mentored an intern through hands-on guidance and structured onboarding, supporting their growth into a junior QA engineer.' },
]
</script>

<template>
  <section class="projects section shell">
    <div class="section-heading">
      <p class="eyebrow">SELECTED IMPACT</p>
      <h2>Work measured in outcomes</h2>
      <p>Three examples of turning quality challenges into sustainable engineering systems.</p>
    </div>
    <div class="project-grid">
      <article v-for="project in projects" :key="project.number" class="project-card">
        <div class="project-number">{{ project.number }}</div>
        <div class="result"><strong>{{ project.result }}</strong><span>{{ project.label }}</span></div>
        <div class="project-copy">
          <h3>{{ project.title }}</h3>
          <p class="company">{{ project.company }}</p>
          <p>{{ project.description }}</p>
        </div>
      </article>
    </div>
  </section>
</template>

<style scoped src="./ProjectsSection.css"></style>
