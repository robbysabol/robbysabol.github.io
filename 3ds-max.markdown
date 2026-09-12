---
title: 3ds Max Renders
permalink: /3ds-max/
---

<div style="width:66vw; margin: 0 auto 1rem; margin-left: calc(50% - 33vw);">
  <a href="/">← Home</a>
</div>

<div style="font-size: 3.5rem; font-weight: 700; line-height: 1.1; width: 66vw; margin-left: calc(50% - 33vw); margin-right: calc(50% - 33vw);">
  3ds Max Renders
  <span style="display: block; margin-top: -.38rem; font-size: 1.3rem; color: #444b; font-style: italic; font-weight: 400; line-height: 1.3;">
    Interior &amp; exterior renders produced with 3ds Max and Arnold.
  </span>
</div>

<div style="display: grid; width: 66vw; max-width: none; margin-left: calc(50% - 33vw); margin-right: calc(50% - 33vw); margin-top: 3.5rem; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1rem;">

  <div>
    <img src="/assets/images/3ds_Max_Arnold_Dining_Room_Table.png" alt="3ds_max_Arnold_Dining_Room_Table.png" style="width:100%; border-radius:8px;">
    <h3>3ds Max Arnold Dining Room Table</h3>
  </div>

  <div>
    <video controls style="width:100%; border-radius:8px;">
      <source src="/assets/videos/3ds_Max_Arnold_Dining_Room_Table_Orbit.mp4" type="video/mp4">
    </video>
    <h3>3ds Max Arnold Dining Room Table Orbit</h3>
  </div>

<style>
  .container-lg {
    margin-top: 0.5rem !important;
  }

 .container-lg > h1 {
    margin-left: 17vw !important;
  }

  h1:has(> a[href="https://robbysabol.github.io/"]) {
    display: none !important;
  }

  .footer {
    display: none !important;
  }

  img {
    cursor: pointer;
    transition: transform 0.3s ease;
  }
  img:hover {
    transform: scale(1.12);
    z-index: 10;
    position: relative;
  }
  #lightbox {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,10);
    z-index: 999;
    justify-content: center;
    align-items: center;
    cursor: zoom-out;
  }
  #lightbox img {
    max-width: 85%;
    max-height: 85%;
  }

  #lightbox img:hover {
    transform: none;
  }

  .anchorjs-link {
    display: none !important;
  }

  .disabled {
    display: none;
  }
</style>

<div id="lightbox" onclick="this.style.display='none'">
  <img id="lightbox-img">
</div>

<script>
  document.querySelectorAll('img').forEach(img => {
    img.onclick = () => {
      document.getElementById('lightbox-img').src = img.src;
      document.getElementById('lightbox').style.display = 'flex';
    };
  });
</script>
