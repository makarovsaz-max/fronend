<script setup>

</script>

<template>
  <header>
    <div class="head">
      <a href=""><i class="fa-sharp fa-solid fa-magnifying-glass"></i></a>
      <a href="">Главная</a>
      <a href="">Новости</a>
      <div class="head-logo">
        <img src="../assets/img/лого.svg" alt="" width="100px">
      </div>
      <a href="">Турниры</a>
      <a href="">Магазин</a>
      <a href="/auth" id="authform" ><i class="fa-solid fa-user-plus"></i></a>
    </div>
  </header>
</template>

<style>
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css');

.head {
  animation: 1s ease-out 0s 1 slideInFromLeft;
  background: -webkit-gradient(linear, left bottom, left top, from(rgba(19, 15, 15, 0)), color-stop(9.38%, rgba(19, 15, 15, .05)), color-stop(20.83%, rgba(19, 16, 16, .15)), color-stop(46.35%, rgba(20, 17, 17, .49)), color-stop(75%, rgba(20, 17, 17, .7)), to(rgba(20, 17, 17, .95)));
  background: linear-gradient(0deg, rgba(19, 15, 15, 0) 0%, rgba(19, 15, 15, .05) 9.38%, rgba(19, 16, 16, .15) 20.83%, rgba(20, 17, 17, .49) 46.35%, rgba(20, 17, 17, .7) 75%, rgba(20, 17, 17, .95) 100%);
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  position: fixed;
  left: 0;
  top: 0;
  width: 100%;
  z-index: 1000;
}

.head a {
  text-decoration: none;
  font-size: 24px;
  color: #fff;
}

.head a:hover {
  text-align: center;
  transition: 0.5s;
  color: red;
  text-shadow: 1px 1px 2px red, 0 0 2em red, 0 0 0.2em red;
}


</style>