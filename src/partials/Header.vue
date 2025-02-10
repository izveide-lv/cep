<script setup>
import ThemeToggle from "./ThemeToggle.vue";
</script>

<template>
  <header
    class="absolute top-4 md:top-6 w-full z-30 pb-4 md:pb-6 border-b [border-image:linear-gradient(to_right,transparent,--theme(--color-indigo-300/.4),transparent)1] dark:[border-image:linear-gradient(to_right,transparent,--theme(--color-indigo-300/.16),transparent)1] shadow-[0_1px_0_0_--theme(--color-white/.2)] dark:shadow-none"
  >
    <div class="px-4 sm:px-6">
      <div class="max-w-3xl mx-auto">
        <div
          class="relative flex items-center justify-between gap-x-2 h-12 bg-linear-to-b from-white/90 to-white/70 dark:from-gray-700/80 dark:to-gray-700/70 rounded-lg px-3 shadow-sm"
        >
          <!-- Border with dots in corners -->
          <!-- Site branding -->
          <div class="flex-1">
            <!-- Logo -->
            <a href="/">🍳</a
            ><a href="https://izveide.lv"
              ><span
                class="font-bold dark:text-white text-2xl logo md:text-xl ml-2 rtl:ml-0 rtl:mr-2 self-center text-gray-900 whitespace-nowrap"
                >Izveide</span
              >
            </a>
          </div>

          <!-- Dark / Light mode toggle -->
          <ThemeToggle />
        </div>
      </div>
    </div>
  </header>
</template>
