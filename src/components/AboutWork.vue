<template>
    <div class="container">
        <div class="work__parent">
            <h2 class="work__title">
                ЧЕМ МЫ ЗАНИМАЕМСЯ?
            </h2>
            <div class="work__items">
                <div class="work__item" v-for="(item, index) in info" :key="index">
                    <WorkItem :title="item.title" :img="item.img"></WorkItem>
                </div>
            </div>
        </div>
    </div>
</template>
 
<script>
import WorkItem from './WorkItem.vue';
export default {
    components: {
        WorkItem,
    },
    data() {

        return {
            info: [
                {
                    title: 'СТРОИТЕЛЬСТВО ОФИСНЫХ ЗДАНИЙ',
                    img: 'house.svg',
                },
                {
                    title: 'СТРОИТЕЛЬСТВО СТАДИОНОВ',
                    img: 'house.svg',
                },
                {
                    title: 'СТРОИТЕЛЬСТВО ДОМОВ',
                    img: 'house.svg',
                },
                {
                    title: 'СТРОИТЕЛЬСТВО МОСТОВ',
                    img: 'house.svg',
                },
                {
                    title: 'СТРОИТЕЛЬСТВО ЗАВОДОВ',
                    img: 'house.svg',
                },
                {
                    title: 'СТРОИТЕЛЬСТВО СОЦИАЛЬНЫХ ЗДАНИЙ',
                    img: 'house.svg',
                },

            ],
        }

    }
}

</script>
<style>
.work__parent {
    display: flex;
    align-items: center;
    flex-direction: column;
}

.work__title {
    font-weight: 500;
    font-size: 36px;
    line-height: 147%;
    text-transform: uppercase;
    color: #000000;
    margin-bottom: 66px;
}

.work__items {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 30px;
}

.work__item {
   transition: all .3s;
}
.work__item:hover{
    transform: scale(1.1);
}
@media (max-width:425px){
    .work__title{
        font-size: 28px;
    }
}
</style>
