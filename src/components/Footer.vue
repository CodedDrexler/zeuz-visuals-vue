<template>
  <div class="footer">
    <div class="full-wrapper">
    <div class="footer-content">
      <div class="left">
        <div class="title-wrapper">
          <svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M15.5784 2.47938C15.671 2.04704 15.4611 1.60647 15.067 1.40603C14.6729 1.20559 14.1932 1.29545 13.8984 1.62497L2.84838 13.975C2.59199 14.2615 2.52796 14.672 2.68491 15.0231C2.84186 15.3741 3.19047 15.6001 3.57499 15.6001H12.1189L10.4216 23.5208C10.329 23.9531 10.5389 24.3937 10.933 24.5942C11.3271 24.7946 11.8068 24.7047 12.1016 24.3752L23.1516 12.0252C23.408 11.7387 23.472 11.3282 23.3151 10.9771C23.1581 10.6261 22.8095 10.4001 22.425 10.4001H13.8811L15.5784 2.47938Z" fill="url(#paint0_linear_5_25)"/>
<path d="M15.5784 2.47938C15.671 2.04704 15.4611 1.60647 15.067 1.40603C14.6729 1.20559 14.1932 1.29545 13.8984 1.62497L2.84838 13.975C2.59199 14.2615 2.52796 14.672 2.68491 15.0231C2.84186 15.3741 3.19047 15.6001 3.57499 15.6001H12.1189L10.4216 23.5208C10.329 23.9531 10.5389 24.3937 10.933 24.5942C11.3271 24.7946 11.8068 24.7047 12.1016 24.3752L23.1516 12.0252C23.408 11.7387 23.472 11.3282 23.3151 10.9771C23.1581 10.6261 22.8095 10.4001 22.425 10.4001H13.8811L15.5784 2.47938Z" fill="url(#paint1_linear_5_25)"/>
<defs>
<linearGradient id="paint0_linear_5_25" x1="13" y1="1.30005" x2="13" y2="24.7001" gradientUnits="userSpaceOnUse">
<stop stop-color="#D9D9D9"/>
<stop offset="1" stop-color="#737373"/>
</linearGradient>
<linearGradient id="paint1_linear_5_25" x1="5.5" y1="26" x2="20" y2="8.5" gradientUnits="userSpaceOnUse">
<stop stop-color="#182653"/>
<stop offset="0.33" stop-color="#9883CE"/>
<stop offset="0.59" stop-color="#A983A1"/>
<stop offset="0.761122" stop-color="#DF6578"/>
<stop offset="1" stop-color="#DFC6A8"/>
</linearGradient>
</defs>
          </svg>
          <h1>zeuzvisuals</h1>
        </div>
        <p>Zeuz Visuals 2024, by Laurentino Rodrigues</p>
      </div>

      <div class="right">
        <a href="">Work with us</a>
        <a href="">Behance</a>
        <a href="#homepage">Go to top</a>
      </div>
    </div>
    <img class="bg" src="../assets/dot-bg.png" alt="">
  </div>
  
  </div>
</template>

<style scoped>
*{
  color: white;
}

.full-wrapper{
  position: relative;
}

.bg{
  position: absolute;
  bottom: 0;
  right: 0;
  z-index: -1;
}

.footer {
    position: absolute;

    bottom: 0;
    left: 0;
    right: 0;
    margin-left: auto; 
    margin-right: auto; 
    width: 100%;
    max-width: 1258px;
    background: linear-gradient(90deg,
        hsla(226, 57%, 21%, 1),
        hsla(218, 33%, 18%, 1)
    );

    border-radius: 10px 10px 0 0;


}

.footer-content{
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 41px 61px 95px;
}

.title-wrapper{
  display: flex;
  align-items: center;
  gap: 5px;
}

.left{
  display: flex;
  flex-direction: column;
  gap: 7px;
}

p{
  color: rgba(255, 255, 255, 0.4);
}
a{
  text-decoration: none;
  font-weight: 700px;
}

.right{
  display: flex;
  gap: 40px;
  font-weight: 600;


}

@media (max-width: 768px){
  *{
    font-size: 95%;
  }

  .footer-content{

  padding: 35px 30px 60px;

}



  p{
    max-width: 70%
  }

  .right{
    flex-direction: column;
    font-size: 16px;
    gap: 15px;
    text-wrap: nowrap;
  }

}

</style>