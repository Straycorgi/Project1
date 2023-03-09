<template>
    <div class="item__parent">
        <img :src="require('../assets/'+imgUrl)" class="item__img">
        <h3 class="item__title">{{ title }}</h3>
        <p class="item__text">{{ description }}</p>
    </div>
</template>
<script>

export default {
    props: ['title', 'description', 'imgUrl'],
    data() {
        return {

        }
    }

}

</script>
<style> 
 .item__img {
     margin-bottom: 66px;
     max-width: 100%;
 }

 .item__title {
     font-weight: 500;
     font-size: 24px;
     line-height: 147%;
     color: #404149;
     margin-bottom: 20px;
     position: relative;
 }
 .item__title::before{
    content: ' ';
    position: absolute;
    width: 53px;
    height: 6px;
    top: -15px;
    background-color: #F7654A;
    display: inline;
 }

 .item__text {
     font-size: 16px;
     line-height: 137%;
     color: #999999;
     max-width: 350px;
 }
 @media (max-width:369.99px){
    .item__title{
        font-size: 20px;
    }
    .item__text{
        font-size: 14px;
    }
 }
</style>
