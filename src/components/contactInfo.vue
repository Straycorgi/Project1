<template>
    <div class="container">
        <div class="contactInfo__parent">
            <h2 class="contactInfo__title">
                КОНТАКТЫ
            </h2>
            <ul class="contactInfo__links">
                <li class="contactInfo__link">
                    <img src="../assets/GPS.svg" alt="gps" class="contactInfo__img">
                    <h3 class="contactInfo__link-title">АДРЕС:</h3>
                    <span class="contactInfo__link-subtitle">НЕВСКИЙ ПРОСПЕКТ 140,
                        ОФИС 140-142</span>
                </li>
                <li class="contactInfo__link">
                    <img src="../assets/Phone.svg" alt="gps" class="contactInfo__img">
                    <h3 class="contactInfo__link-title">ТЕЛЕФОН:</h3>
                    <span class="contactInfo__link-subtitle">8 (812) 111-22-33
                        8 (812) 111-22-33</span>
                </li>
                <li class="contactInfo__link">
                    <img src="../assets/clock.svg" alt="gps" class="contactInfo__img">
                    <h3 class="contactInfo__link-title">ВРЕМЯ РАБОТЫ:</h3>
                    <span class="contactInfo__link-subtitle">ПН-СБ
                        10:00 - 20:00</span>
                </li>
                <li class="contactInfo__link">
                    <img src="../assets/mail.svg" alt="gps" class="contactInfo__img">
                    <h3 class="contactInfo__link-title">E-MAIL:</h3>
                    <span class="contactInfo__link-subtitle">INFO@VIP.RU</span>
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
<style>
.contactInfo__parent {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.contactInfo__title {
    font-weight: 500;
    font-size: 36px;
    line-height: 147%;
    text-transform: uppercase;
    color: #000000;
    margin-bottom: 60px;
}

.contactInfo__links {
    display: flex;
    justify-content: center;
    width: 100%;
    gap: 30px;
    flex-wrap: wrap;
}

.contactInfo__link {
    display: flex;
    flex-direction: column;
    align-items: center;
    min-width: 255px;
}

.contactInfo__img {
    margin-bottom: 36px;
}

.contactInfo__link-title {
    margin-bottom: 25px;
    font-weight: 500;
    font-size: 24px;
    line-height: 150%;
    text-align: center;
    color: #999999;
}

.contactInfo__link-subtitle {
    font-weight: 500;
    font-size: 24px;
    line-height: 150%;
    text-align: center;
    color: #000000;
    transition: all .15s;
    max-width: 255px;

}
.contactInfo__link-subtitle:hover{
    color: #F7654A;
}
@media (max-width: 767.99px){
    .contactInfo__title{
        font-size: 32px;
    }
    .contactInfo__link-title{
        font-size: 20px;
    }
    .contactInfo__link-subtitle{
        font-size: 20px;
        max-width: 200px;
    }
}

</style>
