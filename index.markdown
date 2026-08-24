# Blender 3D Renders

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 2rem; margin: 2rem 0;">

<h2 style="grid-column: 1 / -1;">Interiors & Exteriors</h2>
  <div>
    <img src="/assets/images/Dining_Table_and_Room.png" alt="Dining_Table_and_Room.png" style="width:100%; border-radius:8px;">
    <h3>Dining Table and Room</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Purple_Bedroom.png" alt="Purple_Bedroom.png" style="width:100%; border-radius:8px;">
    <h3>Purple Bedroom</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Forest_Cave.png" alt="Forest_Cave.png" style="width:100%; border-radius:8px;">
    <h3>Forest Cave</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Santas_Workshop.png" alt="Santas_Workshop.png" style="width:100%; border-radius:8px;">
    <h3>Santas Workshop</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/School_Room.png" alt="School_Room.png" style="width:100%; border-radius:8px;">
    <h3>School Room</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Shelf_Dishes.png" alt="Shelf_Dishes.png" style="width:100%; border-radius:8px;">
    <h3>Shelf Dishes</h3>
   <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Student_Desks.png" alt="Student_Desks.png" style="width:100%; border-radius:8px;">
    <h3>Student Desks</h3>
    <!-- <p>Short description.</p> -->
  </div>

<h2 style="grid-column: 1 / -1;">Characters</h2>

  <div>
    <img src="/assets/images/Reptile_Smooth_Shading_Top_View_Textured.png" alt="Reptile_Smooth_Shading_Top_View_Textured.png" style="width:100%; border-radius:8px;">
    <h3>Reptile Smooth Shading Top View Textured</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Reptile_left_top_side_view_textured.png" alt="Reptile_left_top_side_view_textured.png" style="width:100%; border-radius:8px;">
    <h3>Reptile Left Top Side View Textured</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Reptile_right_top_side_view_textured.png" alt="Reptile_right_top_side_view_textured.png" style="width:100%; border-radius:8px;">
    <h3>Reptile Right Top Side View Textured</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Two_Boys_Textured_Smooth_Shading_Front_View.png" alt="Two_Boys_Textured_Smooth_Shading_Front_View.png" style="width:100%; border-radius:8px;">
    <h3>Two Boys Textured Smooth Shading Front View</h3>
    <!-- <p>Short description.</p> -->
  </div>

  <div>
    <img src="/assets/images/Two_Boys_Textured_Smooth_Shading_T-Pose_Front_View.png" alt="Two_Boys_Textured_Smooth_Shading_T-Pose_Front_View.png" style="width:100%; border-radius:8px;">
    <h3>Two Boys Textured Smooth Shading T-Pose Front View</h3>
    <!-- <p>Short description.</p> -->
  </div>

</div>

---

---

<style>
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
    background: rgba(0,0,0,0.9);
    z-index: 999;
    justify-content: center;
    align-items: center;
    cursor: zoom-out;
  }
  #lightbox img {
    max-width: 75%;
    max-height: 75%;
  }

    .anchorjs-link {
    display: none !important;
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
