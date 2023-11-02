<script setup>
import _ from "lodash";

const debounceHandler = _.debounce((event) => {
  console.log(event.target.value);
}, 500);
</script>

<template>
  <div class="search">
    <input @input="debounceHandler" type="text" placeholder="검색어 입력" />
    <img
      src="https://s3.ap-northeast-2.amazonaws.com/cdn.wecode.co.kr/icon/search.png"
    />
  </div>
</template>

<style scoped>
.search {
  position: relative;
  width: 300px;
  border: 1px solid #bbb;
  border-radius: 8px;
}

input {
  box-sizing: border-box;
  width: 85%;
  padding: 10px 12px;
  border-radius: 8px 0 0 8px;
  border: none;
  font-size: 14px;
}

img {
  cursor: pointer;
  position: absolute;
  width: 17px;
  top: 10px;
  right: 14px;
  margin: 0;
}
</style>
