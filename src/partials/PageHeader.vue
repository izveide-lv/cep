<script setup>
const props = defineProps({
  title: String,
  description: String,
});
</script>

<template>
  <div class="max-w-3xl mx-auto">
    <div class="text-center">
      <div class="relative flex items-center justify-center gap-4 mb-5">
        <div
          class="relative text-sm font-medium text-gray-700 bg-white dark:bg-gray-700 inline-flex rounded-lg whitespace-nowrap px-3 py-[3px] tracking-normal before:absolute before:inset-0 before:rounded-lg before:[background-image:linear-gradient(120deg,transparent_0%,--theme(--color-indigo-400/.12)_33%,--theme(--color-pink-400/.12)_66%,--theme(--color-amber-200/.12)_100%)] dark:before:[background-image:linear-gradient(120deg,--theme(--color-indigo-400/.16),--theme(--color-indigo-600/.16)_50%,transparent_100%)] shadow-sm"
        >
          <!-- Border with dots in corners -->
          <span
            class="relative text-gray-800 dark:text-transparent dark:bg-clip-text dark:bg-linear-to-b dark:from-indigo-500 dark:to-indigo-50"
          >
            <slot />
          </span>
        </div>
      </div>

      <h1
        class="font-outfit text-5xl md:text-6xl font-bold text-gray-800 dark:text-transparent dark:bg-clip-text dark:bg-linear-to-b dark:from-indigo-200 dark:to-gray-200 pb-4"
      >
        {{ title }}
      </h1>
      <p class="text-lg text-gray-700 dark:text-gray-400">
        {{ description }}
      </p>
    </div>
  </div>
</template>
