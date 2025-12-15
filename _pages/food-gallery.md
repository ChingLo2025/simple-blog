---
layout: single
title: "美食相簿"
permalink: /food/
author_profile: false
classes: wide
---

歡迎光臨我的專屬美食相簿！

{% assign food_photos = site.static_files | where_exp: "file", "file.relative_path contains '/assets/images/'" | sort: 'name' %}

<div class="food-gallery">
  {% for photo in food_photos %}
  <figure class="food-gallery__item">
    <a href="{{ photo.relative_path | relative_url }}">
      <img src="{{ photo.relative_path | relative_url }}" alt="{{ photo.name | split: '.' | first | replace: '-', ' ' | replace: '_', ' ' }}">
    </a>
  </figure>
  {% endfor %}
  <figcaption class="food-gallery__caption">最愛吃的我，必須留下美食紀錄</figcaption>
</div>

{% if food_photos.size == 0 %}
<div class="notice--warning">
  <p>目前還沒有找到美食照片，請將上傳的圖片放到 <code>assets/images/</code>，再生成站點。</p>
</div>
{% endif %}
