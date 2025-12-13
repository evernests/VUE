<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const ctime = ref('')

const updateTime = () => {
  const now = new Date()
  ctime.value = now.toLocaleTimeString()
}

onMounted(() => {
  updateTime()
  const timer = setInterval(updateTime, 1000)

  onUnmounted(() => {
    clearInterval(timer)
  })
})
</script>

<template>
  <div class="time">{{ ctime }}</div>
</template>

<style scoped>
.time {
  font-size: 32px;
  color: black;
  text-align: center;
}
</style>