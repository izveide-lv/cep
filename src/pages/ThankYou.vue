<script setup>
import BgShapes from "../partials/BgShapes.vue";
import VerticalLines from "../partials/VerticalLines.vue";
import Header from "../partials/Header.vue";
import PageHeader from "../partials/PageHeader.vue";
import Footer from "../partials/Footer.vue";
</script>

<template>
  <div
    class="relative flex flex-col min-h-screen overflow-hidden supports-[overflow:clip]:overflow-clip"
  >
    <BgShapes />
    <VerticalLines />

    <!-- Site header -->
    <Header />

    <!-- Page content -->
    <main class="grow">
      <section>
        <div class="pt-32 pb-12 md:pb-20">
          <div class="px-4 sm:px-6">
            <PageHeader
              class="mb-8"
              title="Tavs pieteikums ir saņemts!"
              description="Parasti izvērtējums tiek veikts vienas darba dienas laikā. Gaidi e-pastu no Armanda!"
              >🧡🧡🧡🧡🧡</PageHeader
            >
            <!-- Cards -->
            <div class="max-w-xs md:max-w-6xl mx-auto">
              <div
                class="grid md:grid-cols-2 gap-6 xl:gap-9 xl:mx-8 max-md:-mx-3"
              >
                <!-- Card -->
                <div
                  class="flex flex-col rounded-lg bg-linear-to-tr from-white/70 to-white/50 dark:bg-linear-to-b dark:from-gray-700/50 dark:to-gray-700/40 p-5"
                >
                  <div class="grow mb-3">
                    <div
                      class="font-inter-tight font-semibold text-gray-800 dark:text-gray-200 mb-1"
                    >
                      E-pasts
                    </div>
                    <p class="text-sm text-gray-600 dark:text-gray-500">
                      Ja vēlies sazināties ar mani par jebkādiem jautājumiem,
                      kas saistīti ar mājaslapu izveidi, vari rakstīt uz
                      e-pastu.
                    </p>
                  </div>
                  <div class="flex items-center space-x-2.5">
                    <svg
                      class="shrink-0 fill-indigo-500/80"
                      width="16"
                      height="16"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M8 0a8 8 0 1 0 3.2 15.335l.916-.4-.8-1.833-.916.4A6 6 0 1 1 14 8v1a1 1 0 1 1-2 0V8a4.033 4.033 0 1 0-1.286 2.92A2.987 2.987 0 0 0 16 9V8a8.009 8.009 0 0 0-8-8Zm0 10a2 2 0 1 1 0-4 2 2 0 0 1 0 4Z"
                      />
                    </svg>
                    <a
                      href="mailto:armands@labojam.lv"
                      class="text-sm text-gray-800 dark:text-gray-200 hover:underline"
                    >
                      armands@labojam.lv</a
                    >
                  </div>
                </div>
                <!-- Card -->
                <div
                  class="flex flex-col rounded-lg bg-linear-to-tr from-white/70 to-white/50 dark:bg-linear-to-b dark:from-gray-700/50 dark:to-gray-700/40 p-5"
                >
                  <div class="grow mb-3">
                    <div
                      class="font-inter-tight font-semibold text-gray-800 dark:text-gray-200 mb-1"
                    >
                      Telefons
                    </div>
                    <p class="text-sm text-gray-600 dark:text-gray-500">
                      Ja vēlies, vari arī piezvanīt vai
                      <a href="https://wa.me/+37125226526" class="underline"
                        >atrakstīt WhatsApp</a
                      >.
                    </p>
                  </div>
                  <div class="flex items-center space-x-2.5">
                    <svg
                      class="shrink-0 fill-indigo-500/80"
                      width="12"
                      height="16"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M10 0H2a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h8a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2ZM2 13V3h8v10H2Z"
                      />
                    </svg>
                    <a
                      href="tel:+37125226526"
                      class="text-sm text-gray-800 dark:text-gray-200 hover:underline"
                    >
                      +371 25226526
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>

    <!-- Site footer -->
    <Footer />
  </div>
</template>
