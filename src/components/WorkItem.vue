<template>
    <div class="WorkItem__parent">
        <img :src="require('../assets/'+img)" class="WorkItem__img" />
        <h3 class="WorkItem__title">{{ title }}</h3>
    </div>
</template>
 
<script>

export default {
    props: ['title', 'img'],
    data() {

        return {

        }

    }
}

</script>
<style>
.WorkItem__parent {
    background: #F7F7F7;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-width: 350px;
    height: 250px;
}

.WorkItem__img {
    margin-bottom: 30px;
}

.WorkItem__title {
    font-weight: 500;
    font-size: 21px;
    line-height: 147%;
    letter-spacing: 0.02em;
    color: #000000;
    text-align: center;
    max-width: 175px;
}
</style>
