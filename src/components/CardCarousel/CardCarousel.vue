<script setup>
  import { ref, onMounted, onUnmounted } from 'vue';
  import Card from './Card.vue';

  const gap = 10; 
  const translateXValue = ref(0);
  const maxTranslateXValue = ref(0);


  const calculateMaxTranslateX = () => {
    const containerWidth = document.querySelector('.carousel-wrapper').clientWidth;
    const cardContainer = document.querySelector('.card-container');
    const cardWidth = cardContainer.children[0].offsetWidth;
    const cardContainerWidth = (cardWidth + gap) * (cardContainer.children.length);
    maxTranslateXValue.value = containerWidth - cardContainerWidth;
  };

  const handleRight = () => {
  if (translateXValue.value > maxTranslateXValue.value) {
    const cardWidth = document.querySelector('.card').offsetWidth;
    let remaining = Math.abs(maxTranslateXValue.value - translateXValue.value);
    console.log(remaining);

    if (remaining > cardWidth) { 
      translateXValue.value -= cardWidth;
    } else {
      translateXValue.value = cardContainerWidth; 
    }
  }
};
const handleLeft = () => {
  const cardWidth = document.querySelector('.card').offsetWidth; 
  if (translateXValue.value >= 0) {
    return; 
  }

  translateXValue.value += cardWidth;
};

  onMounted(() => {
    calculateMaxTranslateX();
    window.addEventListener('resize', calculateMaxTranslateX);
  });

  onUnmounted(() => {
    window.removeEventListener('resize', calculateMaxTranslateX);
  });
</script>


<template>
  <section class="card-carousel" id="past-projects">

    <h1>Explore past projects</h1>
    <div class="carousel-wrapper">
      <div class="card-container" :style="{ transform: `translateX(${translateXValue}px)` }">
        <Card
        h1Text="Intellectual Point"
        pText="Marketing & Website Design"
        backgroundColor="linear-gradient(90deg,
    rgba(45, 79, 131, 1),
    rgba(16, 37, 89, 1)
    )"
        />
        <Card
        h1Text="Wise Evolution"
        pText="Brand Design"
        backgroundColor="linear-gradient(90deg, #2D6E83 0%, #004788 100%)"
        />
        <Card
        h1Text="Neuroscale"
        pText="Product Design"
        backgroundColor="linear-gradient(90deg, #5D2D83 0%, #161059 100%)"
        />
        <Card
        h1Text="Intellectual Point"
        pText="Marketing & Website Design"
        backgroundColor="linear-gradient(90deg,
    rgba(45, 79, 131, 1),
    rgba(16, 37, 89, 1)
    )"
        />
        <Card
        h1Text="Wise Evolution"
        pText="Brand Design"
        backgroundColor="linear-gradient(90deg, #2D6E83 0%, #004788 100%)"
        />
        <Card
        h1Text="Neuroscale"
        pText="Product Design"
        backgroundColor="linear-gradient(90deg, #5D2D83 0%, #161059 100%)"
        />
        <Card
        h1Text="Intellectual Point"
        pText="Marketing & Website Design"
        backgroundColor="linear-gradient(90deg,
    rgba(45, 79, 131, 1),
    rgba(16, 37, 89, 1)
    )"
        />
        <Card
        h1Text="Wise Evolution"
        pText="Brand Design"
        backgroundColor="linear-gradient(90deg, #2D6E83 0%, #004788 100%)"
        />
        <Card
        h1Text="Neuroscale"
        pText="Product Design"
        backgroundColor="linear-gradient(90deg, #5D2D83 0%, #161059 100%)"
        />

      </div>
    </div>
    <button @click="handleRight" class="right">
      <svg width="16" height="28" viewBox="0 0 16 28" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M1.75 1.5L14.25 14L1.75 26.5" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </button>
    <button @click="handleLeft" class="left">
      <svg width="16" height="28" viewBox="0 0 16 28" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M1.75 1.5L14.25 14L1.75 26.5" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </button>
  </section>
</template>

<style scoped>
* {
  color: white;
}

.el-1{
  position: absolute;
  transform: translateY(-280px);
  z-index: 3;
}

#past-projects{
  scroll-behavior: smooth;
}

h1 {
  font-size: 28px;
  margin-bottom: 30px;
  padding-top: 100px;
  text-align: center;
}

.card-carousel {
  z-index: 3;
  position: relative;
  background-color: rgba(6, 6, 6, 1);
}

.carousel-wrapper {
  overflow: hidden;
  
  position: relative; 
  padding-inline: 90px;
}

/* .carousel-wrapper::after{
    content: '';
    position: absolute;
    height: 100%;
    width: 250px;
    right: 0;
    top: 0;
    background: linear-gradient(to left,
    rgba(6, 6, 6, 1),
    rgba(6, 6, 6, 0)
    );
  }
.carousel-wrapper::before{
    content: '';
    position: absolute;
    height: 100%;
    width: 250px;
    left: 0;
    top: 0;
    background: linear-gradient(to right,
    rgba(6, 6, 6, 1),
    rgba(6, 6, 6, 0)
    );
    z-index: 40;
  } */

.card-container {
  display: flex;
  gap: 10px;
  transition: transform 0.5s ease;
  width: fit-content
}

button {
  cursor: pointer;
  background: none;
  border: none;
  position: absolute;
  top: 418px;
}

.right {
  right: 91px;

}

.left{
  transform: rotate(180deg);
  left: 91px;
}
</style>
