<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    Navbar,
    Footer,
  },
};
</script>

<template>
  <main class="mx-auto px-0 xl:px-10 2xl:px-14 bg-white">
    <Navbar />
    <div class="min-h-screen">1</div>
    <Footer />
  </main>
</template>
