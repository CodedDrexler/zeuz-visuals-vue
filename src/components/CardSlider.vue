<template>
  <div class="wrapper">
    <h1>A partner to brands including</h1>

    <div class="card-marquee-wrapper">
      <div class="card-marquee">
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      </div>
      <div class="card-marquee">
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      <div class="card">
        <img src="../assets/ip-white.png" alt="">
      </div>
      </div>
    </div>
</div>
</template>

<style scoped>
  .wrapper{
    

    padding-top: 100px;

  }

  .card{

    padding: 62px 40px 61px 40px;
    background: linear-gradient(45deg,
    rgba(255, 255, 255, 0.4),
    rgba(255, 255, 255, 0)
    );
    
    border-radius: 10px;
    border: 1px solid rgba(255, 255, 255, 0.1);
  }

  h1{
    color: white;
    font-size: 28px;
    text-align: center
  }

  .card-marquee-wrapper{
    overflow: hidden;
    white-space: nowrap;
    position: relative;

    display: flex;
    gap: 30px;

  }


  .card-marquee{

    display: flex;
    gap: 30px;
    animation: 30s slider infinite linear;
    padding-top: 30px;
  }

  @keyframes slider{
    from{
      transform: translateX(0);
    }
    to{
      transform: translateX(-100%)
    }
  }

  @media (max-width: 768px) {
    .card-marquee{


  animation: 18s slider infinite linear;

}
  }
</style>