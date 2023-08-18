<template>
	<body>
        <div class="topnav flex items-center justify-between">
            <img src="/Company_Logo.png" alt="Company Logo" class="" />
            <div class="flex">
                <div class="relative">
                    <div
                      class="notification-number absolute z-10 inline-block -translate-y-1/2 translate-x-2/4 flex items-center justify-center">
                      7
                    </div>
                    <button type="button" class="relative rounded-full p-1 text-gray-400">
                        <span class="absolute -inset-1.5"></span>
                        <span class="sr-only">View notifications</span>
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
                          <path stroke-linecap="round" stroke-linejoin="round" d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0" />
                        </svg>
                    </button>
                </div>
                <div class="flex">
                    <div class="flex">
                        <button type="button" class="relative flex rounded-full" id="user-menu-button" aria-expanded="false" aria-haspopup="true">
                            <span class="absolute -inset-1.5"></span>
                            <span class="sr-only">Open user menu</span>
                            <img class="h-8 w-8 rounded-full" src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
                        </button>
                        <div>
                            <p>Kalu Abasiama</p>
                            <p>Admin</p>
                        </div>
                    </div>
                    <div class="flex items-end">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="arrowRight">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                        </svg>   
                    </div>                   
                </div>
            </div>
        </div>
        
        <!-- Mobile menu, show/hide based on menu state. -->
        <div class="sm:hidden" id="mobile-menu">
            <div class="space-y-1 px-2 pb-3 pt-2">
            <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
            <a href="#" class="bg-gray-900 text-white block rounded-md px-3 py-2 text-base font-medium" aria-current="page">Dashboard</a>
            <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Team</a>
            <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Projects</a>
            <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Calendar</a>
            </div>
        </div>
        
        <div>
            <div>
                <h1>Welcome  Abasiama</h1>
                <p>Pay and manage your employee in minutes</p>
            </div>
            <div>
                <div class="">
                    <div class="flex justify-between">
                        <div>
                            <h2>Wallet Balance</h2>
                            <p>N12,560,078.00</p>
                        </div>
                        <Button class='buttonstyle' btnText='Fund Wallet' />
                    </div>
                    <div class="flex">
                        <div class="wallet-options flex justify-center items-center">
                            <p>Add Employee</p>
                        </div>
                        <div class="wallet-options flex justify-center items-center">
                            <p>Pay Salaries</p>
                        </div>
                        <div class="wallet-options flex justify-center items-center">
                            <p>Pay Compliances</p>
                        </div>
                        <div class="wallet-options flex justify-center items-center">
                            <p>Quick Loan</p>
                        </div>
                    </div>
                </div>
                <!-- payroll  -->
                <div>
    
                </div>
            </div>
        </div>
        <!-- recent activites  -->
        <div>
            <Recent />
        </div>
    </body>
    
</template>

<script lang="ts">
    import { defineComponent } from 'vue';
    import Button from '../../components/Button.vue';
    import Recent from './Recent.vue';

    export default defineComponent({
        name: 'DashboardContent',
        components: {
            Button,
            Recent
        }
    });
</script>

<style>
    body {
        margin-left: 136px;
    }
    .topnav {
        width: 81.5vw;
        padding: 11px 48px 11px 61px;
        background-color: #FFFFFF;
    }
    .notification-number {
        background-color: #C92F02;
        width: 16px;
        height: 16px;
        border-radius: 100px;
        font-weight: 700;
        font-size: 10px;
        line-height: 12px;
        color: #FFFFFF;
        right: 8px;
        bottom: 26px;
    }
    .arrowRight {
        color: #898989;
        height: 24px;
        width: 24px;
        font-weight: bold;
    }
    .buttonstyle {
        width: 132px;
        height: 44px;
        padding: 12px 28px;
        border-radius: 24px;
        gap: 8px;
        font-weight: 500;
        border: 1px solid #D9EBCD;
        color: #11453B;
        background-color: #D9EBCD;
        font-size: 14px;
        line-height: 20px;
        letter-spacing: 0.1px;
    }
    .wallet-options {
        width: 168.5px;
        height: 112px;
        border-radius: 24px;
        border: 1px solid #E7E8E7;
        box-shadow: 0px 9px 18px 0px #AAAAAA26;
        gap: 16px;
        color: #515251;
    }
</style>


