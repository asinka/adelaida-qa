<script setup lang="ts">

const skills = [
  "Python",
  "JavaScript (TypeScript)",
  "Playwright",
  "Selenium",
  "Git",
  "Github Actions",
  "Bamboo CI",
  "REST/GRPC API testing",
  "Cucumber",
  "Postman",
  "Linux CLI",
  "Allure"
];

</script>

<template>
  <div class="relative min-h-screen scroll-smooth">
    <!-- Фото в правом верхнем углу -->
    <img
      src="/your-photo.jpg"
      alt="My photo"
      class="absolute top-4 right-4 w-44 h-44 rounded-full shadow-2xl object-cover border-4 border-violet-950 z-10"
    />

    <h1 class="text-4xl font-bold text-rose-300 text-center mb-6">
      Hi, I’m Adelaida
    </h1>

    <section class="mb-16">
      <div class="text-lg font-medium text-center max-w-3xl mx-auto text-violet-950">
      <p>
        Senior QA Automation Engineer with 10 years of experience.
      </p>
      <p>
        I build and optimize test automation processes to boost product quality and release confidence. From launching QA from scratch to improving legacy workflows, I help teams deliver with precision and speed.
      </p>
      <p>
        Driven by curiosity and impact, I enjoy solving complex challenges, learning new tools, and crafting systems that are both reliable and elegant.
      </p>
      <p>
        In my free time, you’ll find me running, reading, playing piano, or catching up with friends.
      </p>
      </div>
    </section>

    <section class="mb-16 bg-violet-900 rounded-xl shadow-xl px-6 py-8">
      <h2 class="text-2xl font-semibold text-rose-300 text-center mb-6">Tech Stack</h2>
      <div class="flex flex-wrap justify-center gap-3">
        <span
          v-for="(skill, index) in skills"
          :key="index"
          class="rounded-full border border-rose-300 bg-rose-300 text-violet-950 py-2 px-5 shadow-md animate-fade-in text-sm md:text-base"
          :style="{ animationDelay: `${index * 0.05}s` }"
        >
          {{ skill }}
        </span>
      </div>
    </section>

    <section class="mb-16 bg-violet-900 rounded-xl shadow-xl px-6 py-8">
      <h2 class="text-2xl font-semibold text-rose-300 text-center mb-6">Experience Highlights</h2>
      <div class="grid gap-6">
        <Card>
          <CardContent class="p-6 text-left">
            <h3 class="text-lg font-bold text-rose-200">[06.2024 - 05.2025] QA Fullstack Engineer at Vivid Money, Remote</h3>
            <div class="text-violet-200">
              <p>
                Set up a QA process for a new product team from scratch.
              </p>
              <p>
                Expanded automated regression and feature test coverage using Playwright (TypeScript).
              </p>
              <p>
                Revived and scaled mobile test automation after years of inactivity.
              </p>
              <p>
                Evaluated AI-based tools for mobile E2E automation in collaboration with an external team.
              </p>
              <p>
                Increased gRPC API test coverage and manually tested new API and mobile features.
              </p>
              <p>
                Maintained up-to-date test documentation.
              </p>
            </div>
          </CardContent>
        </Card>
        <Card>
          <CardContent class="p-6 text-right">
            <h3 class="text-lg font-bold text-rose-200">[02.2023 - 05.2024] QA Automation Engineer / Team Lead at Trak Services, Remote</h3>
            <div class="text-violet-200">
              <p>
                Built test automation from the ground up as the first QA automation engineer on the team.
              </p>
              <p>
                Achieved 40 - 80% test coverage across multiple projects, leading one to 80% coverage under my guidance.
              </p>
              <p>
                Reduced regression testing time from 2 days to 4 hours through automation.
              </p>
              <p>
                Mentored manual testers in automation basics and onboarded new QA automation engineers.
              </p>
              <p>
                Conducted interviews and managed task planning and resource allocation for the automation team.
              </p>
              <p>
                Initiated regular QA team meetings and drove continuous process improvements.
              </p>
            </div>
          </CardContent>
        </Card>
        <Card>
          <CardContent class="p-6 text-left">
            <h3 class="text-lg font-bold text-rose-200">[09.2022 - 01.2023] Software Developer in Test at Lightspeed, Tbilisi</h3>
            <div class="text-violet-200">
              <p>
                Expanded E2E test coverage using Playwright and Appium.
              </p>
              <p>
                Structured test runs and reports by feature for better traceability.
              </p>
              <p>
                Monitored and maintained automated test results for stability and relevance.
              </p>
              <p>
                Enhanced internal testing framework and infrastructure.
              </p>
            </div>
          </CardContent>
        </Card>
        <Card>
          <CardContent class="p-6 text-right">
            <h3 class="text-lg font-bold text-rose-200">[10.2021 - 08.2022] QA Fullstack Engineer at andex, Moscow</h3>
            <div class="text-violet-200">
              <p>
                Set up QA and release processes as the first automation engineer in the team.
              </p>
              <p>
                Analyzed existing tests and features; created structured, prioritized test documentation.
              </p>
              <p>
                Developed automated tests using the Hermione framework (based on WebdriverIO).
              </p>
              <p>
                Collaborated with cross-functional teams for integration and joint releases.
              </p>
            </div>
          </CardContent>
        </Card>
        <Card>
          <CardContent class="p-6 text-left">
            <h3 class="text-lg font-bold text-rose-200">[12.2018 - 09.2021] Software Developer in Test at Align Technology, Moscow</h3>
            <div class="text-violet-200">
              <p>
                Developed automated tests for web and API services; designed supporting infrastructure.
              </p>
              <p>
                Refactored and modularized test monorepository; introduced a new architecture.
              </p>
              <p>
                Mentored an intern to junior-level QA; wrote onboarding and technical documentation.
              </p>
            </div>
          </CardContent>
        </Card>
        <Card>
          <CardContent class="p-6 text-right">
            <h3 class="text-lg font-bold text-rose-200">[08.2017 - 05.2018] Testing Department Consultant at National Payment Card System, Moscow</h3>
            <div class="text-violet-200">
              <p>
                Contributed to the development of a new internal test automation framework.
              </p>
              <p>
                Managed testing team processes and supported a legacy test framework.
              </p>
              <p>
                Introduced and formalized git-flow practices within the team.
              </p>
            </div>
          </CardContent>
        </Card>
        <Card>
          <CardContent class="p-6 text-left">
            <h3 class="text-lg font-bold text-rose-200">[12.2015 - 07.2017] Junior Software Developer in Test at Ingram Micro Cloud, Moscow</h3>
            <div class="text-violet-200">
              <p>
                Implemented and maintained E2E and API test automation for new features.
              </p>
              <p>
                Analyzed test run results and compiled test reports.
              </p>
              <p>
                Created Jenkins pipelines and managed test environment deployments.
              </p>
            </div>
          </CardContent>
        </Card>
        <Card>
          <CardContent class="p-6 text-right">
            <h3 class="text-lg font-bold text-rose-200">[03.2015 - 11.2015] Manual QA at Luxoft, Omsk </h3>
            <div class="text-violet-200">
              <p>
                Performed manual smoke, regression, and integration testing.
              </p>
              <p>
                Created test designs and documented defects; worked closely with developers to resolve issues.
              </p>
            </div>
          </CardContent>
        </Card>
      </div>
    </section>

    <section class="mb-16 bg-violet-900 rounded-xl shadow-xl px-6 py-8">
      <h2 class="text-2xl font-semibold text-rose-300 text-center mb-6">Contacts</h2>
      <div class="flex flex-col sm:grid sm:grid-cols-3 gap-4 text-center">
        <a href="mailto:sinikowa@gmail.com" class="inline-flex justify-center items-center px-4 py-2 border border-violet-300 rounded-md shadow-sm text-sm font-medium text-pink-200 bg-violet-900 hover:bg-pink-400">
          <Mail class="w-4 h-4 mr-2" /> sinikowa@gmail.com
        </a>
        <a href="https://linkedin.com/in/adasinikova" target="_blank" class="inline-flex justify-center items-center px-4 py-2 border border-violet-300 rounded-md shadow-sm text-sm font-medium text-pink-200 bg-violet-900 hover:bg-pink-400">
          <svg class="w-4 h-4 mr-2" fill="currentColor" viewBox="0 0 24 24"><path d="M19 0h-14c-2.762 0-5 2.238-5 5v14c0 2.762 2.238 5 5 5h14c2.762 0 5-2.238 5-5v-14c0-2.762-2.238-5-5-5zm-11 19h-3v-10h3v10zm-1.5-11.268c-.966 0-1.75-.784-1.75-1.75s.784-1.75 1.75-1.75 1.75.784 1.75 1.75-.784 1.75-1.75 1.75zm13.5 11.268h-3v-5.604c0-1.337-.025-3.063-1.867-3.063-1.868 0-2.154 1.46-2.154 2.97v5.697h-3v-10h2.881v1.367h.041c.401-.761 1.379-1.563 2.839-1.563 3.036 0 3.598 2 3.598 4.598v5.598z"/></svg>
          linkedin.com/in/adasinikova
        </a>
        <a href="https://github.com/asinka" target="_blank" class="inline-flex justify-center items-center px-4 py-2 border border-violet-300 rounded-md shadow-sm text-sm font-medium text-pink-200 bg-violet-900 hover:bg-pink-400">
          <Github class="w-4 h-4 mr-2" /> github.com/asinka
        </a>
      </div>
    </section>
  </div>
</template>

<style scoped>
@keyframes fade-in {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-fade-in {
  animation: fade-in 0.5s ease-in-out both;
}
</style>
