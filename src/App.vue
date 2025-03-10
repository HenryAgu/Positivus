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
  <Navbar/>
  <h1 className="text-4xl bg-red-800">Hello</h1>
  <Footer/>
</template>