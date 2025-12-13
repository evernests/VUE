<script setup>
import Avatar from './comp/Avatar.vue'
import Time from './comp/Time.vue'
import Social from './comp/Social.vue'
</script>

<template>
  <div class='mainContainer'>
    <!-- 懒得写css了，直接加div吧哈哈哈 -->
    <div style='height: 5px;'></div>
    
    <Avatar />
    <div style='height: 5px;'></div>
    
    <div class="name">EverNest</div>
    <div style='height: 5px;'></div>
    
    <Time />
    <div style='height: 5px;'></div>
    
    <Social />
    <div style='height: 5px;'></div>
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
    display: flex;
    align-items: center;
    justify-content: center;
    background-image: url('https://i.imgs.ovh/2025/12/13/CHj0Oq.jpeg');
    background-size: cover;
    background-repeat: no-repeat;
    min-height: 100vh
}
  .mainContainer {
    height: auto;
    min-height: 200px;
    width: 90vw;
    border-radius: 20px;
    background-color: rgba(255,255,255,0.4);
    backdrop-filter: blur(8px);
  }

  @media (orientation: landscape) {
    body {
      background-image: url('https://i.imgs.ovh/2025/12/13/CHf3sg.jpeg')
    }
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
