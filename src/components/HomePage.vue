<script setup>

</script>

<template>
<div>
  <div class="social">
    <a href=""> <i class="fa-brands fa-telegram"></i></a>
    <a href=""> <i class="fa-brands fa-instagram"></i> </a>
    <a href=""><i class="fa-brands fa-github"></i> </a>
  </div>

  <div class="courusel">
    <div class="video">
      <video autoplay="" preload="auto" loop="" playsinline=""><source type="video/webm" src="https://cdn.akamai.steamstatic.com/apps/csgo/videos/csgo_react/cs2/cs2_header.webm"><source type="video/mp4" src="https://cdn.akamai.steamstatic.com/apps/csgo/videos/csgo_react/cs2/cs2_header.mp4">
      </video>
    </div>
    <div id="carouselExample" class="carousel slide">
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="../assets/img/imgcourusel/104a6f1f7700bde73ed4fae7bd23c619.jpeg" class="d-block w-100" alt="...">
        </div>
        <div class="carousel-item">
          <img src="../assets/img/imgcourusel/crysis.jpg" class="d-block w-100" alt="...">
        </div>
        <div class="carousel-item">
          <img src="../assets/img/imgcourusel/division.jpg" class="d-block w-100" alt="...">
        </div>
      </div>
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  </div>
  <div class="weContent animscroll">
    <div class="whyWe">
      <h3>Почему стоит выбрать нас</h3>
    </div>
    <div class="b-we">
      <div class="we-item">
        <div class="we-img"><i class="fa-solid fa-sack-dollar fa-2xl" style="color: #ffffff;"></i></div>
        <div class="we-text"> Скидки<br> круглый год</div>
      </div>
      <div class="we-item">
        <div class="we-img"><i class="fa-solid fa-comment-dots fa-2xl" style="color: #ffffff;"></i></div>
        <div class="we-text"> Круглосуточная<br> поддержка</div>
      </div>
      <div class="we-item">
        <div class="we-img"><i class="fa-solid fa-users fa-2xl" style="color: #ffffff;"></i></div>
        <div class="we-text"> Активное<br> коммьюнити</div>
      </div>
      <div class="we-item">
        <div class="we-img"><i class="fa-solid fa-headset fa-2xl" style="color: #ffffff;"></i></div>
        <div class="we-text"> Любовь<br> к играм</div>
      </div>
    </div>
  </div>
  <div class="card-content">
    <div class="game-card">
      <div class="g-text">
        <h1>Игры на подбор</h1>
      </div>
      <hr>
      <hr>
    </div>
    <div class="news-card">
      <div class="n-text">
        <h1>Подборка новостей</h1>
      </div>
      <hr>
      <hr>
    </div>
  </div>

</div>

</template>

<style>
@import url("https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css");
* {
  box-sizing: border-box;
}

.courusel {
  animation: 1s ease-out 0s 1 slideInFromUP;
  position: relative;
  min-height: 50vh;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: end;
  -ms-flex-pack: end;
  justify-content: flex-end;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  padding-bottom: 6vh;
  margin-bottom: calc(var(--mb) - 6vh)
}


 .courusel::after {
    content: '';
    width: 100%;
    height: 100%;
    left: 0;
    top: 0;
    background: -webkit-gradient(linear,left top,left bottom,from(rgba(19,15,15,0)),color-stop(90%,#141111));
    background: linear-gradient(180deg,rgba(19,15,15,0) 0%,#141111 90%);
    position: absolute;
  }

  .social a {
    font-size: 22px;
    color: #fff;
  }

  .social a:hover {
    text-align: center;
    transition: 0.5s;
    color: red;
    text-shadow: 1px 1px 2px red, 0 0 2em red, 0 0 0.2em red;
  }

  .social {
    display: flex;
    position: absolute;
    flex-direction: column;
    gap: 20px;
    top: 15rem;
    left: 15rem;
    z-index: 14;
  }

  .weContent {
    min-height: 10vh;
    text-align: center;
    margin: 0 auto;
    padding: 0 ;
    background: #141111;
  }

.weContent h3{
    font-size: 38px;
    line-height: 1.1;
    letter-spacing: .04em;
    text-transform: uppercase;
    color: #fff;
  }

.we-img i {
  font-size: 100px;
}

.b-we {
  display: flex;
  justify-content: center;
  padding-top: 150px;
  margin: 0 auto;
}

.we-text {
  text-align: center;
  padding-top: 30px;
  color: #fff;
  text-transform: none;
}

  .we-item {
    padding: 2.5%;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
    text-align: center;
    width: calc((100%/5) - 24px);
    position: relative;
    margin: 0 12px;
    min-width: 185px;
  }


  .we-item::before {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 130%;
    border: 2px solid rgb(243 0 0 / 30%);
    border-radius: 12px;
    z-index: 1;
  }

  .video video{
    position: absolute;
    border-radius: 10%;
    top: 45rem;
    right: 10rem;
    width: 50rem;
    z-index: 1;
    opacity: .5;
  }

  .card-content{
    margin: 0;
    background: #141111;
  }

  .g-text h1{
    text-align: center;
    padding-top: 30px;
    color: #fff;
    text-transform: none;
  }

.card-content hr {
  margin: 0!important;
}

.n-text h1{
  text-align: center;
  padding-top: 30px;
  color: #fff;
  text-transform: none;
}
</style>