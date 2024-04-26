<script setup>
  import MainCard from './components/MainCard.vue';
  import Footer from './components/Footer.vue';
  import CardCarousel from './components/CardCarousel/CardCarousel.vue';
  import CardSlider from './components/CardSlider.vue';
  import Testimonials from './components/Testimonials/Testimonials.vue';
  import Note from './components/Note.vue';

</script>

<template>
  <div class="hero">
    <div class="initial-page" id="homepage">
      <MainCard class="mc"/>
      <div class="gradient"></div>
    </div>
    <div class="content-page">
      <CardCarousel/>
      <CardSlider/>
      <Testimonials/>
      <Note/>
      <div class="footer">
        <Footer/>
      </div>
     
    </div>
   
  </div>
</template>

<style scoped>
.hero {
  overflow: hidden;
  display: flex;
  flex-direction: column;
}

.initial-page {
  position: relative; 
  display: grid;
  place-content: center;
  min-height: 100vh;
  background-image: url('/src/assets/Preview.png');
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}

.gradient {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 35vh;
  background: linear-gradient(to bottom, rgba(6, 6, 6, 0), rgba(6, 6, 6, 1));
}

.content-page {

  z-index: 999;
  position: relative;
  background-color: rgba(6, 6, 6, 1);
  background-image: url('/src/assets/Mask-bg.png');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;

}

@media (max-width: 768px) {
  .content-page{
    background-image: url('/src/assets/mobile-bg.png');
  }
}

.mc {
  z-index: 3;
  position: relative;
}

.footer {
  position: relative;
  margin-top: 100px;
}

html {
  scroll-behavior: smooth;
}
</style>
