<template>
  <div class="container mx-auto px-1 md:p-5">
    <Header />
    <main-view />
    <Footer />
  </div>
</template>
<script setup>
  import Header from './components/Header.vue';
  import Footer from './components/Footer.vue';
  import mainView from './views/mainView.vue';
</script>