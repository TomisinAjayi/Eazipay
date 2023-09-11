<template>
    <div class="hero">
        <h1 class="text-center">For Individuals and Businesses</h1>
        <p style="color: #292A29" class="text-center">Join 200+ businesses using Eazipay's easy solution.</p>

        <div class="flex cards gap-6 relative" style="padding-left: 192px;">
           
            <div class="card card-1 herocard start lg:relative lg:left-0">
                <h3 class="">Tamper-proof Payroll for Life</h3>
                <p class="">
                    Your staff payroll history is kept in one place forever.
                </p>
                <p class="">
                    No more excel sheet or manual records.                            
                </p>
                <p class="">
                    Download your payroll history anytime you need it.                            
                </p>
            </div>
            <div class="card card-2 herocard lg:absolute lg:left-[30%] py-5 lg:py-0 mid">
                <h3 class="">All Payroll, Anytime Anywhere</h3>
                <p class="">
                    Wherever you are Eazipay has got you covered on ALL your Payroll tasks.                            
                </p>
                <p class="">
                    Whether it is Taxes, Pension insurances HMOs, trustfunds, Eazipay handle all your compliamces in one place and easily, in seconds!                            
                </p>
            </div>
            <div class="card card-3 herocard relative right-0 cards third">
                <h3 class="">Payroll in Seconds</h3>
                <p class="">
                    Never again will you spend more than 2 minutes on payroll.
                </p>
                <p class="">
                    Just click on your staff and bulk-pay them at once.                          
                </p>
                <p class="">
                    Payment is done permanently.                           
                </p>
            </div>
            
        </div>
        <p class="text-center" style="color: #515251; margin: 64px auto 0; width: 621.74px;">We are happy to answer your queries. Please, reach us at <a class="email-link" href="mailto:hello@myeazipay.com">hello@myeazipay.com</a> and expect our response shortly after.</p>
    </div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';

    export default defineComponent({
        name: 'Hero',
        components: {
            
        }
    });
</script>

<style scoped>
    .hero {
        padding-top: 131.75px;
        padding-bottom: 87px;
        background-image: url(/hero-desktop.png);
        background-repeat: no-repeat;
        background-size: cover;
        z-index: 2;
        margin-top: -5%;
    }
    .hero h1 {
        color: #11453B;
        font-family: MADE Mellow PERSONAL USE;
        font-size: 64px;
        font-weight: 500;
        line-height: 64px; /* 100% */
        margin-bottom: 16px;
    }
    .hero p {
        font-size: 20px;
        font-weight: 400;
        line-height: 24px; /* 120% */
        letter-spacing: 0.2px;
        margin-bottom: 64px;
    }
    .herocard {
        color: #FFF;
        display: flex;
        width: 552px;
        height: 320px;
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: flex-start;
        gap: 10px;
        flex-shrink: 0;
        padding: 64px;
        border-radius: 16px;
        transition: 4s, 2s ease-in-out;
        background: radial-gradient(50% 50.00% at 50% 50.00%, rgba(217, 235, 205, 0.14) 0%, rgba(217, 235, 205, 0.03) 100%), #11453B;
        box-shadow: -11px 0px 19px 0px rgba(23, 23, 23, 0.30), 0px 13px 20px 0px rgba(23, 23, 23, 0.20);
    }
    .herocard h3 {
        color:  #FFF;
        font-size: 28px;
        font-weight: 700;
        line-height: 36px; /* 128.571% */
    }
    .herocard p {
        color: #FFF;
        font-size: 18px;
        font-weight: 400;
        line-height: 24px; /* 133.333% */
        margin: 16px 0 0;
    }
    .email-link {
       color: #EA4E4B;
    }
    .start {
        padding-right: 20px;
      }
      .start:hover~.mid {
        left: 46%
      }
      .mid:hover {
        left: 18%
      }
      .third:hover {
        left: -2%
      }
</style>
  