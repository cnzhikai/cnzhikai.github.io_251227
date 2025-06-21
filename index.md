---
layout: homepage
---

## About Me

I am a Ph.D. student at ...

## Research Interests

- **Computer Vision:** image recognition, image generation, video captioning
- **Machine Learning:** meta-learning, incremental learning, transfer learning

## News

- **[Feb. 2020]** Our paper about incremental learning is accepted to CVPR 2020.
- **[Feb. 2020]** We will host the ACM Multimedia Asia 2020 conference in Singapore!
- **[Sept. 2019]** Our paper about few-shot learning is accepted to NeurIPS 2019.
- **[Mar. 2019]** Our paper about few-shot learning is accepted to CVPR 2019.
- **[Feb. 2020]** Our paper about incremental learning is accepted to CVPR 2020.
- **[Feb. 2020]** We will host the ACM Multimedia Asia 2020 conference in Singapore!
- **[Sept. 2019]** Our paper about few-shot learning is accepted to NeurIPS 2019.
- **[Mar. 2019]** Our paper about few-shot learning is accepted to CVPR 2019.

{% include_relative _includes/publications.md %}

{% include_relative _includes/services.md %}

<style>
.news-item.hidden { display: none; }
</style>
<script>
document.addEventListener('DOMContentLoaded', function(){
  const items = document.querySelectorAll('#news-list .news-item');
  const btn = document.getElementById('toggle-news');
  btn.addEventListener('click', function() {
    items.forEach(i => i.classList.remove('hidden'));
    btn.style.display = 'none';
  });
});
</script>
