<template>
    <div class="container">
        <div class="ReviewBlock__parent">
            <h2 class="ReviewBlock__title">отзывы о работе с нами</h2>

            <ul class="ReviewBlock__items">
                <li class="ReviewBlock__item">
                    <div class="ReviewBlock__content">
                        <img src="../assets/comma.svg" alt="" class="ReviewBlock__img">
                        <p class="ReviewBlock__text">Lorem Ipsum - это текст-"рыба", часто используемый в печати и
                            вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI
                            века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.
                        </p>
                    </div>
                    <div class="ReviewBlock__owner">
                        <span>Иванов Иван,</span>
                        <span> ООО “Газпром-Арена”</span>
                    </div>
                </li>
                <li class="ReviewBlock__item">
                    <div class="ReviewBlock__content">
                        <img src="../assets/comma.svg" alt="" class="ReviewBlock__img">
                        <p class="ReviewBlock__text">Lorem Ipsum - это текст-"рыба", часто используемый в печати и
                            вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI
                            века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.
                        </p>
                    </div>
                    <div class="ReviewBlock__owner">
                        <span>Иванов Иван,</span>
                        <span> ООО “Газпром-Арена”</span>
                    </div>
                </li>
                <li class="ReviewBlock__item">
                    <div class="ReviewBlock__content">
                        <img src="../assets/comma.svg" alt="" class="ReviewBlock__img">
                        <p class="ReviewBlock__text">Lorem Ipsum - это текст-"рыба", часто используемый в печати и
                            вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI
                            века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.
                        </p>
                    </div>
                    <div class="ReviewBlock__owner">
                        <span>Иванов Иван,</span>
                        <span> ООО “Газпром-Арена”</span>
                    </div>
                </li>
            </ul>

        </div>
    </div>
</template>
 
<script>

export default {

    data() {

        return {

        }

    }
}

</script>
<style scoped>
.ReviewBlock__parent {
    display: flex;
    align-items: center;
    flex-direction: column;
}

.ReviewBlock__title {
    font-weight: 500;
    font-size: 36px;
    line-height: 147%;
    text-transform: uppercase;
    color: #000000;
    margin-bottom: 60px;
}

.ReviewBlock__items {
    display: flex;
    gap: 30px;
    flex-wrap: wrap;
    justify-content: center;
}

.ReviewBlock__item {
    max-width: 350px;
}

.ReviewBlock__content {
    background: #F7F7F7;
    padding: 30px 30px 38px 30px;
    margin-bottom: 30px;
}

.ReviewBlock__img {
    margin-bottom: 20px;
}

.ReviewBlock__text {
    font-size: 14px;
    line-height: 150%;
    color: #999999;
    max-width: 270px;
}

span {
    font-weight: 500;
    font-size: 21px;
    line-height: 147%;
    letter-spacing: 0.02em;
}

span:nth-child(even) {
    color: #F7654A;

}
@media (max-width:767.99px){
    .ReviewBlock__title{
        font-size: 32px;
    }
}
@media (max-width:424.99px){
    .ReviewBlock__title{
        font-size: 26px;
    }
    .ReviewBlock__owner>span{
        font-size: 18px;
    }
}
@media (max-width:319.99px){
    .ReviewBlock__title{
        font-size: 20px;
    }
    .ReviewBlock__owner>span{
        font-size: 16px;
    }
}
</style>
