<script setup></script>

<template>
  <header>TRIP IS WAITING</header>
</template>

<style scoped>
header {
  box-sizing: border-box;
  width: 1440px;
  height: 58px;
  padding: 0 20px;
  display: flex;
  align-items: center;
  color: var(
    --font-color
  ); /* 투명도 때문에 폰트 컬러 적용 안되고, 폰트 패밀리 전역 지정 안되는 거 바꿔야 함 */
  background-color: var(--navbar-color);
  opacity: 0.5;
  font-family: "Pretendard";
  font-size: 20px;
  letter-spacing: 1px;
}
</style>
