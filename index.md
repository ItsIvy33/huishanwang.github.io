---
layout: default
title: home

# hello, huishan!

permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
<style>
/* 确保网格布局正确显示 */
.blog-grid {
  display: grid !important;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)) !important;
  gap: 1.5rem !important;
  margin: 2rem 0 !important;
}

.blog-card {
  background: #ffffff !important;
  border-radius: 12px !important;
  overflow: hidden !important;
  box-shadow: 0 2px 12px rgba(1, 47, 99, 0.08) !important;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1) !important;
}

.blog-card:hover {
  transform: translateY(-8px) !important;
  box-shadow: 0 8px 25px rgba(1, 47, 99, 0.15) !important;
}

.blog-card-image {
  position: relative !important;
  width: 100% !important;
  height: 200px !important;
  overflow: hidden !important;
}

.blog-card-image img {
  width: 100% !important;
  height: 100% !important;
  object-fit: cover !important;
  transition: transform 0.3s ease !important;
}

.blog-badge {
  position: absolute !important;
  top: 12px !important;
  left: 12px !important;
  background: linear-gradient(135deg, #FE667B 0%, #ff8599 100%) !important;
  color: white !important;
  padding: 0.4em 0.8em !important;
  border-radius: 20px !important;
  font-size: 0.75em !important;
  font-weight: 600 !important;
  box-shadow: 0 2px 8px rgba(254, 102, 123, 0.3) !important;
  z-index: 10 !important;
}

.blog-card-content {
  padding: 1.2rem !important;
}

.blog-title {
  font-size: 1.1rem !important;
  font-weight: 700 !important;
  color: #012F63 !important;
  margin-bottom: 0.8rem !important;
  line-height: 1.3 !important;
}

.blog-description {
  font-size: 0.9rem !important;
  color: #666 !important;
  line-height: 1.5 !important;
  margin-bottom: 1rem !important;
}

.blog-links {
  display: flex !important;
  gap: 0.6rem !important;
  flex-wrap: wrap !important;
  align-items: flex-end !important;
}

.blog-link {
  display: inline-flex !important;
  align-items: center !important;
  gap: 0.3rem !important;
  padding: 0.4em 0.8em !important;
  background: linear-gradient(135deg, #FE667B 0%, #ff8599 100%) !important;
  color: white !important;
  text-decoration: none !important;
  border-radius: 20px !important;
  font-size: 0.8rem !important;
  font-weight: 500 !important;
  transition: all 0.3s ease !important;
  box-shadow: 0 2px 8px rgba(254, 102, 123, 0.2) !important;
}

.blog-link:hover {
  transform: translateY(-2px) !important;
  box-shadow: 0 4px 12px rgba(254, 102, 123, 0.3) !important;
  color: white !important;
  text-decoration: none !important;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .blog-grid {
    grid-template-columns: 1fr !important;
    gap: 1rem !important;
  }
  
  .blog-card-image {
    height: 180px !important;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .blog-grid {
    grid-template-columns: repeat(2, 1fr) !important;
  }
}

@media (min-width: 1025px) {
  .blog-grid {
    grid-template-columns: repeat(3, 1fr) !important;
  }
}

/* Publications统一设计风格 */
.publication-box {
  display: flex !important;
  background: #ffffff !important;
  border-radius: 12px !important;
  overflow: hidden !important;
  box-shadow: 0 2px 12px rgba(1, 47, 99, 0.08) !important;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1) !important;
  margin: 1.5rem 0 !important;
  align-items: center !important;
  padding-left: 1.5rem !important;
}

.publication-box:hover {
  transform: translateY(-5px) !important;
  box-shadow: 0 8px 25px rgba(1, 47, 99, 0.15) !important;
}

.publication-image {
  position: relative !important;
  width: 280px !important;
  height: 180px !important;
  flex-shrink: 0 !important;
  overflow: hidden !important;
}

.publication-image img {
  width: 100% !important;
  height: 100% !important;
  object-fit: cover !important;
  transition: transform 0.3s ease !important;
}

.publication-image:hover img {
  transform: scale(1.03) !important;
}

.publication-badge {
  position: absolute !important;
  top: 12px !important;
  left: 0px !important;
  background: linear-gradient(135deg, #FE667B 0%, #ff8599 100%) !important;
  color: white !important;
  padding: 0.4em 0.8em !important;
  border-radius: 20px !important;
  font-size: 0.75em !important;
  font-weight: 600 !important;
  box-shadow: 0 2px 8px rgba(254, 102, 123, 0.3) !important;
  z-index: 10 !important;
}

.publication-content {
  flex: 1 !important;
  padding: 1.8rem 1.8rem 1.8rem 0.8rem !important;
  display: flex !important;
  flex-direction: column !important;
  gap: 0.8rem !important;
}

.publication-title {
  font-size: 1.25rem !important;
  font-weight: 700 !important;
  color: #012F63 !important;
  margin: 0 !important;
  line-height: 1.3 !important;
}

.publication-authors {
  font-size: 1rem !important;
  color: #333 !important;
  line-height: 1.4 !important;
}

.publication-venue {
  font-size: 0.95rem !important;
  color: #666 !important;
  font-style: italic !important;
}

.publication-links {
  display: flex !important;
  gap: 0.8rem !important;
  flex-wrap: wrap !important;
  margin-top: 0.5rem !important;
}

.publication-link {
  display: inline-flex !important;
  align-items: center !important;
  gap: 0.4rem !important;
  padding: 0.5em 1em !important;
  background: linear-gradient(135deg, #FE667B 0%, #ff8599 100%) !important;
  color: white !important;
  text-decoration: none !important;
  border-radius: 20px !important;
  font-size: 0.85rem !important;
  font-weight: 500 !important;
  transition: all 0.3s ease !important;
  box-shadow: 0 2px 8px rgba(254, 102, 123, 0.2) !important;
}

.publication-link:hover {
  transform: translateY(-2px) !important;
  box-shadow: 0 4px 12px rgba(254, 102, 123, 0.3) !important;
  color: white !important;
  text-decoration: none !important;
}

.publication-link i {
  font-size: 0.9em !important;
}

/* 响应式设计 - Publications */
@media (max-width: 768px) {
  .publication-box {
    flex-direction: column !important;
    margin: 1rem 0 !important;
  }
  
  .publication-image {
    width: 100% !important;
    height: 160px !important;
  }
  
  .publication-content {
    padding: 1.2rem !important;
    gap: 0.6rem !important;
  }
  
  .publication-title {
    font-size: 1.1rem !important;
  }
  
  .publication-authors,
  .publication-venue {
    font-size: 0.9rem !important;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .publication-image {
    width: 240px !important;
    height: 160px !important;
  }
  
  .publication-content {
    padding: 1.5rem 1.5rem 1.5rem 0.8rem !important;
  }
  
  .publication-title {
    font-size: 1.15rem !important;
  }
}
</style>

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

🐼 Howdy! My name is <span class="accent-text">Huishan Wang</span>, a Ph.D. student at 
<i class="fas fa-university"></i> 
<a href="https://public-health.tamu.edu/" class="link-accent"><strong>Texas A&amp;M University School of Public Health</strong></a>, 
where I am fortunate to be advised by 
<a href="https://shawnchiang.com/" class="link-accent"><strong>Dr. Shawn Chiang</strong></a> 
and co-advised by 
<a href="https://public-health.tamu.edu/directory/ma.html" class="link-accent"><strong>Dr. Ping Ma</strong></a>.
I previously worked as a research assistant at 
<i class="fas fa-hospital-alt"></i> 
<a href="https://ch.shmu.edu.cn/english" class="link-accent"><strong>Children's Hospital of Fudan University</strong></a>, 
gaining valuable experience in public health research. 
Before that, I earned my Master’s degree in Communication from 
<i class="fas fa-university"></i> 
<a href="https://english.pku.edu.cn/" class="link-accent"><strong>Peking University</strong></a>, 
under the mentorship of 
<a href="https://sjc.pku.edu.cn/info/1130/11658.htm" class="link-accent"><strong>Prof. Jing Xu</strong></a>.
Prior to this, I earned my Bachelor’s degree in Food Science and Technology from 
<i class="fas fa-university"></i> 
<a href="https://english.bjfu.edu.cn/" class="link-accent"><strong>Beijing Forestry University</strong></a>.

🎨 Outside of academics, I love <strong> 📝 journaling </strong> and love explopring <strong>🖼 ️ art exhibits</strong>, and <strong> 🐽 wildlife safaris</strong>. I also love watching <strong> 🎤 stand-up comedy</strong> and all kinds of TV shows: my all-time favorite is <strong> 📺 <em>Frasier</em></strong>, and my favorite Japanese anime is <strong><em>🍥 Inuyasha</em></strong>. I’m a big fan of 🎮 gaming too! I enjoy everything from cozy <strong>🎮 Nintendo Switch</strong> games to <strong>⚔️ competitive mobile games</strong>, 🧠 <strong>sudoku</strong>, and so on. If you share any of these interest, feel free to reach out! I am always happy to connect and play together! 

💖 This site is a reflection of my journey, projects, and passions. Thanks for visiting! 💖

<div class="quote-accent">
<span class="primary-gradient-text">She believed she could, so she did.</span>
</div>

🧑‍🎓 My research interests focus on <strong>health communication</strong>, <strong>mental health</strong>, <strong>maternal and adolescent health</strong>, and <strong>the role of social media in shaping health behaviors and perceptions</strong>. I am especially interested in how individuals engage with health information, the role of stigma and acculturation in Asian American communities, and the use of social media to improve health outcomes.

👻 **I am actively seeking research collaboration**. Feel free to reach out, or learn more from <a href="assets/whs_CV_PHD_2025.pdf" class="link-accent">My CV</a>.

<div class="highlight-blocks">

  <div class="highlight-block floating-card">
    <h3><i class="fas fa-microscope"></i> Health Researcher</h3>
    <ul>
      <li>Research focus on <span class="accent-text">Health Communication</span></li>
      <li>Internships at <span class="primary-gradient-text">Top Institutions</span></li>
      <li>Publications at <span class="accent-text">APHA</span></li>
    </ul>
  </div>

  <div class="highlight-block floating-card">
    <h3><i class="fas fa-globe-asia"></i> Life Explorer</h3>
    <ul>
      <li>Visited <span class="accent-text">5 countries worldwide and 20 provinces </span> in China</li>
      <li>Binged more than <span class="accent-text"> 30 TV series and Movies </span> </li>
      <li>Rich experience in <span class="primary-gradient-text">social work</span></li>
    </ul>
  </div>

</div>

<hr>

<h2><i class="fas fa-fire"></i> News</h2>
<ul>
   <li><strong>2025.07</strong>: 🎉🎉 Get started on my fitness journey 💪.</li>
   <li><strong>2025.06</strong>: 🎉🎉 One abstract was accepted by The 2025 Annual APHA Conference. See you in Washington D.C.!</li>
   <li><strong>2024.08</strong>: 🎉🎉 Started my Ph.D. journey in Public Health at Texas A&M University.</li>
</ul>

<hr>

<h2><i class="fas fa-file-alt"></i> Publications</h2>

<div class="publication-box">
  <div class="publication-content">
    <h3 class="publication-title">
      Perceived Social Isolation and Health Information Seeking via Social Media Among Cancer Survivors
    </h3>
    <div class="publication-authors">
      <strong>Huishan Wang</strong>, Shawn Chiang, Ping Ma
    </div>
    <div class="publication-venue">
      In The Annual American Public Health Association Conference 2025
    </div>
  </div>
</div>

<div class="publication-box">
  <div class="publication-content">
    <h3 class="publication-title">
      Nativity Differences in Awareness and Knowledge About HPV Infection and Vaccination Among Foreign- and US-Born Asians: Findings from a National Population-Based Sample
    </h3>
    <div class="publication-authors">
      Shawn Chiang, <strong>Huishan Wang</strong>, MS Sifat, Ping Ma
    </div>
    <div class="publication-venue">
      In the American Society of Preventive Oncology Annual Conference 2024
    </div>
  </div>
</div>


<hr>

<h2><i class="fas fa-graduation-cap"></i> Education</h2>
<ul>
  <li><strong>2024.08 - Present</strong>: Doctor of Philosophy, Health Education, <span class="primary-gradient-text">Texas A&M University</span></li>
  <li><strong>2019.09 - 2021.07</strong>: Master of Journalism and Communication, Health Communication, <span class="primary-gradient-text">Peking University</span></li>
  <li><strong>2015.09 - 2019.07</strong>: Bachelor of Engineering, Food Science and Technology, <span class="primary-gradient-text">Beijing Forestry University</span></li>
</ul>

<hr>

<h2><i class="fas fa-laptop-code"></i> Professional Experience</h2>
<ul>
  <li><strong>2024.04 - 2024.07</strong>: Research Intern, <a href="https://hcdata.nju.edu.cn/" class="link-accent">Digital Medical Group</a>, <strong>Nanjing University</strong></li>
  <li><strong>2021.07 - 2023.09</strong>: Research Assistant, Center for Clinical Guidelines Production and Evaluation, GRADE Center of Fudan University, <strong>Children's Hospital of Fudan University</strong></li>
  <li><strong>2020.12 - 2021.02</strong>: Management Training Intern, Outpatient Department & Communication Department, <strong>Peking Union Medical College Hospital</strong></li>
</ul>

