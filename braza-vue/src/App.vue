<template>
  <div id="app">
    <Header />
    <main>
      <Home />
      <Services />
      <Empresa />
      <SobreNos />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Home from './components/Home.vue';
import Services from './components/Services.vue';
import Empresa from './components/Empresa.vue';
import SobreNos from './components/SobreNos.vue';

export default {
  components: {
    Header,
    Footer,
    Home,
    Services,
    Empresa,
    SobreNos,
  },
};
</script>

<style>
@import './assets/style.css';
</style>
