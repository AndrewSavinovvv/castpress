<script setup>
import man from "@/assets/img/man.png"
import woman from "@/assets/img/woman.png"

const teamMembers = [
  {
    name: "Aida Cave",
    role: "Position",
    image: woman,
  },
  {
    name: "Nick Carleton",
    role: "Position",
    image: man,
  },
];
</script>

<template>
  <div class="team container2">
    <h1 class="team__title">Team</h1>
    <div class="team__cards">
      <div v-for="(member, index) in teamMembers" :key="index" class="team__card">
        <img :src="member.image" :alt="member.name" class="team__photo" />
        <p class="team__role">{{ member.role }}</p>
        <h2 class="team__name">{{ member.name }}</h2>
        <div class="team__icons">
          <img src="@/assets/icon/soundclub.svg" alt="Facebook" class="team__icon" />
          <img src="@/assets/icon/soundclub.svg" alt="Twitter" class="team__icon" />
          <img src="@/assets/icon/soundclub.svg" alt="LinkedIn" class="team__icon" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.team {
  margin-top: 64px;
}

.team__title {
  font-size: 28px;
  font-weight: bold;
  color: #222222;
  margin-bottom: 32px;
}

.team__cards {
  display: flex;
  gap: 69px;
  justify-content:space-between;
}

.team__card {
  width: 280px;
  background: #F5F5F7;
  border: 1px solid #e0e0e0;
  border-radius: 8px;
}

.team__photo {
  width: 100%;
  height: auto;
  margin-bottom: 16px;
}

.team__name {
  font-size: 18px;
  font-weight: 400;
  padding-left: 16px;
  color: #222222;
  margin-bottom: 39px;
}

.team__role {
  font-size: 12px;
  color: #7247CA;
  margin-bottom: 16px;
  padding-left: 16px;
  font-family: Source Sans Pro;
  text-transform: uppercase;
  font-weight: 600;
}

.team__icons {
  display: flex;
  gap: 8px;
  padding-left: 15px;
}

.team__icon {
  height: 12px;
  width: 12px;
  margin-bottom: 12px;
}
@media (max-width: 769px) {
  .team__cards{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .team__title {
    padding-left: 16px;
  }
  .team__card {
    width: 390px;
  }
}
</style>