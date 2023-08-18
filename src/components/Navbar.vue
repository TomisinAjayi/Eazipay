<template>
  <nav class="navigation">
    <div class="container mx-auto flex justify-between items-center">
      <div class="flex items-center justify-between" style="width: 634px">
        <img src="/Logo.png" alt="Logo" class="" />
        <ul class="flex space-x-4 justify-evenly" style="width: 442px">
          <li><a href="#" class="">Individual</a></li>
          <li><a href="#" class="">Business</a></li>
          <li><a href="#" class="">Pricing</a></li>
          <li><a href="#" class="">Set your payroll</a></li>
        </ul>
      </div>
      <div class="flex items-center justify-between" style="width: 360px">
        <Button class='buttonstyle login' btnText='Log in' />
        <Button class='buttonstyle register' btnText='Register' />  
      </div>    
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Button from './Button.vue';

export default defineComponent({
  name: 'Navbar',
  components: {
    Button
  }
});
</script>

<style scoped>
  .navigation {
    height: 80px;
    padding: 20px 192px 20px 192px;
  }
.buttonstyle {
        width: 168px;
        height: 40px;
        padding: 10px 32px;
        border-radius: 24px;
        gap: 8px;
        font-weight: 500;
    }
    .login {
        border: 1px solid #11453B;
        color: #11453B;
    }
    .register {
        background-color: #11453B;
        color: #FFFFFF;
    }
</style>
