<script setup>
const showNewLabel = [true, false, false];
</script>

<template>
  <div class="news container2">
    <p class="news_info">
      <span v-if="showNewLabel[0]" class="news_info__new">
        new
      </span>Business  |  Jan 18, 2021</p>
    <h1 class="news__title">23 - How to rapidly test any experience!</h1>
    <p class="news__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lorem ipsum dolor sit amet, consect adipiscing elit. Sed at arcu dui. Aenean placerat mauris nisl...</p>
    <div class="news__btns">
      <button class="news__btn">
        <img src="@/assets/icon/btn.svg" alt="">
      </button>
      <p class="news__btn__text">listen now</p>
    </div>
  </div>
  <div class="news container2">
    <p class="news_info">
      <span v-if="showNewLabel[1]" class="news_info__new">
        new
      </span>Education  |  Jan 18, 2021</p>
    <h1 class="news__title">22 - How to rapidly test any experience!</h1>
    <p class="news__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lorem ipsum dolor sit amet, consect adipiscing elit...</p>
    <div class="news__btns">
      <button class="news__btn">
        <img src="@/assets/icon/btn.svg" alt="">
      </button>
      <p class="news__btn__text">listen now</p>
    </div>
  </div>
  <div class="news container2">
    <p class="news_info">
      <span v-if="showNewLabel[2]" class="news_info__new">
        new
      </span>Market  |  Jan 18, 2021</p>
    <h1 class="news__title">21 - How to rapidly test any experience!</h1>
    <p class="news__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lorem ipsum dolor sit amet, consect adipiscing elit...</p>
    <div class="news__btns">
      <button class="news__btn">
        <img src="@/assets/icon/btn.svg" alt="">
      </button>
      <p class="news__btn__text">listen now</p>
    </div>
  </div>
  <div class="news__footer container2">
    <span class="news__footer__pagination">1</span>
    <span class="news__footer__pagination">2</span>
    <span class="news__footer__pagination">3</span>
    <span class="news__footer__pagination">....</span>
    <span class="news__footer__pagination">
      <img src="@/assets/icon/arrow-left.svg" alt="">
    </span>
  </div>
</template>

<style scoped>
.news_info{
  font-size: 14px;
  font-family: Source Sans Pro;
  font-weight: 400;
  color: #979797;
  justify-content: space-between;
  margin-top: 96px;
}
.news_info__new {
  color: #7247CA;
  padding: 6px 8px;
  background: #F5F5F7;
  border-radius: 5px;
  text-align: center;
  margin-right: 6px;
  text-transform: uppercase;
  font-size: 10px;
  font-weight: 600;
}
.news__title {
  font-size: 21px;
  font-weight: 600;
  font-family: Source Sans Pro;
  color: #222222;
  margin-top: 14px;
  margin-bottom: 12px;
}
.news__btns {
  display: flex;
  align-items: center;
  margin-top: 16px;
}
.news__btn {
  background: none;
  border: none;
  margin-right: 10px;
  padding: 0;
}
.news__btn__text {
  color: #7247CA;
  font-size: 12px;
  font-weight: 600;
  font-family: Source Sans Pro;
  text-transform: uppercase;
}
.news__footer {
  display: flex;
  margin-top: 64px;
}
.news__footer__pagination {
  padding: 8px 12px;
  background: #F5F5F7;
  color: #555555;
  font-size: 12px;
  font-weight: 400;
  font-family: Source Sans Pro;
  margin-right: 5px;
}
.news__footer__pagination:nth-child(5) {
  background: none;
}
@media (max-width: 769px) {
  .news {
    padding: 16px;
  }
  .news__title,.news__text {
    word-wrap: break-word;
    overflow-wrap: break-word;
  }
  .news_info {
    margin-top: 48px;
  }
  .news__footer {
    padding: 16px;
    margin-top: 32px;
  }
}
</style>