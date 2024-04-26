<script>
export default {
  props: {
    h1Text: String, 
    pText: String,
    backgroundColor: String
  }
}

</script>


<template>
  <div class="card">

      <img src="../../assets/ip.png" alt="">

    <div class="card-info" :style="{ background: backgroundColor }">
      <div class="card-info-text">
        <h1>{{ h1Text }}</h1>
        <p>{{ pText }}</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .card{

    cursor: pointer;
    min-width: 420px;
    display: flex;
    flex-direction: column;
    overflow: hidden;

  }



  .card-info{
    /* background: linear-gradient(90deg,
    rgba(45, 79, 131, 1),
    rgba(16, 37, 89, 1)
    ); */
    padding: 24px 0px 24px 33px;
    border-radius: 0px 0px 10px 10px;
  }

  h1{
    color: white;
    font-size: 22px;
    font-weight: 600;
  }

  p{
    color: rgba(255, 255, 255, 0.6);
    font-weight: 400;
    font-size: 22px;
  }

  @media(max-width: 768px){
    .card{

      min-width: 297px;

    }
    p{
      font-size: 18px;
    }
  }
</style>