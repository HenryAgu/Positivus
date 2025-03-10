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
  <main className="container mx-auto px-5 xl:px-14">
    <Navbar />
    <div className="min-h-screen">1</div>
    <Footer />
  </main>
</template>
