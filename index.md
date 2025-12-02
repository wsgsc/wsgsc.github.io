---
layout: default
title: 马斯克铁粉站
---


## 🔥 四大栏目快速导航

- 📝 **[大作文](/long/)**：关于马斯克的长篇深度文章  
- 💬 **[马斯克名言](/quotes/)**：令人深思的经典语录  
- 🐦 **[X言X语](/tweets/)**：马斯克在 X 上的发言整理  
- 😎 **[马斯克八卦](/gossip/)**：轻松有趣的马斯克故事  

---

## 📰 最新文章  
{% for post in site.posts limit:8 %}
- [{{ post.title }}]({{ post.url }})  
  <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}


<p>
本站总访问量：<span id="busuanzi_value_site_pv">加载中...</span> 次  
<br>
本站访客数：<span id="busuanzi_value_site_uv">加载中...</span> 人  
</p>

