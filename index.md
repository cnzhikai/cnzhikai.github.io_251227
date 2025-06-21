---
layout: homepage
---

## About Me

I am PhD student at <a href="https://ideas.ethz.ch/">Integrated Devices, Electronics, And Systems Group (IDEAS)</a>, under supervison of Prof. Dr. Hua Wang from Swiss Federal Institute of Technology Zürich (ETH Zürich).

I received M.Sc. in Biomedical Engineering from <a href="https://ethz.ch/en.html">ETH Zurich</a> and B.Eng. in Microelectronics from <a href="http://en.xjtu.edu.cn/">Xi'an Jiaotong University</a>. I was a visiting research intern at <a href="https://www.mcgill.ca/">McGill University</a>.

I pursue a vertically integrated strategy, driving innovation from device to circuit to system level, all within a CMOS-centric platform, to tackle key challenges in biomedicine.

## Research Interests

- **Lab on CMOS**
- **Micro-/Nano-Fabrication**
- **CMOS-MEMS Monolitic/Hetergenous Integration and Packaging**  
- **Micro-Robotics** 
- **Machine Learning** 

## News
<ul id="news-list">
  <li class="news-item"> [Oct 2024] I presented my paper on Actuatable Microcage on IEEE BioCAS 2024 in Xi'an China.</li>
</ul><button id="toggle-news">Show More</button>

{% include_relative _includes/publications.md %}
{% include_relative _includes/services.md %}

<style>
.news-item.hidden {
  display: none;
}
#news-list {
  margin-bottom: 0;
  padding-left: 20px; /* match <ul> indent */
}
#toggle-news {
  background: none;
  border: none;
  color: #007acc;
  font-size: 14px;
  cursor: pointer;
  padding: 0;
  margin: 0;
  text-decoration: underline;
  display: inline;
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const items = document.querySelectorAll('#news-list .news-item');
  const btn = document.getElementById('toggle-news');
  let expanded = false;

  // Hide items beyond the 5th
  items.forEach((item, index) => {
    if (index >= 5) item.classList.add('hidden');
  });

  if (items.length <= 5) {
    btn.style.display = 'none';
    return;
  }

  btn.addEventListener('click', function() {
    expanded = !expanded;
    items.forEach((item, index) => {
      if (index >= 5) {
        item.classList.toggle('hidden', !expanded);
      }
    });
    btn.textContent = expanded ? 'Show Less' : 'Show More';
  });
});
</script>
