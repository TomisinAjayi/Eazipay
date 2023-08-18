<template>
    <div class="works" style="">
        <div>
            <h1 class="text-center">How Eazipay Works</h1>
            <p class="text-center">Get started in 3 simple steps.</p>
        </div>
        <div style="padding-left: 149px;">
            <!-- image  -->
            <div class="circle big-circle">
                <div class="circle medium-circle">
                    <div class="circle smaller-circle">
                        <img src="https://s3-alpha-sig.figma.com/img/afa0/c1e6/561787658c7d935e98021ba603c76f08?Expires=1693180800&Signature=KuxMDqeeLDUOBKCjxVju~iSpBNxcLtv2VxGKe85K-opRDi5jkKodNQTThEPO5mQvlnhppqiDeFAYXXvPiIkHbavc8n84YSh~7gXr488fj-73RoIJj3hD4p0~njHbT7BiuFMC-jbMiq5rRQ8kVYQbagWh8rDnMXBKhu0m-0QJMOG8Ul29W0Q1sc0NWV4tE3OI87ay~Lno11jIYOd4bwWgjzjkfNUZmBtwqo1Hn6FX2K~ahgh96gmzhcLzvicFwgpuNtRwrQFqEDgvp8OckKw-mKSyganILaBFGhUcmW0cbaUP1nJsVcU87jSd93~O2gyY7fcYmqbnri0CXPqe6G-zfg__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4" alt="Logo" class="onboarding-phone" />
                    </div>
                </div>
            </div>
            <!-- steps  -->
            <div>

            </div>
        </div>
    </div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';

    export default defineComponent({
        name: 'Works',
        components: {
            
        }
    });
</script>

<style scoped>
    .works {
        padding-top: 93.07px;
        padding-bottom: 138.41px;
        background-color: #fff;
    }
    .works h1 {
        margin-bottom: 16px;
        color: var(--new-styles-primary-eazi-green, #11453B);
        font-family: MADE Mellow PERSONAL USE;
        font-size: 56px;
        font-weight: 500;
        line-height: 64px; /* 114.286% */
    }
    .works p {
        color: var(--new-styles-text-body-dark, #515251);
        font-size: 28px;
        font-weight: 400;
        line-height: 36px; /* 128.571% */
    }
    .circle {
        border-radius: 50%;
    }
    .big-circle {
        margin-top: 132px;
        position: relative;
        height: 577px;
        width: 577px;
        border: 0.187px solid var(--new-styles-primary-eazi-green, #11453B);
        background: var(--new-styles-primary-mint-light, #F0F7EB);
    }
    .medium-circle {
        position: absolute;
        background: var(--new-styles-primary-mint, #D9EBCD);
        width: 518.158px;
        height: 518.158px;
        top: 31%;
        left: 31%;
        margin: -150px 0px 0px -150px;
    }
    .smaller-circle {
        position: absolute;
        top: 35%;
        left: 35%;
        margin: -150px 0px 0px -150px;
        width: 450.897px;
        height: 450.897px;
        background: var(--new-styles-primary-eazi-green, #11453B);
    }
    .onboarding-phone {
        position: absolute;
        top: -25%;
        left: 11%;
        border-radius: 60px;
        width: 347.614px;
        height: 682px;
    }
</style>


  