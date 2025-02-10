<script setup>
import BgShapes from "../partials/BgShapes.vue";
import VerticalLines from "../partials/VerticalLines.vue";
import Header from "../partials/Header.vue";
import PageHeader from "../partials/PageHeader.vue";
import SubscribeForm from "../partials/SubscribeForm.vue";
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
        <div class="pt-32 pb-12 md:pt-28 md:pb-20">
          <div class="px-4 sm:px-6">
            <PageHeader
              class="mb-12 px-4"
              title="Iegūsti bezmaksas mājaslapas novērtējumu"
              description="Ievadi savu e-pastu un mājaslapas adresi, lai saņemtu individuāli veidotu pārskatu par vietnes 🖱️lietojamību, ⚡ātrdarbību, 🎨dizainu un 🍪sīkdatnēm."
            >
              <a
                href="https://www.threads.net/@armandslei/post/DFxB_b0oK5K"
                target="_blank"
                >👉 Apskatītas jau 50+ mājaslapas</a
              >
            </PageHeader>

            <SubscribeForm />
          </div>
        </div>
      </section>
    </main>

    <!-- Site footer -->
    <Footer />
  </div>
</template>
