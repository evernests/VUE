<script setup>
import Avatar from './comp/Avatar.vue'
import Time from './comp/Time.vue'
import Social from './comp/Social.vue'
</script>

<template>
  <div style='height: 2px;'></div>
  <Avatar />
  <div class="name">EverNest</div>
  <Time />
  <Social />
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
