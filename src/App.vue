<script setup>
import BackToTop from "./components/button/BackToTop.vue";
import Footer from "./components/footer/Footer.vue";
import Hero from "./components/main/Hero.vue";
import Menu from "./components/main/Menu.vue";
import Navigation from "./components/Navigation.vue";
</script>

<template>
  <header>
    <Navigation />
  </header>
  <main>
    <Hero />
    <Menu />
  </main>
  <footer>
    <Footer />
  </footer>


  <BackToTop />
</template>

<style scoped>
</style>
