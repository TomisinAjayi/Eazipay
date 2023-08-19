<template>
  <div id="app">
    <div v-if="windowWidth < 600">
      <p>No Mobile View. Open this page on a larger screen.</p>
    </div>
    <div v-else>
      <Main />
    </div>

  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Main from './main.vue';

export default defineComponent({
  name: 'App',
  components: {
    Main
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