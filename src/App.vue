<script setup>
import Avatar from './comp/Avatar.vue'
import Time from './comp/Time.vue'
import Social from './comp/Social.vue'
</script>

<template>
  <div class='mainContainer'>
    <!-- 懒得写css了，直接加div吧哈哈哈 -->
    <div style='height: 2px;'></div>
    <Avatar />
    <div class="name">EverNest</div>
    <Time />
    <Social />
  </div>
</template>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: "LXGW WenKai Mono TC", monospace;
}

  body {
  background-image: url('https://i.imgs.ovh/2025/12/13/CHj0Oq.jpeg');
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 100vh
}
  .mainContainer {
    height: auto;
    min-height: 200px;
    width: 100%;
    border-radius: 20px;
    background-color: rgba(255,255,255,0.4);
    backdrop-filter: blur(8px);
  }
</style>

<style scoped>
body {
  background-image: url('https://i.imgs.ovh/2025/12/13/CHj0Oq.jpeg');
  background-size: cover;

}
.name {
  font-size: 40px;
  text-align: center;
}
</style>
