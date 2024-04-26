<template>
  <div class="main-page-wrapper">
  <div class="card">
    <div class="card-main-info">
      <div class="card-main-info-content">
        <h1 class="main-title">zeuzvisuals is a <br>
        design agency created by</h1>

        <div class="card-agency-owner">
          <img src="/src/assets/laurentino.png" alt="Imagem de perfil">
          <h2>Laurentino Rodrigues.</h2>
        </div>
      </div>
    </div>

    <div class="card-other-infos">
      <p>From bright-eyed startups to industry giants, zeuzvisuals ignites brands with captivating designs, strategic websites, and buzz-worthy marketing.</p>
      <div class="card-other-wrapper">
        <button class="navl">
          <!-- <span>Book a call</span> -->
          <!-- <svg width="20" height="21" viewBox="0 0 20 21" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M5.75 2.5C6.16421 2.5 6.5 2.83579 6.5 3.25V4.5H13.5V3.25C13.5 2.83579 13.8358 2.5 14.25 2.5C14.6642 2.5 15 2.83579 15 3.25V4.5H15.25C16.7688 4.5 18 5.73122 18 7.25V15.75C18 17.2688 16.7688 18.5 15.25 18.5H4.75C3.23122 18.5 2 17.2688 2 15.75V7.25C2 5.73122 3.23122 4.5 4.75 4.5H5V3.25C5 2.83579 5.33579 2.5 5.75 2.5ZM4.75 8C4.05964 8 3.5 8.55964 3.5 9.25V15.75C3.5 16.4404 4.05964 17 4.75 17H15.25C15.9404 17 16.5 16.4404 16.5 15.75V9.25C16.5 8.55964 15.9404 8 15.25 8H4.75Z" fill="white"/>
          </svg> -->
          <span >Not avaliable</span>
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="white" class="w-6 h-6">
          <path  stroke-linecap="round" stroke-linejoin="round" d="m9.75 9.75 4.5 4.5m0-4.5-4.5 4.5M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
          </svg>

        </button>
        <div class="sender">
            <a class="sender-link" href="#past-projects">See work!</a>
          <svg width="20" height="21" viewBox="0 0 20 21" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M10 2.5C10.4142 2.5 10.75 2.83579 10.75 3.25V15.8401L12.7004 13.7397C12.9823 13.4361 13.4568 13.4186 13.7603 13.7004C14.0639 13.9823 14.0814 14.4568 13.7996 14.7603L10.5496 18.2603C10.4077 18.4132 10.2086 18.5 10 18.5C9.79145 18.5 9.59231 18.4132 9.4504 18.2603L6.2004 14.7603C5.91855 14.4568 5.93613 13.9823 6.23966 13.7004C6.54319 13.4186 7.01774 13.4361 7.29959 13.7397L9.25 15.8401V3.25C9.25 2.83579 9.58579 2.5 10 2.5Z" fill="white"/>
          </svg>

        </div>
      </div>
    </div>
  </div>

</div>
</template>

<style scoped>

.gradients{
  position: absolute;
  left: 0;
}

.main-page-wrapper{
  position: relative;
  height: 100%;
  width: 100%;
}



svg{
  width: 20px;
}

  a{
    text-wrap: nowrap;
  }

  .navl{
    text-wrap: nowrap;
    opacity: 0.5;
  }

  .card{
    width: 100%;
    max-width: 620px;
    padding-inline: 20px;
  }


  h1{
    font-size: 38px;
    font-weight: 600;

    line-height: 48px;
    letter-spacing: -5%;
  }

  .card-main-info{

    background: linear-gradient(to bottom right, hsla(0, 0%, 100%, 1), hsla(0, 0%, 100%, 1), hsla(0, 0%, 85%, 1));


    border-radius: 10px 10px 0 0;
  }

  .card-main-info-content{
    padding: 32px 50px 32px 40px;
  }

  .card-agency-owner{
    display: flex;
    align-items: center;
       
    border-radius: 88px;
    gap: 12px;
    padding: 5px 20px;
    margin-top: 15px;
    width: fit-content;


    background: linear-gradient(90deg, 
        hsla(226, 55%, 21%, 1),
        hsla(257, 43%, 66%, 1),
        hsla(313, 18%, 59%, 1),
        hsla(351, 66%, 64%, 1),
        hsla(33, 46%, 77%, 1)
    );


  }



  .card-main-info-titles{
    width: fit-content
  }

  .card-other-infos{
    background: linear-gradient(90deg,
    hsla(226, 57%, 21%, 1),
    hsla(218, 33%, 18%, 1)
    );


    color: #fff;

    padding: 33px 40px;

    border-radius: 0 0 10px 10px;
  }

  .card-other-wrapper{
    display: flex;
    gap: 20px;
    font-size: 600;
  }

  .sender{
    display: flex;
    align-items: center;
    cursor: pointer;
  }

  button span{
    color: white;
  }

  button{
    padding: 17.5px 35px ;
    border-radius: 65px;
    font-size: 18px;
    border: 1px solid white;
    background: hsla(0, 0%, 100%, 0.1);

    cursor: pointer;
    gap: 5px;
    display: flex;
    align-items: center;
    font-weight: 600;
  }
  p{
    margin-bottom: 15px;
    font-size: 18px;
    font-weight: 400;
  }

  .sender-link{
    font-weight: 600;
    text-decoration: none;
    color: white;
  }

  @media (max-width: 1200px){
    p, a, button{
    font-size: 85%;
  }

  h1{
    font-size: 28px;
    line-height: 32px;
  }

  .card-other-infos{

    padding: 28px 35px;

  }

  .card-main-info-content{
    padding: 28px 46px 28px 36px;
  }
}

</style>