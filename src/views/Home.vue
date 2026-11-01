<template>
  <div class="home">
   <!-- ④ 关于我 -->
    <section class="section about">
      <img class="avatar" src="/bg.jpg" alt="口琴" />
      <div class="about-text"> 
        <h1>亦柠·前端开发 / 音乐人</h1>
        <p>37岁转行做音乐的前端程序员。会吹半音阶口琴，会用库乐队编曲，写代码也写旋律。泪点低，所以曲子都偏抒情。</p>
      </div>
    </section>
        <!-- 作品集 -->
    <section class="works">
      <h2 class="section-title">作品集</h2>
      <div class="card-grid">
        <WorkCard
          emoji="🎵"
          title="口琴作品集"
          desc="个人音乐展示页，收录口琴演奏作品与编曲试听，含作品详情与介绍。"
          tech="Vue3 · Vite · TypeScript"
          gradient="linear-gradient(135deg, #667eea 0%, #764ba2 100%)"
          preview-link="https://music-portfolio-7yl.pages.dev/"
          github-link="https://github.com/teresacyl123/music-portfolio.git"
        />
        <WorkCard
          emoji="🎛️"
          title="后台管理 Demo"
          desc="用户管理 CRUD 页面，含搜索筛选、分页、弹窗表单、表单校验，Mock 数据驱动。"
          tech="Vue3 · Element Plus · Mock"
          gradient="linear-gradient(135deg, #f093fb 0%, #f5576c 100%)"
          preview-link=" "
          github-link=" "
        />
        <WorkCard
          emoji="🎼"
          title="口琴调音器"
          desc="基于 Web Audio API 的实时频率检测工具，辅助口琴调音与音准练习。"
          tech="Web Audio API · Canvas · TS"
          gradient="linear-gradient(135deg, #4facfe 0%, #00f2fe 100%)"
          preview-link=" "
          github-link=" "
        />
      </div>
    </section>
</div>
</template>
<script setup lang="ts">
import WorkCard from '../components/WorkCard.vue'
</script>
<style scoped>
/* ④ 关于 */
.about {
  padding: 2rem;
  display: flex;
  align-items: center;
  gap: 3rem;
  background: #7878d7;
}
.avatar {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
  flex-shrink: 0; 
  border: 3px solid #0d1117;
}
.about-text h2 {
  text-align: left;
  margin-bottom: 1rem;
}
.about-text p {
  color: #ccc;
  line-height: 1.8;
  margin-bottom: 1rem;
}
.about-text a {
  color: #7c5cbf;
  text-decoration: none;
}
.home {
  min-height: 100vh;
  background: #0d1117;
}
h1{color: white;}
/* Hero */
.hero {
  padding: 80px 24px 60px;
  text-align: center;
}

.avatar-ring {
  width: 120px;
  height: 120px;
  margin: 0 auto 24px;
  border-radius: 50%;
  padding: 4px;
  background: linear-gradient(135deg, #667eea, #764ba2, #4facfe);
}
 
.hero-title {
  font-size: 36px;
  font-weight: 700;
  color: #e8e8e8;
  margin: 0 0 8px;
}

.hero-sub {
  font-size: 16px;
  color: #8cb4ff;
  margin: 0 0 16px;
}

.hero-desc {
  font-size: 14px;
  color: #6a7088;
  max-width: 420px;
  margin: 0 auto;
  line-height: 1.7;
}

/* Works */
.works {
  padding: 40px 24px 80px;
  max-width: 1100px;
  margin: 0 auto; 
}

.section-title {
  font-size: 24px;
  font-weight: 600;
  color: #e8e8e8;
  text-align: center;
  margin: 0 0 40px;
}

.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 24px;
  justify-items: center;
}

/* Footer */
.footer {
  text-align: center;
  padding: 32px;
  border-top: 1px solid #1a2040;
  color: #4a5080;
  font-size: 13px;
}

@media (max-width: 100vw) {
  .hero-title { font-size: 28px; }
  .card-grid { grid-template-columns: 1fr; }
}
</style>