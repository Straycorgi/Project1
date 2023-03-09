<template>
    <div class="question__item-block">
        <div class="question__item-parent" @click="isOpen = !isOpen, isRotate = !isRotate">
            <img src="../assets/arrow.svg" alt="arrow" class="questions__item-img" :class="{rotateDeg:isRotate}">
            <h3  class="questions__item-title" aria-expanded="true">{{ title
            }}</h3>
        </div>
        <p v-if="isOpen" class="questions__item-answer">{{ answer }}</p>
    </div>
</template>
 
<script>





export default {
    props: ['title', 'answer'],
    data() {

        return {
            isOpen: false,
            isRotate: false,
        }

    },


}

</script>
<style> .questions__item-title {
     font-weight: 500;
     font-size: 24px;
     line-height: 150%;
     color: #F7654A;
     margin-left: 15px;
     text-align: center;
 }

 .question__item-parent {
     display: flex;
     align-items: center;
     margin-bottom: 40px;
     cursor: pointer;
 }
 .questions__item-img{
    transition: all .3s;
 }
 .rotateDeg {
    transform: rotate(-90deg);
 }



 .questions__item-answer {
     margin-top: -10px;
     margin-bottom: 40px;
     font-size: 16px;
     line-height: 137%;
     color: #999999;
     max-width: 575px;

     animation: ShowAnswer 0.5s;
 }

 @keyframes ShowAnswer {
     from {
         opacity: 0;
     }

     to {
         opacity: 1;
     }

 }
 @media (max-width:359.99px){
    .questions__item-title{
        font-size: 18px;
    }
 }
 </style>
