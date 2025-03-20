<script setup>
import ResumeButton from "./ResumeButton.vue";
</script>

<template>
  <header
    class="sticky top-0 z-50 flex flex-wrap w-full py-6 text-sm md:px-16 bg-slate-900 sm:justify-start sm:flex-nowrap"
  >
    <nav
      class="max-w-[85rem] w-full mx-auto px-4 sm:flex sm:items-center sm:justify-between"
      aria-label="Global"
    >
      <div class="flex items-center justify-between">
        <a
          href="/"
          class="flex-none text-lg font-extrabold tracking-wide font-fira text-cyan-300"
        >
          Portfolio
        </a>
        <div class="sm:hidden">
          <button
            type="button"
            class="inline-flex items-center justify-center p-2 text-xs font-bold border rounded-lg shadow-sm text-lightText border-slate-600 bg-slate-900 hs-collapse-toggle gap-x-2 hover:bg-slate-800 disabled:opacity-50 disabled:pointer-events-none"
            data-hs-collapse="#navbar-collapse-with-animation"
            aria-controls="navbar-collapse-with-animation"
            aria-label="Toggle navigation"
          >
            <svg
              class="flex-shrink-0 hs-collapse-open:hidden size-4"
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <line x1="3" x2="21" y1="6" y2="6" />
              <line x1="3" x2="21" y1="12" y2="12" />
              <line x1="3" x2="21" y1="18" y2="18" />
            </svg>
            <svg
              class="flex-shrink-0 hidden hs-collapse-open:block size-4"
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path d="M18 6 6 18" />
              <path d="m6 6 12 12" />
            </svg>
            Menu
          </button>
        </div>
      </div>
      <div
        id="navbar-collapse-with-animation"
        class="hidden overflow-hidden transition-all duration-300 hs-collapse basis-full grow sm:block"
      >
        <div class="w-full">
          <ul
            class="flex flex-col items-start w-full pl-3 mt-5 space-y-5 text-xs font-semibold sm:space-y-0 sm:items-center sm:space-x-8 sm:flex-row sm:justify-end sm:mt-0 sm:ps-5"
          >
            <li class="hidden md:block">
              <ResumeButton />
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>
