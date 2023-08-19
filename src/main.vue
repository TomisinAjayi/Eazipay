<template>
    <div>
      <div>
        <Navbar />
        <Landingpage />
        <Footer />
      </div>
      <div>
        <!-- <Dashboard /> -->
      </div>
    </div>
  </template>
  
<script lang="ts">
    import { defineComponent } from 'vue';
    import Navbar from './components/Navbar.vue';
    import Landingpage from './pages/landingpage/index.vue';
    // import Dashboard from './pages/dashboard/index.vue';
    import Footer from './components/Footer.vue';
    import "./assets/fonts/Aeonik-/Aeonik-Medium.otf";

    export default defineComponent({
    name: 'Main',
    components: {
        Navbar,
        Landingpage,
        // Dashboard,
        Footer
    }
    });
</script>
  
  
<style>
</style>