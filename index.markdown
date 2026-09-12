---
title: Robby Sabol — 3D Art
---

<div style="text-align:center; margin: 3rem auto 4rem; max-width: 66vw;">
  <div style="font-size: 3.2rem; font-weight: 700;">Robby Sabol</div>
  <div style="font-size:1.3rem; color:#444b; font-style: italic; margin-top:.4rem;">
    3D renders, walkthroughs, and character work.
  </div>
</div>

<div style="display:grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap:2rem; width:70vw; max-width:none; margin: 0 auto 4rem;">

  <a href="/blender/" class="preview-card" data-images='["/assets/images/Dining_Table_and_Room.png","/assets/images/Purple_Bedroom.png","/assets/images/Two_Boys_Textured_Smooth_Shading_Front_View.png","/assets/images/Reptile_Smooth_Shading_Top_View_Textured.png"]'>
    <img class="preview-img" src="/assets/images/Dining_Table_and_Room.png" alt="Blender Renders">
    <h2>Blender Renders</h2>
    <p>Interiors, exteriors, and characters.</p>
  </a>

  <a href="/3ds-max/" class="preview-card" data-images='["/assets/images/3ds_Max_Arnold_Dining_Room_Table.jpg"]'>
    <img class="preview-img" src="/assets/images/3ds_Max_Arnold_Dining_Room_Table.jpg" alt="3ds Max Renders">
    <h2>3ds Max Renders</h2>
    <p>Interior &amp; exterior renders, 3ds Max + Arnold.</p>
  </a>

</div>

<style>
  .container-lg {
    margin-top: 0.5rem !important;
  }

  h1:has(> a[href="https://robbysabol.github.io/"]) {
    display: none !important;
  }

  .footer {
    display: none !important;
  }

  .anchorjs-link {
    display: none !important;
  }

  .preview-card {
    display: block;
    text-decoration: none;
    color: inherit;
    border-radius: 10px;
    overflow: hidden;
    transition: transform .25s ease;
  }
  .preview-card:hover {
    transform: translateY(-4px);
  }
  .preview-card img {
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    border-radius: 8px;
    display: block;
  }
  .preview-card h2 {
    margin: .8rem 0 .2rem;
  }
  .preview-card p {
    margin: 0;
    color: #444b;
  }
</style>

<script>
  document.querySelectorAll('.preview-card').forEach(card => {
    const imgs = JSON.parse(card.dataset.images || '[]');
    const imgEl = card.querySelector('.preview-img');
    const original = imgEl.src;
    let interval = null;
    let i = 0;

    if (imgs.length > 1) {
      card.addEventListener('mouseenter', () => {
        interval = setInterval(() => {
          i = (i + 1) % imgs.length;
          imgEl.src = imgs[i];
        }, 900);
      });
      card.addEventListener('mouseleave', () => {
        clearInterval(interval);
        i = 0;
        imgEl.src = original;
      });
    }
  });
</script>
