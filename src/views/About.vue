<template>
  <div class="home">
   <!-- ④ 关于我 -->
    <section class="section about">
      <img class="avatar" src="/bg.jpg" alt="口琴" />
      <div class="about-text">
        <h1>关于我</h1>
        <h2>亦柠·前端开发 / 音乐人</h2>
        <p class="p_info"><text>
37 岁转行，从代码走向音乐。会吹半音阶口琴，会用库乐队编曲，写代码也写旋律。泪点低，所以曲子都偏抒情。
</text></p>
<p class="p_info">
  <text>技术栈：</text>
<text>
前端：Vue3 / Vite / TypeScript / Element Plus</text>
<text>工具：Git / Cloudflare Pages / Web Audio API</text>
<text>音乐：半音阶口琴演奏 · 库乐队编曲 · 音乐制作</text>
</p>
<p class="p_info">
<text>个人标签：</text> 
<text>跨界开发者 · 前端转音乐 · 独立作品全流程 · Vue3 生态</text>
    </p>
     <p class="p_info">
        <a href="mailto:chenyilin2009@yeah.net">邮箱:chenyilin2009@yeah.net</a>
        <a href="https://github.com/teresacyl123" target="_blank">GitHub:teresacyl123</a>
     </p>
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
h1,h2{color: white;}
.p_info text ,.p_info a{display: block; text-align: left;color: white;}

.avatar {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
  flex-shrink: 0; 
  border: 3px solid #0d1117;
}
.about-text h2 { 
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
  border:red 1px solid;
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
.p_info a {
  color: white;
  text-decoration: none; /* 去掉下划线 */ 
}

.p_info a:hover {
  color: black; /* 鼠标悬停变色 */ 
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