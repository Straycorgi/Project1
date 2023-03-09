<template>
    <div class="root">
        <div class="PartnersBlock__parent container">
            <h2 class="PartnersBlock__title">наши партнеры</h2>
            <div class="PartnersBlock__partners">
                <ul class="PartnersBlock__list">
                    <li class="PartnersBlock__item">
                        <img src="../assets/partners.png" alt="partnerts" class="PartnersBlock__img">
                    </li>
                    <li class="PartnersBlock__item">
                        <img src="../assets/partners.png" alt="partnerts" class="PartnersBlock__img">
                    </li>
                    <li class="PartnersBlock__item">
                        <img src="../assets/partners.png" alt="partnerts" class="PartnersBlock__img">
                    </li>
                    <li class="PartnersBlock__item">
                        <img src="../assets/partners.png" alt="partnerts" class="PartnersBlock__img">
                    </li>
                    <li class="PartnersBlock__item">
                        <img src="../assets/partners.png" alt="partnerts" class="PartnersBlock__img">
                    </li>
                </ul>
            </div>
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
<style>
.PartnersBlock__parent {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.PartnersBlock__title {
    font-weight: 500;
    margin-top: 100px;
    font-size: 36px;
    line-height: 147%;
    text-transform: uppercase;
    color: #FFFFFF;
    margin-bottom: 60px;
}

.PartnersBlock__list {
    display: flex;
    justify-content: center;
    gap: 64px;
    flex-wrap: wrap;
    margin-bottom: 100px;
}
@media (max-width:767.99px){
    .PartnersBlock__title{
        font-size: 28px;
    }
}
</style>
