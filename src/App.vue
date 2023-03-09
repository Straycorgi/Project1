<template>
  <div class="wrapper" >
    <headerBlock id="Header" />
    <main class="main">
      <AboutSection class="about" />
      <AboutProjects class="projects" id="Projects" />
      <contactUs class="contactUs" :titile="this.contactUstext[0].title" :subtitle="this.contactUstext[0].subtitle"
        :btn-text="this.contactUstext[0].btnText" />
      <AboutWork class="aboutWork" id="Works"/>
      <div class="visual" />
      <QuestionsBlock class="QuestionsBlock" id="FAQ" />
      <PartnersBlock class="PartnersBlock" id="Partners" />
      <ReviewBlock class="ReviewBlock" id="Review" />
      <contactUs class="contactUs" :titile="this.contactUstext[1].title" :subtitle="this.contactUstext[1].subtitle"
        :btn-text="this.contactUstext[1].btnText" />
      <contactInfo class="contactInfo" id="Contact"/>
    </main>
    <footer class="footer">
      <div class="container">
        <div class="footer__parent">
          <p class="footer__text">
            © 2019 Строительная компания
          </p>
          <p class="footer__text">
            Разработано лучшей студей
          </p>
        </div>
      </div>
    </footer>
    
  </div>
</template>

<script>
import headerBlock from './components/headerBlock.vue'
import AboutSection from './components/AboutSection.vue';
import AboutProjects from './components/AboutProjects.vue';
import contactUs from './components/contactUs.vue';
import AboutWork from './components/AboutWork.vue';
import QuestionsBlock from './components/QuestionsBlock.vue';
import PartnersBlock from './components/PartnersBlock.vue';
import ReviewBlock from './components/ReviewBlock.vue';
import contactInfo from './components/contactInfo.vue';

export default {
  name: 'App',
  components: {
    headerBlock, AboutSection, AboutProjects, contactUs, AboutWork, QuestionsBlock, PartnersBlock, ReviewBlock, contactInfo,

  },
  data() {
    return {
      contactUstext: [
        {
          title: 'САМЫЕ УМНЫЕ ПРОЕКТЫ',
          subtitle: 'РЕАЛИЗУЕМ САМЫЕ СМЕЛЫЕ РЕШЕНИЯ В РОССИИ!',
          btnText: 'ВАШ ЗАПРОС',
        },
        {
          title: 'ХОТИТЕ С НАМИ РАБОТАТЬ?',
          subtitle: 'ОСТАВЬТЕ ЗАЯВКУ И МЫ СВЯЖЕМСЯ С ВАМИ!',
          btnText: 'ВАШ ЗАПРОС',
        },
      ],
    
      
    }
  }
}
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Oswald:regular,500,700);

*,
*::before,
*::after {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
  font-family: 'Oswald';
  
}
html{
  scroll-behavior: smooth;
}
.wrapper {
  overflow: hidden;
}

.main {
  margin-top: -150px;

}

.container {
  max-width: 1140px;
  padding: 0 15px;
  margin: 0 auto;
  font-size: 16px;

}

.about {
  margin-bottom: 100px;
}

.projects {
  margin-bottom: 150px;
}

.contactUs {
  margin-bottom: 150px;
}

.aboutWork {
  margin-bottom: 150px;
}

.visual {
  margin-bottom: 150px;
  background-image: url('assets/visual.jpg');
  background-position: center;
  height: 814px;
  width: 100vw;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
}

.QuestionsBlock {
  margin-bottom: 150px;
}

.PartnersBlock {
  margin-bottom: 150px;
  background-color: #404149;
  width: 100vw;
}

.ReviewBlock {
  margin-bottom: 150px;
}

.contactInfo {
  margin-bottom: 150px;
}

.footer {
  width: 100vw;
  background-color: #404149;
}

.footer__parent {
  display: flex;
  justify-content: space-between;
  padding: 30px 0;
}

.footer__text {
  font-size: 16px;
  line-height: 137%;
  color: #FFFFFF;
}

@media(max-width:767.99px){
  .footer__text{
    font-size: 14px;
  }
}
@media(max-width:319.99px){
  .footer__text{
    font-size: 12px;
  }
}


</style>
