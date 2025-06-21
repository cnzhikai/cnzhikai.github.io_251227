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
  <li class="news-item">**[Jan. 2020]** We will host the ACM Multimedia Asia 2020 conference in Singapore!</li>
  <li class="news-item">**[Dec. 2019]** Our paper about few-shot learning is accepted to NeurIPS 2019.</li>
  <li class="news-item">**[Nov. 2019]** We released new code for meta-learning.</li>
  <li class="news-item">**[Oct. 2019]** Gave a talk at CVPR Workshop on Incremental Learning.</li>
  <li class="news-item">**[Sept. 2019]** Paper accepted to ICCV 2019.</li>
  <li class="news-item">**[Aug. 2019]** Released new dataset on few-shot classification.</li>
</ul>
<button id="toggle-news">Show More</button>

{% include_relative _includes/publications.md %}
{% include_relative _includes/services.md %}

<style>
.news-item.hidden {
  display: none;
}
#toggle-news {
  margin-top: 10px;
  padding: 6px 12px;
  font-size: 14px;
  cursor: pointer;
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function(){
  const items = document.querySelectorAll('#news-list .news-item');
  const btn = document.getElementById('toggle-news');

  // Automatically hide items beyond the 5th
  items.forEach((item, index) => {
    if (index >= 5) item.classList.add('hidden');
  });

  // Hide button if 5 or fewer items
  if (items.length <= 5) {
    btn.style.display = 'none';
    return;
  }

  btn.addEventListener('click', function() {
    items.forEach(item => item.classList.remove('hidden'));
    btn.style.display = 'none';
  });
});
</script>
