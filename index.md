---
layout: default
title: 马斯克铁粉站
---

<div class="hero">
  <h1>🚀 马斯克铁粉站</h1>
  <p>中文互联网最系统的马斯克知识库：深度文章、名言、X 发言、故事、时间线。</p>
  <a href="/long/" class="hero-btn">开始阅读</a>
</div>

<!-- 必读推荐 -->
<section>
  <h2>⭐ 必读推荐</h2>
  <div class="card">
    <div class="card-icon">📘</div>
    <div class="card-content">
      <a class="card-title" href="/long/2025/11/30/elon-musk-intro.html">
        埃隆·马斯克：改变世界的工程狂人
      </a>
      <p class="card-desc">一文读懂马斯克的成长轨迹、创办公司背后的逻辑，以及他的工程思维。</p>
      <span class="card-date">2025-11-30</span>
    </div>
  </div>
</section>

<!-- 栏目导航 -->
<section>
  <h2>🔥 四大栏目</h2>
  <div class="nav-grid">

    <a class="nav-card" href="/long/">
      <div class="nav-icon">📝</div>
      <div class="nav-title">大作文</div>
      <p>对马斯克现象的深度解析</p>
    </a>

    <a class="nav-card" href="/quotes/">
      <div class="nav-icon">💬</div>
      <div class="nav-title">马斯克名言</div>
      <p>值得深思的金句与解释</p>
    </a>

    <a class="nav-card" href="/tweets/">
      <div class="nav-icon">🐦</div>
      <div class="nav-title">X言X语</div>
      <p>马斯克 X 上的发言整理</p>
    </a>

    <a class="nav-card" href="/gossip/">
      <div class="nav-icon">😎</div>
      <div class="nav-title">马斯克八卦</div>
      <p>轻松有趣的幕后故事</p>
    </a>

  </div>
</section>

<!-- 最新文章 -->
<section>
  <h2>📰 最新文章</h2>
  <ul class="latest-list">
    {% for post in site.posts limit:100 %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <small>{{ post.date | date: "%Y-%m-%d" }}</small>
      </li>
    {% endfor %}
  </ul>
</section>

<!-- 数据统计 -->
<p class="stats">
本站总访问量：<span id="busuanzi_value_site_pv">加载中...</span> 次  
<br>
本站访客数：<span id="busuanzi_value_site_uv">加载中...</span> 人  
</p>

<style>
/* 页面整体排版 */
section { margin: 40px 0; }
h2 { margin-bottom: 20px; }

/* Hero 区域 */
.hero {
  text-align: center;
  padding: 60px 20px;
  background: linear-gradient(135deg, #1a1a1a, #333);
  color: white;
  border-radius: 16px;
  margin-bottom: 40px;
}
.hero-btn {
  display: inline-block;
  margin-top: 20px;
  padding: 12px 28px;
  background: #ffcc00;
  color: #000;
  font-weight: bold;
  border-radius: 50px;
  text-decoration: none;
  transition: 0.25s;
}
.hero-btn:hover {
  background: #ffe680;
}

/* 必读推荐卡片 */
.card {
  display: flex;
  gap: 16px;
  padding: 20px;
  border-radius: 16px;
  background: #f5f5f5;
  border: 1px solid #ddd;
}
.card-icon {
  font-size: 38px;
}
.card-title {
  font-size: 20px;
  font-weight: bold;
  text-decoration: none;
}
.card-title:hover {
  text-decoration: underline;
}
.card-desc {
  margin: 6px 0 4px;
  color: #555;
}
.card-date {
  font-size: 13px;
  color: #999;
}

/* 栏目导航 Grid */
.nav-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 20px;
}
.nav-card {
  display: block;
  background: #fafafa;
  padding: 20px;
  border-radius: 16px;
  text-decoration: none;
  color: inherit;
  text-align: center;
  border: 1px solid #ddd;
  transition: 0.25s;
}
.nav-card:hover {
  background: #f0f0f0;
  transform: translateY(-3px);
}
.nav-icon {
  font-size: 30px;
  margin-bottom: 10px;
}
.nav-title {
  font-size: 18px;
  font-weight: bold;
}

/* 最新文章列表 */
.latest-list {
  list-style: none;
  padding: 0;
}
.latest-list li {
  margin: 10px 0;
}

/* 访问量统计排版 */
.stats {
  margin-top: 40px;
  text-align: center;
  color: #666;
}

/* 深色模式支持 */
@media (prefers-color-scheme: dark) {
  body { background: #1a1a1a; color: #eee; }
  .card, .nav-card { background: #2a2a2a; border-color: #444; }
  .nav-card:hover { background: #333; }
  .hero { background: linear-gradient(135deg, #000, #222); }
}
</style>

