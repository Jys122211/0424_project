<template>
  <div class="card">
    <div class="top-section">
      <img :src="profileImg" class="profile-img" />
      <div class="name-area">
        <h2>효선</h2>
        <p class="greeting">반갑습니당 👋</p>
      </div>
    </div>
    <div class="divider"></div>
    <div class="info-list">
      <span class="label">이름</span><span class="value">안효선</span>
      <span class="label">MBTI</span><span class="value">INFP</span> <span class="label">취미</span
      ><span class="value">게임, 유튜브보기</span>
    </div>
  </div>
</template>

<script setup>
import profileImg from '@/assets/img/hs.png';
</script>

<style scoped>
.card {
  background: linear-gradient(145deg, #fff5f5, #fde8e8);
  border: 1.5px solid #e8b4b8;
  border-radius: 16px;
  padding: 20px;
  box-shadow: 3px 3px 10px rgba(232, 180, 184, 0.35);
}

.top-section {
  display: flex;
  align-items: center;
  gap: 14px;
  margin-bottom: 12px;
}

.profile-img {
  width: 70px;
  height: 70px;
  border-radius: 50%;
  object-fit: cover;
  border: 2px solid #e8b4b8;
}

.name-area h2 {
  margin: 0 0 4px;
  font-size: 20px;
  color: #c9747a;
}

.greeting {
  margin: 0;
  font-size: 13px;
  color: #c9747a;
}

.divider {
  height: 1px;
  background: #e8b4b8;
  margin-bottom: 12px;
}

.info-list {
  display: grid;
  grid-template-columns: auto auto;
  gap: 6px 14px;
}

.label {
  color: #c9747a;
  font-size: 13px;
  font-weight: bold;
}

.value {
  color: #555;
  font-size: 13px;
}
</style>
