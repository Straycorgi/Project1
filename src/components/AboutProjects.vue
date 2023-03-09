<template>
    <div class="container">
        <div class="aboutProject__parent">
            <h2 class="about__project-title">
                НАШИ САМЫЕ БОЛЬШИЕ ПРОЕКТЫ
            </h2>
            <div class="about__project-items">
                <div class="about__project-item" v-for="(item, index) in info" :key="index">
                    <ProjectItem :title="item.title" :description="item.description" :img-Url="item.imgUrl" />
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import ProjectItem from './ProjectItem.vue';

export default {
    components: {
        ProjectItem,
    },
    data() {
        return {
            info: [
                {
                    title: 'Газпром Арена',
                    description: 'Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву.',
                    imgUrl: 'arena.jpg'
                },
                {
                    title: 'Газпром Арена',
                    description: 'Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву.',
                    imgUrl: 'arena.jpg'
                },
                {
                    title: 'Газпром Арена',
                    description: 'Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву.',
                    imgUrl: 'arena.jpg'
                }
            ]
        }
    }
}

</script>
<style> .aboutProject__parent {
     display: flex;
     flex-direction: column;
     align-items: center;
 }

 .about__project-title {
     font-weight: 500;
     font-size: 36px;
     line-height: 147%;
     text-transform: uppercase;
     color: #404149;
     margin-bottom: 60px;
 }

 .about__project-items {
    display: flex;
    gap: 30px;
    flex-wrap: wrap;
    justify-content: space-around;
 }

 
@media (max-width:767.99px){
    .about__project-title {
        font-size: 30px;
    }
}
@media (max-width:450.99px){
    .about__project-title {
        font-size: 24px;
    }
}
@media (max-width:369.99px){
    .about__project-title {
        font-size: 20px;
    }
}
</style>
