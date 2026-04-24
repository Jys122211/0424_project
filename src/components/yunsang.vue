<template>
  <div class="card highlight">
    <div class="badge">Web Developer</div>

    <div class="profile">Y</div>

    <h2>조윤상</h2>

    <div class="skills">
      <span>C</span>
      <span>Vue.js</span>
      <span>PHP</span>
      <span>CSS</span>
      <span>Unix</span>
      <span>JAVA</span>
    </div>
  </div>
</template>

<style scoped>
.card {
  height: 100%;
  border-radius: 20px;
  padding: 24px;
  color: white;

  display: flex;
  flex-direction: column;
  justify-content: center;

  position: relative;
  overflow: hidden;

  transition: 0.3s;
}

/* ⭐ 메인 카드 강조 */
.highlight {
  background: linear-gradient(135deg, #6366f1, #22d3ee);
  color: #0f172a;
}

/* 은은한 빛 효과 */
.highlight::before {
  content: '';
  position: absolute;
  inset: -2px;
  background: linear-gradient(45deg, #ffffff, transparent, #ffffff);
  opacity: 0.2;
  filter: blur(20px);
}

/* hover 효과 */
.highlight:hover {
  transform: scale(1.05);
  box-shadow: 0 30px 60px rgba(0, 0, 0, 0.5);
}

/* 상단 배지 */
.badge {
  position: absolute;
  top: 12px;
  right: 12px;
  font-size: 12px;
  background: rgba(255, 255, 255, 0.4);
  padding: 6px 12px;
  border-radius: 999px;
  font-weight: 600;
}

/* 프로필 */
.profile {
  width: 80px;
  height: 80px;
  margin: 0 auto 12px;
  border-radius: 50%;
  background: white;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 34px;
  font-weight: 900;
}

/* 텍스트 */
h2 {
  margin: 6px 0;
}

.goal {
  font-size: 14px;
  font-weight: 600;
  margin-bottom: 10px;
}

.desc {
  font-size: 13px;
  line-height: 1.6;
  margin-bottom: 16px;
}

/* 스킬 */
.skills {
  display: flex;
  justify-content: center;
  gap: 8px;
  flex-wrap: wrap;
}

.skills span {
  background: rgba(255, 255, 255, 0.5);
  padding: 6px 12px;
  border-radius: 999px;
  font-size: 12px;
  font-weight: 600;
}
</style>
