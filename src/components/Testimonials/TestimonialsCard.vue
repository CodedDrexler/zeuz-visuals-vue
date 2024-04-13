<template>
  <div class="card">
    <div class="card-wrapper">
      <p class="testimonial">
        {{ testimonialText }}
      </p>

      <div class="info">
            <img :src="imageSrc" alt="Autor da descrição">
        <div class="names">
          <h2>{{ name }}</h2>
          <h3>{{ position }}</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    testimonialText: String, 
    imageSrc: String,
    name: String, 
    position: String
  }
}
</script>

<style scoped>


img{
  width: 40px;
  height: 40px;
  border-radius: 80px;
}

.card{
  padding: 30px 21px;
  border: 1px solid rgba(255, 255, 255, 0.1);
  background: linear-gradient(45deg,
  rgba(255, 255, 255, 0.4),
  rgba(255, 255, 255, 0)
  );
  max-width: fit-content;

  font-size: 16px;
  color: white;

  border-radius: 8px;
  height: fit-content;

}

h2{
  font-size: 18px;
  font-weight: 600;
}
h3{
  font-size: 16px;
  font-weight: 400;
  color: rgba(255, 255, 255, 0.7);
}

p{
  margin-bottom: 20px;
}

.info{
  display: flex;
  gap: 13px;
}

.card-wrapper{
  max-width: 342px;
}
</style>