<template>
    <div class="aboutItem">
        <h2 class="aboutItem__title">
            {{ title }}
        </h2>
        <span class="aboutItem__subtitle">
            {{ subtitle }}
        </span>
        <p class="aboutItem__desc">
            {{ description }}
        </p>
    </div>
</template>
<script>

export default {

    props: ['title', 'subtitle', 'description'],
    data() {
        return {

        }
    }
}

</script>
<style> 
.aboutItem {
    text-align: center;

   
}

 .aboutItem__title {
     font-weight: 500;
     text-transform: uppercase;
     color: #F7654A;
     font-size: 72px;
     line-height: 148%;
     margin-bottom: 25px;
 }

 .aboutItem__subtitle {
     line-height: 147%;
     font-size: 36px;
     text-transform: uppercase;
     color: #000000;
     margin-bottom: 10px;
 }

 .aboutItem__desc {
     font-weight: 500;
     font-size: 18px;
     line-height: 150%;
     color: #999999;
 }
 @media (max-width:954.99px){
    .aboutItem__title{
        font-size: 55px;
    }   
    .aboutItem__subtitle{
        font-size: 22px;
    }
    .aboutItem__desc{
        font-size: 16px;
    }
}
@media (max-width:800px){
    .aboutItem__title{
        font-size: 48px;
    }   
    .aboutItem__subtitle{
        font-size: 18px;
    }
    .aboutItem__desc{
        font-size: 16px;
    }
}

</style>
