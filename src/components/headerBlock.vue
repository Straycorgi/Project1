<template>
    <div class="header">
        <div class="container">        
            <transition name="fade">
            <nav class="header__menu" v-if="isBurger">
                <ul class="header__menu-list">
                    <li class="header__menu-item">
                        <a href="#Projects" class="header__menu-link">Наши проекты </a>
                    </li>
                    <li class="header__menu-item">
                        <a href="#Works" class="header__menu-link">Чем занимаемся</a>
                    </li>
                    <li class="header__menu-item">
                        <a href="#FAQ" class="header__menu-link">FAQ</a>
                    </li>
                    <li class="header__menu-item">
                        <a href="#Partners" class="header__menu-link">Партнеры</a>
                    </li>
                    <li class="header__menu-item">
                        <a href="#Review" class="header__menu-link">Отзывы</a>
                    </li>
                    <li class="header__menu-item">
                        <a href="#Contact" class="header__menu-link">Контакты</a>
                    </li>
                </ul>
            </nav>
        </transition>
            <div class="header__top">
                <a href="" class="header__link">
                    <img src="../assets/logo.svg" alt="icon" class="header__link-icon">
                </a>
                <button class="burger" @click="isBurger = !isBurger">
                    <span class="burger__line" :class="{ line1: isBurger }" />
                    <span class="burger__line" :class="{ line2: isBurger }" />
                    <span class="burger__line" :class="{ line3: isBurger }" />
                </button>

            </div>
            <div class="header__botttom">
                <h1 class="header__title">
                    РЕАЛИЗУЕМ КРУПНЕЙШИЕ
                    ПРОЕКТЫ В РОССИИ
                </h1>
                <span class="header__subtitle">
                    стадионы, газопроводы, мосты, дамбы
                </span>
            </div>
        </div>
    </div>
</template>

<script>

export default {


    data() {
        return {
            isBurger: false,
        }

    },
   
}

</script>
<style>
.header {
    background-image: url('../assets/background.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

.burger {
    width: 50px;
    height: 50px;
    background-color: #F7654A;
    border: none;
    cursor: pointer;
    animation: ViewBurger 0.5s;
    z-index: 50;
    padding: 11px 15px;
    position: relative;
}

.burger__line {
    display: block;
    width: 21px;
    height: 3px;
    background-color: white;
    transition: transform 0.5s;
}
.line1{
    margin-top: 0;
    transform: rotate(45deg);
}
.line2{
    opacity: 0;
}
.line3{
    margin-top: -14px;    
    transform: rotate(131deg);
}
.burger__line:not(:last-child) {
    margin-bottom: 4px;
}

.header__top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 102px;
    padding-top: 20px;
}

.header__botttom {
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.header__title {
    font-size: 64px;
    font-weight: 500;
    line-height: 148%;
    margin-bottom: 35px;
    text-align: center;
    max-width: 734px;
}

.header__subtitle {
    font-size: 18px;
    font-weight: 400;
    line-height: 150%;
    margin-bottom: 320px;
}

.header__botttom {
    animation: view 3s;
}

.header__link {
    animation: ViewIcon 0.5s;
}

.header__menu {
    position: absolute;
    width: 100%;

    left: 0;
    background-color: rgba(255, 255, 255, 0.5);
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 24px;
    color: black;
    transition: all .0.5s ease-in-out;
    animation: ShowNav 0.5s ease-in-out;
    padding: 50px 0;

}

.header__menu-list {
    display: flex;
    justify-content: space-between;
    gap: 30px;
    align-items: center;
    flex-wrap: wrap;
}



.header__menu-link {
    color: inherit;
    border-bottom: 0px;
    transition: border-bottom 3s;
}

.header__menu-link:hover {
    border-bottom: 1px solid black;

}

@keyframes view {
    from {
        opacity: 0;
    }

    to {
        opacity: 1;
    }

}

@keyframes ViewIcon {
    from {
        opacity: 0;
        margin-left: -200px;
    }

    to {
        opacity: 1;
        margin-left: 0;
    }
}

@keyframes ViewBurger {
    0% {
        opacity: 0;
        margin-right: -200px;
    }

    100% {
        opacity: 1;
        margin-right: 0;
    }
}
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}


@media (max-width:991.99px) {
    .header__menu {
        padding: 25px 0;
    }

    .header__title {
        font-size: 48px;
    }

    .header__subtitle {
        font-size: 16px;
    }

    .header__menu-link {
        font-size: 18px;

    }

    .header__menu-list {
        gap: 20px;
    }
}

@media (max-width:767.99px) {
    .header__title {
        font-size: 42px;
    }

    .header__subtitle {
        font-size: 14px;
    }

    .header__menu-link {
        font-size: 16px;

    }

    .header__menu-list {
        gap: 15px;
    }
}

@media (max-width:599.99px) {
    .header__menu-list {
        width: 250px;
        gap: 10px;
    }
}

@media (max-width:459.99px) {
    .header__menu-list {
        width: 200px;
        gap: 5px;
    }
}

@media (max-width:399.99px) {
    .header__menu-list {
        flex-direction: column;
        gap: 0;
    }

    .header__menu {
        background-color: rgba(156, 148, 148, 0.993);
        padding: 10px 0;
    }

    .header__menu-link {
        font-size: 20px;
    }
}</style>
