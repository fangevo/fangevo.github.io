---
permalink: /photos/
layout: splash
---

<div class="photo-gallery">
  {% for photo in site.data.photos %}
  <div class="photo-item">
    <a href="{{ photo.image }}" data-lightbox="gallery">
      <img src="{{ photo.image }}" alt="{{ photo.caption }}">
    </a>
    <p>{{ photo.caption }}</p>
  </div>
  {% endfor %}
</div>