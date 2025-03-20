<script setup>
import SocialLinkButton from "./SocialLinkButton.vue";
import EmailButton from "./EmailButton.vue";
</script>

<template>
  <div
    class="flex flex-col justify-between w-full max-h-screen space-y-14 md:space-y-20 md:items-start md:sticky md:top-44 md:w-1/2"
  >
    <div class="space-y-5 text-center md:text-left">
      <p class="font-semibold uppercase text-md text-lightText">
        Hi There 👋🏼 , I'm
      </p>

      <h1 class="text-6xl font-extrabold text-lightText">Aung Thu Zaw</h1>

      <p class="text-lg font-semibold text-lightText">
        Full Stack Web Developer
      </p>

      <p
        class="text-md text-slate-400 max-w-[500px] mx-auto md:mx-0 text-center md:text-left !mb-14"
      >
        Passionate about crafting high-performance web applications, I
        specialize in building seamless and scalable solutions using modern web
        technologies. From intuitive front-end experiences to robust back-end
        architectures, I turn ideas into reality with clean code and efficient
        problem-solving.
      </p>

      <div class="flex items-center justify-center w-full md:justify-start">
        <ul
          class="flex flex-row items-center justify-between space-x-5 text-xs font-bold uppercase md:flex-col md:space-x-0 md:space-y-5 md:items-start"
        ></ul>
      </div>
    </div>

    <!-- Social Media  -->
    <div
      class="flex items-center justify-center w-full space-x-3 md:justify-start"
    >
      <!-- <SocialLinkButton
        href="https://www.facebook.com/aungthuzaw322/"
        icon="fa-brands fa-facebook"
        tooltip="Connect with me on Facebook"
      /> -->

      <SocialLinkButton
        href="https://github.com/aung-thu-zaw"
        icon="fa-brands fa-github"
        tooltip="Explore my projects on GitHub"
      />

      <EmailButton
        icon="fa-solid fa-envelope"
        tooltip="Get in touch via email ( aungthuzaw003@gmail.com )"
      />
    </div>
  </div>
</template>
