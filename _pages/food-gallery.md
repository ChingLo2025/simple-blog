---
layout: single
title: "美食相簿"
permalink: /food-gallery/
classes: wide
---

隨手紀錄生活中的美食瞬間，收藏每一次的色香味記憶。

<div class="food-gallery">
  <figure>
    <img src="/assets/images/food/20230930.jpg" alt="2023 年的家常餐點" loading="lazy">
    <figcaption>2023 年 9 月 | 家常餐桌</figcaption>
  </figure>
  <figure>
    <img src="/assets/images/food/20240705.jpg" alt="2024 年的美食紀錄" loading="lazy">
    <figcaption>2024 年 7 月 | 美食日常</figcaption>
  </figure>
</div>

<style>
.food-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1.5rem;
  margin-top: 1rem;
}

.food-gallery figure {
  margin: 0;
}

.food-gallery img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.08);
}

.food-gallery figcaption {
  margin-top: 0.5rem;
  text-align: center;
  font-size: 0.95rem;
  color: #6c7a89;
}
</style>
