<script setup>
import clock from "@/assets/img/clock.png"
import headset from "@/assets/img/headset.png"


const posts = [
  {
    title: "How to create your own podcast cover art?",
    date: "Dec 4, 2019",
    image: clock,
  },
  {
    title: "How to create your own podcast cover art?",
    date: "Dec 4, 2019",
    image: headset,
  },
];
</script>

<template>
  <div class="post container2">
    <h1 class="post__title">Latest Posts</h1>
    <div v-for="(post, index) in posts" :key="index" class="post__item">
      <img :src="post.image" :alt="post.title" class="post__image" />
      <div class="post__content">
        <h2 class="post__item-title">{{ post.title }}</h2>
        <p class="post__date">{{ post.date }}</p>
        <button class="post__button">Read More</button>
      </div>
    </div>
  </div>
  <div class="btn__footer container2">
    <button class="btn__footer__details">
      <span>View Blog</span>
      <img src="@/assets/icon/arrow-left.svg">
    </button>
  </div>
</template>

<style scoped>
.post {
  margin-top: 64px;
}

.post__title {
  font-size: 26px;
  font-weight:600;
  color: #222222;
  margin-bottom: 32px;
  font-family: Source Sans Pro;
}

.post__item {
  display: flex;
  align-items: flex-start;
  gap: 16px;
  margin-bottom: 24px;
}

.post__image {
  width: 120px;
  height: auto;
}

.post__content {
  display: flex;
  flex-direction: column;
  margin-left: 39px;
}

.post__item-title {
  font-size: 21px;
  font-weight: 600;
  color: #222222;
  font-family: Source Sans Pro;
}

.post__date {
  font-size: 14px;
  color: #979797;
  font-weight: 400;
  margin-top: 16px;
}

.post__button {
  align-self: flex-start;
  background: none;
  color:#7247CA;
  border: none;
  cursor: pointer;
  font-size: 14px;
  font-weight: 600;
  margin-top: 39px;
}
.btn__footer__details {
  border: none;
  border-radius: 10px;
  padding: 10px 20px;
  background: #F5F5F7;
  margin-top: 48px;
}
.btn__footer__details span {
  color: #7247CA;
  font-size: 14px;
  font-weight: 400;
  font-family: Source Sans Pro;
  margin-right: 8px;
}
@media (max-width: 769px) {
  .post {
    padding: 16px;
  }
  .post__item {
    display: flex;
    flex-direction: column;
  }
  .post__content {
    margin: 0;
  }
  .post__button {
    padding: 0;
    margin-top: 16px;
  }
  .post__item-title {
    margin-right: 150px;
  }
  .btn__footer {
    padding-left: 16px;

  }
}
</style>