<template>
    <Header />
    <Hero />
    <Works />
    <Payment />
    <Bottom />
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Header from './Header.vue';
import Hero from './Hero.vue';
import Payment from './Payment.vue';
import Works from './Works.vue';
import Bottom from './Bottom.vue';

export default defineComponent({
name: 'Landingpage',
components: {
    Header,
    Hero,
    Payment,
    Works,
    Bottom
}
});
</script>

<style scoped>
</style>
  