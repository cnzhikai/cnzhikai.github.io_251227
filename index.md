---
layout: homepage
---

## About Me

I am a Ph.D. student at ...

## Research Interests

- **Computer Vision:** image recognition, image generation, video captioning
- **Machine Learning:** meta-learning, incremental learning, transfer learning

## News
<ul id="news-list">
  <li class="news-item">**[Feb. 2020]** Our paper about incremental learning is accepted to CVPR 2020.</li>
<li class="news-item">**[Feb. 2020]** Our paper about incremental learning is accepted to CVPR 2020.</li>
<li class="news-item">**[Feb. 2020]** Our paper about incremental learning is accepted to CVPR 2020.</li>

</ul>
<button id="toggle-news">Show More</button>

{% include_relative _includes/publications.md %}

{% include_relative _includes/services.md %}

<style>
.news-item.hidden { display: none; }
</style>
<script>
document.addEventListener('DOMContentLoaded', function(){
  const items = document.querySelectorAll('#news-list .news-item');
  const btn = document.getElementById('toggle-news');
  if (items.length <= 5) {
    btn.style.display = 'none';
    return;
  }
  btn.addEventListener('click', function() {
    items.forEach(i => i.classList.remove('hidden'));
    btn.style.display = 'none';
  });
});
</script>
