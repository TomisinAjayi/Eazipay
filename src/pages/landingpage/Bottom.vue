<template>
    <div class="bottom-background">
        <div class="flex">
            <div class="bottom-left">
                <h1 class="bottom-head">Get an Exclusive Demo of Eazipay</h1>
                <p class="bottom-note">Our greatest priority is to put you and your business first. Let’s show you how we can help.</p>
            </div>
            <div class="contact-form">
                <form class="">
                    <h2>First things first</h2>
                    <p>We want to serve you better. Tell us a bit about yourself or company</p>
                    <div className="flex buttonGroup">
                        <Button class="flex items-center justify-center buttonStyle individual" btnText="Individual" />
                        <Button class="flex items-center justify-center buttonStyle company" btnText="Company" />
                    </div>
                    <div class="form-input">
                        <input class="w-full focus:outline-none" id="fname" type="text" placeholder="First Name" />
                    </div>
                    <div class="form-input">
                        <input class="w-full focus:outline-none" id="lname" type="text" placeholder="Last Name" />
                    </div>
                    <div class="form-input">
                        <input class="w-full focus:outline-none   " id="email" type="email" placeholder="Email" />
                    </div>
                    <div class="form-input">
                        <input class="w-full focus:outline-none   " id="job" type="text" placeholder="Job Title" />
                    </div>
                    <div class="form-input">
                        <input class="w-full focus:outline-none   " id="size" type="text" placeholder="Company Size" />
                    </div>
                    <div class="flex items-center justify-between">
                        <Button class="w-full flex items-center justify-center btnStyle" btnText="Request Demo" />
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';
    import Button from '../../components/Button.vue';

    export default defineComponent({
        name: 'Bottom',
        components: {
            Button
        }
    });
</script>

<style scoped>
    .bottom-background {
        height: 947px;
        background-image: url(/bottom.png);
        background-repeat: no-repeat;
        background-size: cover;
        padding: 130px 0 113px 192px;
    }
    .bottom-left {
        display: flex;
        width: 552px;
        flex-direction: column;
        align-items: flex-start;
        margin-top: 195px;
    }
    .bottom-head {
        color: var(--new-styles-primary-eazi-green, #11453B);
        font-family: MADE Mellow PERSONAL USE;
        font-size: 64px;
        font-weight: 500;
        line-height: 72px; /* 112.5% */
        margin-bottom: 24px;
    }
    .bottom-note {
        width: 435px;
        margin-top: 24px;
        color: var(--new-styles-text-body-dark, #515251);
        font-size: 24px;
        font-weight: 400;
        line-height: 32px; /* 133.333% */
    }
    .contact-form {
        width: 552px;
        padding: 32px;
        border-radius: 32px;
        border: 1px solid var(--new-styles-grays-outline, #E7E8E7);
        background: var(--new-styles-shades-white, #FFF);
        box-shadow: 0px 20px 48px 0px rgba(170, 170, 170, 0.29);
    }
    .contact-form h2 {
        color: var(--new-styles-text-heading, #292A29);
        text-align: center;
        font-family: Aeonik;
        font-size: 28px;
        font-style: normal;
        font-weight: 700;
        line-height: 48px; /* 171.429% */
    }
    .contact-form p {
        width: 342px;
        margin: 12px auto 24px;
        color: var(--old-styles-main-text-color, #444);
        text-align: center;
        font-family: Aeonik;
        font-size: 18px;
        font-weight: 400;
        line-height: 24px; /* 133.333% */
    }
    .buttonGroup {
        display: flex;
        width: 488px;
        padding: 8px;
        align-items: center;
        justify-content: space-between;
        border-radius: 16px;
        border: 1.15px solid var(--new-styles-grays-outline, #E7E8E7);
        background: var(--new-styles-shades-white, #FFF);
        margin-bottom: 24px;
    }
    .buttonStyle {
        width: 225px;
        padding: 8px 11.504px;
        border-radius: 12px;
        gap: 8px;
        font-weight: 500;
        font-size: 16px;
        font-weight: 500;
        line-height: 24px;
    }
    .individual {
        color: #FFFFFF;
        background: var(--new-styles-primary-eazi-green, #11453B);
        box-shadow: 0px 8.871848106384277px 40.5570182800293px -2.534813642501831px rgba(24, 39, 75, 0.12), 0px 5.069627285003662px 13.941474914550781px -3.802220582962036px rgba(24, 39, 75, 0.12);
    }
    .company {
        color: var(--new-styles-text-body-dark, #515251);
        background: var(--new-styles-grays-bg, #F2F1F1);
    }
    .form-input {
        margin-top: 24px;
    }
    input {
        height: 48px;
        padding: 16px;
        border-radius: 16px;
        border: 1px solid var(--new-styles-text-body-light, #B5B6B5);
        background: var(--new-styles-shades-white, #FFF);
    }
    .btnStyle {
        margin-top: 28px;
        padding: 12px 28px;
        border-radius: 24px;
        color: var(--new-styles-shades-white, #FFF);
        font-size: 16px;
        font-weight: 500;
        line-height: 24px; /* 150% */
        background: var(--new-styles-primary-eazi-green, #11453B);
    }
</style>
  