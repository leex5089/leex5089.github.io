---
layout: archive
permalink: /Data/
title: "Data"
author_profile: true
header:
  image:  "/images/L1007377.jpg"
---

<!-- Section Title -->
<div style="text-align: center; margin-bottom: 20px;">
  <h3 style="font-size: 16px;"> Explore these apps and feel free to test them! </h3>
</div>

<!-- Create 3 Columns Layout -->
<div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 20px; margin-bottom: 30px;">

  <!-- Embedded App 1 -->
  <div class="iframe-container">
    <iframe src="https://wonoctavia-ece.hf.space" frameborder="0" width="100%" height="300" style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;" onclick="expandIframe(this)"></iframe>
  </div>

  <!-- Add Childcare Access Map -->
  <div class="iframe-container">
    <iframe src="/_pages/Map/childcareaccess_map.html" frameborder="0" width="100%" height="300" style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;" onclick="expandIframe(this)"></iframe>
  </div>

  <!-- Add House Map -->
  <div class="iframe-container">
    <iframe src="https://mn-ece-delta-equilibrium.netlify.app/assets/house_map.html" frameborder="0" width="100%" height="300" style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;" onclick="expandIframe(this)"></iframe>
  </div>

</div>

<!-- Video Gallery -->
<div style="display: flex; justify-content: space-between; flex-wrap: wrap; gap: 20px; margin-bottom: 30px;">
  <div class="video-container" onclick="expandVideo(this)">
    <video src="/images/disparity_ratio_mathgap.mp4" width="100%" height="300" autoplay loop style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;"></video>
  </div>

  <div class="video-container" onclick="expandVideo(this)">
    <video src="/images/disparity_ratio_mathgap_hispanic.mp4" width="100%" height="300" autoplay loop style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;"></video>
  </div>

  <div class="video-container" onclick="expandVideo(this)">
    <video src="/images/disparity_ratio_mathgap_asian.mp4" width="100%" height="300" autoplay loop style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;"></video>
  </div>
</div>

<!-- iFrame Gallery -->
<div style="display: flex; flex-direction: column; gap: 20px; justify-content: center; margin-bottom: 30px;">

  <div class="iframe-container">
    <iframe src="/images/agedepen.html" frameborder="0" width="100%" height="300" style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;" onclick="expandIframe(this)"></iframe>
  </div>

  <div class="iframe-container">
    <iframe src="/images/wdi_femalelaborparticipation.html" frameborder="0" width="100%" height="300" style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;" onclick="expandIframe(this)"></iframe>
  </div>

  <div class="iframe-container">
    <iframe src="/images/wdi_mobilphone.html" frameborder="0" width="100%" height="300" style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;" onclick="expandIframe(this)"></iframe>
  </div>

  <div class="iframe-container">
    <iframe src="/images/wdi_electricity.html" frameborder="0" width="100%" height="300" style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;" onclick="expandIframe(this)"></iframe>
  </div>

  <div class="iframe-container">
    <iframe src="/images/wdi_birthrate.html" frameborder="0" width="100%" height="300" style="border-radius: 8px; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1); cursor: pointer;" onclick="expandIframe(this)"></iframe>
  </div>
</div>

<!-- Modal (for expansion) -->
<div id="modal" class="modal" style="display: none;">
  <span class="close" onclick="closeModal()">&times;</span>
  <div id="modal-content" class="modal-content"></div>
</div>

<!-- Add styles for responsiveness and modal -->
<style>
  .iframe-container, .video-container {
    position: relative;
    overflow: hidden;
    border-radius: 8px;
  }

  .iframe-container iframe, .video-container video {
    width: 100%;
    height: 100%;
  }

  /* Modal styles */
  .modal {
    position: fixed;
    z-index: 1;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    overflow: auto;
    display: none;
  }

  .modal-content {
    margin: 15% auto;
    padding: 20px;
    width: 80%;
    max-width: 800px;
    background-color: #fff;
    border-radius: 8px;
  }

  .close {
    color: #aaa;
    float: right;
    font-size: 28px;
    font-weight: bold;
  }

  .close:hover,
  .close:focus {
    color: black;
    text-decoration: none;
    cursor: pointer;
  }
</style>

<!-- Add JavaScript for modal behavior -->
<script>
  function expandIframe(iframe) {
    const modal = document.getElementById('modal');
    const modalContent = document.getElementById('modal-content');
    modalContent.innerHTML = iframe.outerHTML;
    modal.style.display = "block";
  }

  function expandVideo(video) {
    const modal = document.getElementById('modal');
    const modalContent = document.getElementById('modal-content');
    modalContent.innerHTML = video.outerHTML;
    modal.style.display = "block";
  }

  function closeModal() {
    const modal = document.getElementById('modal');
    modal.style.display = "none";
  }
</script>