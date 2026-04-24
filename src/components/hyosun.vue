<template>
  <div class="card">
    <h2>효선</h2>
    <p>반갑습니당 👋</p>
    <div class="info-list">
      <span class="label">이름</span>
      <span class="value">안효선</span>
      <span class="label">MBTI</span>
      <span class="value">INFP</span>
      <span class="label">취미</span>
      <span class="value">게임, 유튜브보기</span>
    </div>
  </div>
</template>

<style scoped>
.card {
  border: 1px solid #ccc;
  border-radius: 10px;
  padding: 20px 40px;
  text-align: center;
}

.card h2 {
  margin-bottom: 5px;
}

.card p {
  margin: 5px 0;
  color: #555;
  font-size: 15px;
}

.info-list {
  display: grid;
  grid-template-columns: auto 1fr;
  gap: 6px 12px;
  margin-top: 12px;
  text-align: left;
}

.label {
  color: #888;
  font-size: 13px;
  font-weight: bold;
}

.value {
  color: #333;
  font-size: 13px;
}
</style>
