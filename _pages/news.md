---
layout: default
title: News and Events
---
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-BZ7FX1WQPT"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-BZ7FX1WQPT');
</script>
{% for post in site.posts %}
{% if post.categories contains 'news' %}
{% include post-grid.html %}
{% endif %}
{% endfor %}