<script setup>

</script>

<template>
  <footer class="footer">
    <div class="first"><div class="first__left-side"><div class="logo"></div> <div class="address">
      <span>VENTORSPACE © 2023 Все права защищены</span>
      <span>Newera Frozen PTE. Limited, 3 PHILLIP STREET #14-05 ROYAL GROUP BUILDING SINGAPORE (048693)</span>
      <span>E.K. 11 Holdings Ltd, Agias Sofias 103, 3066, Limassol, Cyprus</span></div></div> <div class="first__right-side">
      <div  class="socials">
                    <span  class="socials__title">
                        Следите за нами:
                    </span>
        <a href="" target="_blank" rel="noopener" class="socials__list">
          <i class="fa-brands fa-facebook"></i>
        </a>
        <a href="" target="_blank" rel="noopener" class="socials__list">
          <i class="fa-brands fa-twitter"></i>
        </a>
        <a href="" target="_blank" rel="noopener" class="socials__list">
          <i class="fa-brands fa-youtube"></i>
        </a>
        <a href="" target="_blank" rel="noopener" class="socials__list">
          <i class="fa-brands fa-instagram"></i>
          <a  href="" target="_blank" rel="noopener" class="socials__list">
            <i class="fa-brands fa-discord"></i>
            </a>
          </a>
          <a href="" target="_blank" rel="noopener" class="socials__list">
            <i class="fa-brands fa-tiktok"></i>
          </a>
          <a href="" target="_blank" rel="noopener" class="socials__list">
            <i class="fa-brands fa-steam"></i>
          </a>
      </div>
    </div>
    </div>
  </footer>
</template>

<style>

footer {
  background-color: #101117;
  color: #515765;
  padding: 1.25rem 0;
}

.first {
  display: flex;
  flex: 1 1 50%;
  flex-direction: row;
  justify-content: space-between;
  padding: 0 1.875rem;
}

.first__left-side .address {
  display: flex;
  flex-direction: column;
}


.first__left-side .logo {
  background-image: url("../assets/img/лого.svg");
  background-size: cover;
  height: 2.875rem;
  margin-right: 0.625rem;
  width: 2.3125rem;
}



.first__left-side {
  align-items: center;
  display: flex;
  flex: 1 1 100%;
  font-size: 1rem;
  font-weight: 900;
  height: 100%;
  line-height: .875rem;
}

.first__right-side  {
  align-self: center;
  display: flex;
  flex: 1 1 100%;
  flex-direction: row;
  justify-content: flex-end;
  margin: 0;
  width: 100%;
}

.socials {
  align-items: center;
  align-self: start;
  display: flex;
  gap: 0 1.875rem;
  justify-content: flex-end;
}

a {
  color: #fff;
  cursor: pointer;
  -webkit-text-decoration: none;
  text-decoration: none;
}

a:hover {
  color: #fff;
  transition: 0.5s;
  -webkit-transform:scale(1.5);
}

</style>