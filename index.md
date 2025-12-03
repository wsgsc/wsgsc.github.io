---
layout: default
title: 马斯克铁粉站
---

<!-- 必读推荐 -->
<section>
  <h2>⭐ 必读推荐</h2>
  <div class="card">
    <div class="card-icon">📘</div>
    <div class="card-content">
      <a class="card-title" href="/long/2025/11/30/elon-musk-intro.html">
        埃隆·马斯克：改变世界的工程狂人
      </a>
      <p class="card-desc">一文读懂马斯克的成长、工程思维与公司体系。</p>
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
      <p>深度解析马斯克现象及思想</p>
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
    {% for post in site.posts limit:8 %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <small>{{ post.date | date: "%Y-%m-%d" }}</small>
      </li>
    {% endfor %}
  </ul>
</section>

<!-- 全部文章 -->
<section>
  <h2>🗂 全部文章</h2>
  <ul class="latest-list">
    {% for post in site.posts %}
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


/* 全局颜色变量 */
:root {
  --bg: #ffffff;
  --text: #000000;
  --card-bg: #f5f5f5;
  --nav-solid: rgba(255,255,255,0.9);
}
body.dark {
  --bg: #1a1a1a;
  --text: #eeeeee;
  --card-bg: #2a2a2a;
  --nav-solid: rgba(0,0,0,0.85);
}

body {
  background: var(--bg);
  color: var(--text);
  transition: 0.25s ease;
}

/* 必读推荐卡片 */
.card {
  display: flex;
  gap: 16px;
  padding: 20px;
  border-radius: 16px;
  background: var(--card-bg);
  border: 1px solid #ddd;
  transition: 0.25s;
}
body.dark .card {
  border-color: #444;
}

/* 栏目导航 Grid */
.nav-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 20px;
}
.nav-card {
  background: var(--card-bg);
  text-decoration: none;
  padding: 20px;
  border-radius: 16px;
  border: 1px solid #ddd;
  transition: 0.25s;
  color: inherit;
}
.nav-card:hover {
  transform: translateY(-3px);
  background: rgba(0,0,0,0.05);
}
body.dark .nav-card {
  border-color: #444;
}
body.dark .nav-card:hover {
  background: rgba(255,255,255,0.08);
}

/* 最新文章列表 */
.latest-list {
  list-style: none;
  padding: 0;
}
.latest-list li {
  margin: 10px 0;
}

/* 数据排版 */
.stats {
  margin-top: 40px;
  text-align: center;
  color: #666;
}
</style>

<!-- Busuanzi 访客统计（直接放在首页可确保生效） -->
<script async src="https://cdn.jsdelivr.net/gh/pg7go/busuanzi/bsz.pure.mini.js"></script>


