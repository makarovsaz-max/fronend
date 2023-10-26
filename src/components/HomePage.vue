<script setup>

</script>

<template>
  <div class="social">
    <a href=""> <i class="fa-brands fa-telegram"></i></a>
    <a href=""> <i class="fa-brands fa-instagram"></i> </a>
    <a href=""><i class="fa-brands fa-github"></i> </a>
  </div>
  <div class="game-control">
    <div class="game-control_btn_next"></div>
    <div class="game-control_progressbar">
      <div class="game-control_progressbar" style="height: 20%"></div>
    </div>
    <div class="game-control_btn"></div>
  </div>
  <div class="courusel">
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

</template>

<style>
@import url("https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css");
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
    position: fixed;
    flex-direction: column;
    gap: 20px;
    top: 15rem;
    left: 15rem;
    z-index: 14;
  }

.b-control_btn_next::before {
  content: '';
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  border-radius: 50px;
  border: 2px solid rgba(255,255,255,.3);
  -webkit-transition: .3s;
  transition: .3s;
}
</style>