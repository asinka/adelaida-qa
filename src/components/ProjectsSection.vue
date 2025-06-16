<template>
  <section class="mb-16 bg-violet-900 rounded-xl shadow-xl px-6 py-8">
    <h2 class="text-2xl font-semibold text-rose-300 text-center mb-6">Projects & Case Studies</h2>
    <div class="grid gap-6 sm:grid-cols-2">
      <div
        v-for="(project, index) in projects"
        :key="index"
        class="bg-white/5 rounded-xl p-6 border border-rose-200 hover:shadow-lg transition"
      >
        <h3 class="text-lg font-bold text-rose-200 mb-2">{{ project.icon }} {{ project.title }}</h3>
        <p class="text-violet-200 italic mb-1">{{ project.company }}</p>
        <p class="text-violet-100">{{ project.description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const projects = [
  {
    title: "CI & Test Automation from Scratch",
    company: "Trak Services (2023–2024)",
    description:
      "Built test automation from the ground up, reached 80% test coverage, and reduced regression time from 2 days to 4 hours. Mentored new engineers and led QA process design.",
    icon: "🚀",
  },
  {
    title: "Test Suite Refactoring & Scalability",
    company: "Align Technology (2018–2021)",
    description:
      "Refactored a monorepo, implemented modular architecture, mentored an intern, and wrote onboarding documentation for automation processes.",
    icon: "🔄",
  },
  {
    title: "Reviving Mobile Automation",
    company: "Vivid Money (2024–Present)",
    description:
      "Restarted and expanded mobile E2E testing after years of inactivity. Introduced AI-based automation tools and increased gRPC API test coverage.",
    icon: "📱",
  },
  {
    title: "Mentorship & Team Enablement",
    company: "Trak / Align",
    description:
      "Trained manual testers in automation, onboarded new QAs, organized team meetings, and drove process improvements across projects.",
    icon: "🧑‍🏫",
  },
];
</script>
