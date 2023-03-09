<template>
    <div class="container">
        <div class="questions__parent">
            <h2 class="questions__title">
                ОТВЕТЫ НА ВОПРОСЫ
            </h2>
            <ul class="questions__list" v-for="(item,index) in info" :key="index">
                <QuestionItem :title="item.title" :answer="item.answer"/>
            </ul>
        </div>
    </div>
</template>
 
<script>
import QuestionItem from './QuestionItem.vue';
export default {
    components:{
        QuestionItem,
    },
    data() {

        return {
            info: [
                {
                    title: 'РАБОТАЕТЕ ЛИ ВЫ ПО 249 ФЗ?',
                    answer: 'Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов. ',
                },
                {
                    title: 'РАБОТАЕТЕ ЛИ ВЫ ПО 249 ФЗ?',
                    answer: 'Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов. ',
                }, 
                {
                    title: 'РАБОТАЕТЕ ЛИ ВЫ ПО 249 ФЗ?',
                    answer: 'Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов. ',
                }, 
                {
                    title: 'РАБОТАЕТЕ ЛИ ВЫ ПО 249 ФЗ?',
                    answer: 'Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов. ',
                },
            ],
        }

    }
}

</script>
<style>
.questions__parent {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.questions__title {
    margin-bottom: 50px;
}

.questions__list {
    display: flex;
    flex-direction: column;
    align-self: start;
}




</style>
