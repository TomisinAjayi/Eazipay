<template>
    <div class="logo-bg-image flex justify-center items-center">
        <img src="/logo-white.png" alt="Logo" class="" />
    </div>
    <div style="padding: 20px 40px">  
        <li>Dashboard</li>
        <li>Wallet</li>
        <li>Employee Management</li>
        <li>Payroll</li>
        <li>Compliance</li>
        <li>Quick Loan</li>
        <li>Book Keeping</li>
        <li>Support</li>
        <li>Settings</li>
    </div>

</template>

<script lang="ts">
    import { defineComponent } from 'vue';

    export default defineComponent({
        name: 'Sidebar',
        components: {
            
        }
    });
</script>

<style>
    .logo-bg-image {
        background-image: url(/sidebar.png);
        background-repeat: no-repeat;
        background-size: cover;
        width: 321px;
        height: 150.7px;
    }
</style>