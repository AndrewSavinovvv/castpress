<script setup>

</script>

<template>
  <footer class="footer container2">
    <div class="footer__content">
      <ul class="footer__list">
        <li><a href="#">Episodes</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#">Donate</a></li>
      </ul>

      <div class="footer__tile">
        <h3>Newsletter</h3>
        <p class="footer__tile__text"> Sign up now;  get closer to our action.</p>
        <div class="footer__subscribe">
          <input type="email" placeholder="Email  adress..." class="footer__input" />
          <button class="footer__button">
            <img src="@/assets/icon/arrow-left.svg" alt="">
          </button>
        </div>
      </div>
    </div>
    <div class="footer__bottom">
      <p>PodcastTheme by VitaThemes | Privacy policy </p>
      <div class="footer__icons">
        <a href="#"><i class="">
          <img src="@/assets/icon/facebook.svg" alt="">
        </i></a>
        <a href="#"><i class="">
          <img src="@/assets/icon/git.svg" alt="">
        </i></a>
        <a href="#"><i class="">
          <img src="@/assets/icon/twitter.svg" alt="">
        </i></a>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  color: #555555;;
  margin-top: 64px;
  border-top: 1px solid #ddd;
}

.footer__content {
  display: flex;
  justify-content: space-between;
  margin-top: 64px;
}

.footer__list {
  list-style: none;
  padding: 0;
}

.footer__list li {
  margin-bottom: 9px;
  color: #555555;
  font-size: 14px;
  font-weight: 600;
  font-family: Source Sans Pro;
}

.footer__list a {
  text-decoration: none;
  color: #555555;
}

.footer__tile {
  max-width: 300px;
}

.footer__tile h3 {
  margin-top: 0;
  font-size: 16px;
  color: #222222;
  font-weight: 600;
  font-family: Source Sans Pro;
  text-transform: uppercase;
  margin-bottom: 8px;
}
.footer__tile__text {
  color: #555555;
  font-weight: 400;
  font-size: 12px;
  font-family: Source Sans Pro;
}
.footer__subscribe {
  display: flex;
}

.footer__input {
  flex: 1;
  padding: 14px;
  border: none;
  border-radius: 4px;
}

.footer__button {
  padding: 8px 12px;
  background-color: #7247CA;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.footer__bottom {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
}
.footer__bottom p {
  color: #222222;
  margin-bottom: 24px;
  margin-top: 89px;
}
.footer__icons a {
  margin-left: 23px;
}

.footer__input {
  flex: 1;
  padding: 10px;
  border-radius: 4px 0 0 4px;
  color: #555555;
  background-color: #F5F5F7;
  font-family: inherit;
  margin-top: 14px;
}

.footer__button {
  padding: 8px 12px;
  background-color: #7247CA;
  color: white;
  border: none;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 14px;
}

.footer__subscribe {
  display: flex;
  margin-top: 10px;
}
@media (max-width: 769px) {
  .footer__content {
    flex-direction: column;
  }

  .footer__tile {
    max-width: 100%;
    margin-bottom: 20px;
  }

  .footer__subscribe {
    display: flex;
    flex-direction: column;
  }
  .footer__input{
    position: relative;
    width: 370px;
    margin-top: 10px;
  }
  .footer__button {
    position: absolute;
    right: 25px;
  }
  .footer__bottom p {
    margin-top: 20px;
  }
  .footer__bottom {
    padding-right: 20px;
  }
}
</style>