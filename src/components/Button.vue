<template>
  <button id='btn' class="flex items-center justify-center">
    {{btnText}}
  </button>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue';

export default defineComponent({
    name: 'Button',
    props: {
        btnText: {
            type: String as PropType<string>,
            required: true
        }
    }
});
</script>

<style scoped>
    
</style>