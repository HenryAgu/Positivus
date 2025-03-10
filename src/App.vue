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
  <main class="container mx-auto px-5 2xl:px-14">
    <Navbar />
    <div class="min-h-screen">1</div>
    <Footer />
  </main>
</template>
