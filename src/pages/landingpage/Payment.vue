<template>
    <div class="payment">
        <div class="flex" style="paddingLeft: 192px">
            <section class="payment-left">
                <h1>Free forever <br /> for your <span class="red">salary <br /> payment</span></h1>
                <p>Subscribe to the Eazilife today</p>
                <div  class="flex justify-between" style="width: 391px">
                    
                    <div class="downloadStore">
                        <div class="icon">
                            <svg width="24" height="25" viewBox="0 0 24 25" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <g id="ic:baseline-apple">
                                <path id="Vector" d="M17.0499 20.781C16.0699 21.731 14.9999 21.581 13.9699 21.131C12.8799 20.671 11.8799 20.651 10.7299 21.131C9.28992 21.751 8.52992 21.571 7.66992 20.781C2.78992 15.751 3.50992 8.09104 9.04992 7.81104C10.3999 7.88104 11.3399 8.55104 12.1299 8.61104C13.3099 8.37104 14.4399 7.68104 15.6999 7.77104C17.2099 7.89104 18.3499 8.49104 19.0999 9.57104C15.9799 11.441 16.7199 15.551 19.5799 16.701C19.0099 18.201 18.2699 19.691 17.0399 20.791L17.0499 20.781ZM12.0299 7.75104C11.8799 5.52104 13.6899 3.68104 15.7699 3.50104C16.0599 6.08104 13.4299 8.00104 12.0299 7.75104Z" fill="black"/>
                                </g>
                            </svg>
                        </div>
                        <div class="icon-text">
                            <p>Download on the</p>
                            <span>Appstore</span>
                        </div>
                    </div>
                    <div class="downloadStore"> 
                        <div class="icon">
                            <svg width="22" height="25" viewBox="0 0 22 25" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <g id="logos:google-play-icon" clip-path="url(#clip0_4_4165)">
                                <path id="Vector" d="M10.2837 11.9427L0.234863 22.4709C0.347711 22.8708 0.550502 23.2396 0.827735 23.5492C1.10497 23.8587 1.4493 24.1007 1.83442 24.2568C2.21953 24.4129 2.63523 24.4788 3.04973 24.4496C3.46424 24.4204 3.86657 24.2968 4.22599 24.0882L15.5329 17.6486L10.2837 11.9427Z" fill="#EA4335"/>
                                <path id="Vector_2" d="M20.4449 10.1531L15.5555 7.35248L10.0518 12.1822L15.5779 17.6335L20.4301 14.8629C20.86 14.6378 21.22 14.2993 21.4712 13.8842C21.7224 13.4691 21.8552 12.9932 21.8552 12.5079C21.8552 12.0227 21.7224 11.5468 21.4712 11.1317C21.22 10.7165 20.86 10.3781 20.4301 10.153H20.4451L20.4449 10.1531Z" fill="#FBBC04"/>
                                <path id="Vector_3" d="M0.234942 2.49286C0.174202 2.71741 0.143966 2.94912 0.145048 3.18174V21.7819C0.145677 22.0144 0.175884 22.246 0.234942 22.4709L10.6283 12.2123L0.234942 2.49286Z" fill="#4285F4"/>
                                <path id="Vector_4" d="M10.3586 12.4819L15.5553 7.35258L4.26347 0.882923C3.83862 0.634109 3.35542 0.502342 2.86308 0.501043C1.64128 0.498668 0.567132 1.30958 0.234863 2.48541L10.3586 12.4819Z" fill="#34A853"/>
                                </g>
                                <defs>
                                <clipPath id="clip0_4_4165">
                                <rect width="21.7102" height="24" fill="white" transform="translate(0.14502 0.501038)"/>
                                </clipPath>
                                </defs>
                            </svg>
                        </div>
                        <div class="icon-text">
                            <p>Get on</p>
                            <span>Google Play</span>
                        </div>
                    </div>
                    <!-- <img
                         class=""
                        src="/googleplay.png"
                        alt="googleplay"
                    /> -->
                </div>
            </section>
            <section class="payment-right">

            </section>
        </div>
    </div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';

    export default defineComponent({
        name: 'Payment',
        components: {
            
        }
    });
</script>

<style scoped>
    .payment {
        height: 795.572px;
        background-image: url(/works.png);
        background-repeat: no-repeat;
        background-size: cover;
    }
    .payment-left {
        width: 552px;
        margin-top: 190px;
    }
    .payment h1 {
        color: var(--new-styles-text-heading, #292A29);
        font-family: MADE Mellow PERSONAL USE;
        font-size: 56px;
        font-weight: 500;
        line-height: 64px; /* 114.286% */
        margin-bottom: 42px;
    }
    .payment-left p {
        color: var(--new-styles-text-heading, #292A29);
        font-size: 18px;
        font-weight: 500;
        line-height: 24px; /* 133.333% */
        margin-bottom: 16px
    }
    .red {
        color: #EA4E4B;
    }
    .downloadStore {
        width: 179px;
        display: flex;
        padding: 12px;
        align-items: center;
        gap: 12px;
        border-radius: 8px;
        background: #FFF;
        cursor: pointer;
        box-shadow: 0px 20px 48px 0px rgba(170, 170, 170, 0.29);
    }
    .icon {
        width: 48px;
        height: 48px;
        background-color: #F2F1F1;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .icon-text p {
        color: #515251;
        font-size: 12px;
        font-weight: 500;
        line-height: 16px; /* 133.333% */
        margin: 0;
    }
    .icon-text span {
        color: #515251;
        font-size: 18px;
        font-weight: 700;
        line-height: 24px; /* 133.333% */
    }
    .payment-right {
        margin-top: 140.7px;
        width: 480px;
        height: 433px;
        background-image: url(/payment.png);
        background-repeat: no-repeat;
        background-size: cover;
    }
</style>
  