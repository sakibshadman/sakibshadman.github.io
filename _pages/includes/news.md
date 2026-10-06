# 🔥 News

<!-- News items live in _data/news.yml. This section shows on laptops and phones;
     on wide screens the same items appear in the panel on the right instead. -->
<div class="news-inline">
{% include news-items.html %}
<details class="news-older">
<summary>Older news</summary>
{% include news-items.html older=true %}
</details>
</div>
