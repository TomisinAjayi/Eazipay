<template>
  <div id="app">
    <div v-if="windowWidth < 600">
      <p>No Mobile View. Open this page on a larger screen.</p>
    </div>
    <div v-else>
      <!-- <Navbar />
      <Landingpage /> -->
      <Dashboard />
      <!-- <Footer /> -->
    </div>

  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
// import Navbar from './components/Navbar.vue';
// import Landingpage from './pages/landingpage/index.vue';
import Dashboard from './pages/dashboard/index.vue';
// import Footer from './components/Footer.vue';
// import "./assets/fonts/Aeonik-/Aeonik-Medium.otf";

export default defineComponent({
  name: 'App',
  components: {
    // Navbar,
    // Landingpage,
    Dashboard,
    // Footer
  },
  data() {
    return {
      windowWidth: window.innerWidth, // Initial value based on window width
    };
  },
  created() {
    // Attach an event listener to update the windowWidth when the window is resized
    window.addEventListener('resize', this.handleResize);
  },
  destroyed() {
    // Remove the event listener when the component is destroyed
    window.removeEventListener('resize', this.handleResize);
  },
  methods: {
    handleResize() {
      this.windowWidth = window.innerWidth; // Update windowWidth when window is resized
    },
  },
});
</script>


<style>
  #app {
    font-family: Aeonik;
    background-image: url(/gradient.png);
    background-repeat: no-repeat;
  }
</style>