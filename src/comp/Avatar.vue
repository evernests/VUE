<template>
  <div class="avatar" :class="{ 'enlarged': isEnlarged }" @click="toggleEnlarge">
  </div>
</template>

<script setup>
import { ref } from 'vue'

const isEnlarged = ref(false)

const toggleEnlarge = () => {
  isEnlarged.value = !isEnlarged.value
}
</script>

<style scoped>
.avatar {
  margin-top: 2px;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100px;
  height: 100px;
  border-radius: 50%;
  border: 1px solid black;
  background-color: green;
  background-image: url('https://i.imgs.ovh/2025/12/12/C2iSDC.jpeg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  cursor: pointer;
  transition: transform 0.3s ease;
  margin: 0 auto;
}

.avatar.enlarged {
  transform: scale(1.4);
}
</style>
