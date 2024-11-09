<template>
  <div class="header container">
    <h1 class="header__title">CastPress.</h1>
    <div class="header__burger">
      <div class="burger-line"></div>
      <div class="burger-line"></div>
    </div>
    <ul class="header__list">
      <li>
        <a href="">
          <span>Episodes</span>
          <img src="@/assets/icon/arrow-down.svg" alt="">
        </a>
      </li>
      <li><a href="">Blog</a></li>
      <li><a href="">Contact</a></li>
      <li>
        <a href="" class="header__donate">
          <img src="@/assets/icon/donate.svg" alt="">
          <span>Donate</span>
        </a>
      </li>
      <li class="header__search">
        <a href="">
          <img src="@/assets/icon/search.svg" alt="">
        </a>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  padding-top: 39px;
}

.header__title {
  color: #222222;
  font-size: 19px;
  font-weight: 400;
  font-family: Oswald;
}

.header__list {
  display: flex;
  list-style: none;
  gap: 39px;
  text-transform: uppercase;
  color: #222222;
  font-size: 12px;
  font-weight: 600;
  align-items: baseline;
  font-family: Source Sans Pro;
}

.header__list li {
  display: flex;
  align-items: center;
}

.header__list li a {
  display: flex;
  align-items: center;
  gap: 6px;
  color: #222222;
  text-decoration: none;
}

.header__donate {
  color: #7247CA !important;
  display: flex;
  align-items: flex-start !important;
}

.header__search {
  display: flex;
}

@media (max-width: 769px) {
  .header__list {
    display: none;
  }
  .header__burger {
    cursor: pointer;
    width: 30px;
    height: 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding-right: 16px;
  }

  .burger-line {
    width: 100%;
    height: 1px;
    background-color: #222222;
  }
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 24px;
    border-bottom: 1px solid #EAEAEE;
    padding-bottom: 24px;
  }

  .header__title {
    padding-left: 16px;
  }
}

@media (min-width: 769px) {
  .header__burger {
    display: none;
  }
}
</style>