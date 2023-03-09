<template>
    <div class="container">
        <div class="section__parent">
            <div class="section__parent-item" v-for="(info, index) in aboutInfo " :key="index">
                <AboutItem :title="info.title" :subtitle="info.subtitle" :description="info.description" />
            </div>
        </div>
    </div>
</template>
<script>
import AboutItem from './AboutItem.vue';
export default {
    components: {
        AboutItem,
    },
    data() {
        return {
            aboutInfo: [
                {
                    title: '26',
                    subtitle: 'лет',
                    description: 'на рынке'
                },
                {
                    title: '100',
                    subtitle: 'тысяч',
                    description: 'довольных клиентов'
                },
                {
                    title: '100',
                    subtitle: 'процентная',
                    description: 'гарантия'
                },
                {
                    title: '80+',
                    subtitle: 'филиалов',
                    description: 'в разных городах'
                }
            ]
        }
    }
}

</script>
<style> .section__parent {
     background-color: #F7F7F7;
     padding: 57px 130px;
     display: flex;
     flex-wrap: wrap;
     justify-content: center;
     gap: 30px;
 }

 @media (max-width:780px) {
     .section__parent-item {
         flex: 0 1 25%;
     }
 }
</style>
