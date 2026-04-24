<template>
  <div class="profile-card">
    <div class="image-wrapper">
      <img src="@/assets/img/dongju.png" alt="프로필 사진" class="profile-image" />
    </div>

    <h2 class="name">이름: 동주</h2>
    <p class="age">mbti: ISFJ</p>

    <p class="intro">
      안녕하세요! 동주입니다.<br/>
      vue와 git을 활용한 자기소개 페이지입니다.
    </p>
  </div>
</template>

<script setup>
</script>

<style scoped>
.profile-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  background-color: #eae9e9;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding: 15px;
  box-sizing: border-box;
}

.image-wrapper {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background-color: #e0e0e0;
  margin-bottom: 10px;
  overflow: hidden;
  flex-shrink: 0;
}

.profile-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.name {
  margin: 0;
  font-size: 16px;
  font-weight: bold;
  color: #333;
}

.age {
  margin: 4px 0 8px 0;
  font-size: 13px;
  color: #666;
}

.intro {
  margin: 0;
  font-size: 12px;
  color: #444;
  text-align: center;
  line-height: 1.4;
  width: 100%; /* 너비 확보 */
  
  /* 스크롤 생성 설정 */
  overflow-y: auto; /* 내용이 넘치면 세로 스크롤 생성 */
  flex-grow: 1; /* 남은 공간을 자기소개가 모두 차지하도록 설정 */
  padding-right: 5px; /* 스크롤바가 글자를 가리지 않게 여백 추가 */
}

.intro::-webkit-scrollbar {
  width: 4px;
}
.intro::-webkit-scrollbar-thumb {
  background: #ccc;
  border-radius: 4px;
}
</style>