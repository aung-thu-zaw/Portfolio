<script setup>
import ExperienceSection from "./components/ExperienceSection.vue";
import ProfileSection from "./components/ProfileSection.vue";
import AboutMeSection from "./components/AboutMeSection.vue";
import ProjectSection from "./components/ProjectSection.vue";
import ResumeButton from "./components/ResumeButton.vue";
import Spotlight from "./components/Spotlight.vue";
import Navbar from "./components/Navbar.vue";
</script>

<template>
  <div class="bg-slate-900 max-h-screen overflow-scroll min-w-screen">
    <div class="fixed z-50 block bottom-10 right-6 md:hidden">
      <ResumeButton />
    </div>

    <Navbar />

    <Spotlight />

    <section class="py-10 md:py-20">
      <div
        class="container relative flex flex-col items-start justify-between h-full px-8 mx-auto space-y-10 md:space-y-0 md:space-x-5 md:flex-row"
      >
        <ProfileSection />

        <div class="w-full h-full space-y-10 md:w-1/2">
          <AboutMeSection />

          <hr />

          <ExperienceSection />

          <hr />

          <ProjectSection />
        </div>
      </div>
    </section>
  </div>
</template>
