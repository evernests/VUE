<template>
  <div :class="['app', theme]">
    <header class="header">
      <img class="avatar" src="https://i.imgs.ovh/2025/12/09/CWGhre.jpeg" alt="头像" />
      <button class="toggle-btn" @click="toggleTheme">
        {{ theme === 'light' ? '🌙 夜间' : '☀️ 日间' }}
      </button>
    </header>

    <!-- 社交区域 -->
    <section class="social">
      <h2>联系我</h2>
      <div class="social-links">
        <a href="https://github.com/evernests" target="_blank" class="link github">GitHub</a>
        <a href="mailto:477522069@qq.com" class="link email">Email</a>
      </div>
    </section>

    <!-- 作品区域 -->
    <section class="works">
      <h2>作品</h2>
      <div class="cards">
        <div class="card">
          <h3>博客</h3>
          <p>来看我的博客喵，谢谢喵。关于我的一些事情也在博客里哦。</p>
          <a class='link github' href='https://blog.evernests.qzz.io/'>点击访问博客</a>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "PersonalHome",
  data() {
    return {
      theme: "light"
    };
  },
  methods: {
    toggleTheme() {
      this.theme = this.theme === "light" ? "dark" : "light";
    }
  }
};
</script>

<style scoped>
* {
  box-sizing: border-box;
  margin: 0;
  padding: p;
}
/* 基础样式 */
.app {
  font-family: "Segoe UI", sans-serif;
  transition: background-color 0.5s ease, color 0.5s ease;
  min-height: 100vh;
  padding: 20px;
}

/* 日间与夜间主题 */
.app.light {
  background: #fdf6e3;
  color: #333;
}
.app.dark {
  background: #2e3440;
  color: #eceff4;
}

/* 顶部头像 */
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.avatar {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  border: 3px solid #ccc;
  animation: fadeIn 1.5s ease;
}
.toggle-btn {
  padding: 8px 16px;
  border: none;
  border-radius: 20px;
  cursor: pointer;
  background: #ffb347;
  color: #fff;
  transition: transform 0.3s ease;
}
.toggle-btn:hover {
  transform: scale(1.1);
}

/* 社交区域 */
.social {
  margin-top: 40px;
  text-align: center;
}
.social-links {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-top: 10px;
}
.link {
  padding: 10px 20px;
  border-radius: 10px;
  text-decoration: none;
  color: inherit;
  background: rgba(255, 255, 255, 0.2);
  transition: background 0.3s ease, transform 0.3s ease;
}
.link:hover {
  background: rgba(255, 255, 255, 0.4);
  transform: translateY(-3px);
}

/* 作品卡片 */
.works {
  margin-top: 40px;
}
.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
}
.card {
  width: 250px;
  padding: 20px;
  border-radius: 15px;
  background: rgba(255, 255, 255, 0.1);
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  animation: slideUp 0.8s ease;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.2);
}

/* 动画 */
@keyframes fadeIn {
  from { opacity: 0; transform: scale(0.9); }
  to { opacity: 1; transform: scale(1); }
}
@keyframes slideUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
</style>

