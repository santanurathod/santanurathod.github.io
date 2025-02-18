---
layout: page
title: Misc.
permalink: /misc/
# image: /assets/img/lobuche.jpg
# caption: Battered legs and dried sweat. Lobuche, Nepal
---

<h2>Times when I felt a sense of calm</h2>
<div class="photo-gallery">
  <img src="/assets/img/1_bikes/photo_1.jpg" alt="Photo 1" data-caption="">
  <img src="/assets/img/1_bikes/photo_2.jpg" alt="Photo 2" data-caption="">
  <img src="/assets/img/1_bikes/photo_3.jpg" alt="Photo 3" data-caption="">
  <img src="/assets/img/1_bikes/photo_4.jpg" alt="Photo 4" data-caption="">
  <img src="/assets/img/1_bikes/photo_5.jpg" alt="Photo 5" data-caption="">
  <!-- Add more images as needed -->
</div>

<h2>Curvy roads of Ha-Giang, Vietnam</h2>
<div class="photo-gallery">
  <img src="/assets/img/2_hagiang/photo_1.jpg" alt="Photo 1" data-caption="">
  <img src="/assets/img/2_hagiang/photo_2.jpg" alt="Photo 2" data-caption="">
  <img src="/assets/img/2_hagiang/photo_3.jpg" alt="Photo 3" data-caption="">
  <img src="/assets/img/2_hagiang/photo_4.jpg" alt="Photo 4" data-caption="">
  <!-- Add more images as needed -->
</div>

<h2>Varanasi, India, a place like no other</h2>
<div class="photo-gallery">
  <img src="/assets/img/3_varanasi/photo_1.jpg" alt="Photo 1" data-caption="">
  <img src="/assets/img/3_varanasi/photo_2.jpg" alt="Photo 2" data-caption="">
  <img src="/assets/img/3_varanasi/photo_3.jpg" alt="Photo 3" data-caption="">
  <img src="/assets/img/3_varanasi/photo_4.jpg" alt="Photo 4" data-caption="">
  <img src="/assets/img/3_varanasi/photo_5.jpg" alt="Photo 5" data-caption="">
  <img src="/assets/img/3_varanasi/photo_6.jpg" alt="Photo 6" data-caption="">
  <img src="/assets/img/3_varanasi/photo_7.jpg" alt="Photo 7" data-caption="">
  <img src="/assets/img/3_varanasi/photo_8.jpg" alt="Photo 8" data-caption="">
  <img src="/assets/img/3_varanasi/photo_9.jpg" alt="Photo 9" data-caption="">
  <img src="/assets/img/3_varanasi/photo_10.jpg" alt="Photo 10" data-caption="">
  <img src="/assets/img/3_varanasi/photo_11.jpg" alt="Photo 11" data-caption="">
  <img src="/assets/img/3_varanasi/photo_12.jpg" alt="Photo 12" data-caption="">
  <img src="/assets/img/3_varanasi/photo_13.jpg" alt="Photo 13" data-caption="">
  <img src="/assets/img/3_varanasi/photo_14.jpg" alt="Photo 14" data-caption="">
  <!-- Add more images as needed -->
</div>



<div id="caption-overlay" class="caption-overlay" style="display: none;">
  <span id="caption-text"></span>
  <button onclick="closeCaption()">Close</button>
</div>

<style>
  .photo-gallery {
    display: flex;
    overflow-x: auto;
    white-space: nowrap;
  }
  .photo-gallery img {
    max-height: 500px; /* Adjust the height as needed */
    margin-right: 10px; /* Space between images */
    cursor: pointer; /* Indicate that the image is clickable */
  }
  .caption-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
</style>

<script>
  document.querySelectorAll('.photo-gallery img').forEach(img => {
    img.addEventListener('click', function() {
      const captionText = this.getAttribute('data-caption');
      document.getElementById('caption-text').innerText = captionText;
      document.getElementById('caption-overlay').style.display = 'flex';
    });
  });

  function closeCaption() {
    document.getElementById('caption-overlay').style.display = 'none';
  }
</script>
