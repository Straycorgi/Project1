<template>
    <div class="contacUs__bg">
        <div class="container">
            <div class="contactUs__parent">
                <div class="contactUs__text">
                    <h2 class="contactUs__title">{{ titile }}</h2>
                    <span class="contactUs__subtitle">{{ subtitle }}</span>
                </div>

                <a class="button">
                    <svg width="18" height="15" viewBox="0 0 18 15" fill="none" xmlns="http://www.w3.org/2000/svg" >
                        <path
                            d="M18 4.70312C17.6987 5.0346 17.3571 5.32589 16.9955 5.57701C15.3181 6.71205 13.6306 7.85714 11.9933 9.04241C11.1496 9.66518 10.1049 10.4286 9.01005 10.4286H9H8.98996C7.89509 10.4286 6.85045 9.66518 6.0067 9.04241C4.36942 7.8471 2.68192 6.71205 1.01451 5.57701C0.642857 5.32589 0.301339 5.0346 0 4.70312V12.6786C0 13.5625 0.723214 14.2857 1.60714 14.2857H16.3929C17.2768 14.2857 18 13.5625 18 12.6786V4.70312ZM18 1.75C18 0.866071 17.2667 0.142857 16.3929 0.142857H1.60714C0.532366 0.142857 0 0.986607 0 1.97098C0 2.88504 1.01451 4.02009 1.72768 4.50223C3.2846 5.58705 4.86161 6.67187 6.41853 7.76674C7.07143 8.21875 8.17634 9.14286 8.98996 9.14286H9H9.01005C9.82366 9.14286 10.9286 8.21875 11.5815 7.76674C13.1384 6.67187 14.7154 5.58705 16.2824 4.50223C17.1663 3.88951 18 2.875 18 1.75Z"
                            fill="black" class="mailSvg" />
                    </svg>
                    {{ btnText }}
                </a>

            </div>
        </div>
    </div>
</template>
<script>

export default {
    props: ['titile', 'subtitle', 'btnText'],
    data() {
        return {

        }
    }
}

</script>
<style> .contacUs__bg {
     background-color: #F7654A;
 }

 .contactUs__parent {
     display: flex;
     justify-content: space-between;
     align-items: center;
     padding: 35px 0px;
     flex-wrap: wrap;
 }

 .contactUs__text {
     color: #fff;
 }

 .contactUs__title {
     font-weight: 700;
     font-size: 48px;
     line-height: 148%;
     letter-spacing: 0.02em;
     text-transform: uppercase;
 }

 .contactUs__subtitle {
     font-weight: 700;
     text-transform: uppercase;
     font-size: 24px;
     line-height: 150%;
     letter-spacing: 0.02em;
 }

 .button {
     background-color: #fff;
     padding: 14px 30px;
     border: none;
     font-weight: 500;
     font-size: 14px;
     line-height: 150%;
     letter-spacing: 0.05em;
     font-family: inherit;
     color: #000000;
     position: relative;
     transition: all .3s;
     cursor: pointer;

 }
svg{
    margin-right: 15px;
}
 .button:hover {
     background-color: black;
     color: #fff;
     
 }
 .button:hover  .mailSvg{
    fill: #fff;
 }


 @media(max-width:767.99px) {
     .contactUs__title {
         font-size: 40px;
     }

     .contactUs__subtitle {
         font-size: 18px;
     }
 }

 @media(max-width:659.99px) {
     .contactUs__title {
         font-size: 32px;
     }

     .contactUs__subtitle {
         font-size: 16px;
     }
 }

 @media(max-width:564.99px) {
     .contactUs__parent {
         justify-content: center;
     }

     .contactUs__title {
         margin-bottom: 10px;
     }

     .contactUs__text {
         margin-bottom: 10px;
     }

 }

 @media(max-width:389.99px) {
     .contactUs__title {
         font-size: 26px;
     }

     .contactUs__subtitle {
         font-size: 14px;
     }
 }

 @media(max-width:339.99px) {
     .contactUs__title {
         font-size: 20px;
     }

     .contactUs__subtitle {
         font-size: 12px;
     }
 }</style>
