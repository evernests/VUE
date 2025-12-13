<script setup></script>

<template>
  <div class="container">
    <a class="card" href="https://github.com/evernests/">Github</a>
    <a class="card" href="mailto:477522069@qq.com">QQ邮箱</a>
  </div>
  <div class='container'>
    <a class='card' href='#'>博客</a>
    <a class='card' href='mailto:VICTORIALAZY111@outlook.com'>Outlook</a>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  width: 100%;
  height: 50px;
  align-items: center;
  justify-content: center;
  gap: 20px;
}

.card {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 40px;
  min-width: 120px;
  max-width: 200px;
  width: 45%;
  border: 1px solid black;
  border-radius: 20px;
  text-align: center;
  text-decoration: none;
  color: inherit;
  cursor: pointer;
  transition: background-color 0.3s;
}

.card:hover {
  background-color: #f0f0f0;
}
</style>
