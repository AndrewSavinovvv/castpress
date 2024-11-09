<script setup>

</script>

<template>
  <div class="player container2">
    <div>
      <img src="@/assets/img/main.png" alt="">
    </div>
    <h1 class="player__title">How to rapidly test any experience!</h1>
    <figure>
      <audio class="audio__player" controls src="/media/cc0-audio/t-rex-roar.mp3"></audio>
    </figure>
    <div class="player__footer">
      <h6 class="player__footer__title">LISTEN ON</h6>
      <div class="player__footer__img">
        <img src="@/assets/icon/spotify.svg" alt="">
        <img src="@/assets/icon/spotify.svg" alt="">
        <img src="@/assets/icon/spotify.svg" alt="">
      </div>
    </div>
  </div>
</template>

<style scoped>
.player {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-top: 96px;
  align-items: center;
}

.player__title {
  font-family: Source Sans Pro;
  font-size: 26px;
  font-weight: 600;
  padding-top: 39px;
}
.player__footer {
  font-family: Source Sans Pro;
  font-size: 12px;
  font-weight: 600;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 20px;
}
.player__footer__img  {
  gap:30px
}
.audio__player {
  width: 550px;
  border: none;
  background: none;
  margin-top: 44px;
}
.player__footer__img {
  display: flex;
  gap: 30px;
}
.player__footer__title {
  font-family: Source Sans Pro;
  font-size: 12px;
  font-weight: 600;
  color: #222222;
  margin-bottom: 12px;
}

@media (max-width: 769px) {
  .audio__player {
    width: 400px;
  }
  .player__title {
    word-wrap: break-word;
    overflow-wrap: break-word;
    padding: 20px;
    text-align: center;
  }
  .player {
    padding-top: 48px;
  }
}
</style>