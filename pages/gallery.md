---
permalink: /gallery
title: NIH Tech
layout: gallery
---
<div class="container">
<h3>Transformation & Excellence Center for Health (TECH).</h3>
<p>Transformation & Excellence Center for Health (TECH) has been functioning as a significant component of the National Institute of Health.</p>
</div>
<div class="row m-0">
  <div class="col-md-4 mt-4">
    <img src="/assets/images/aboutus.png" style="width:100%; height:220px; border-radius:20px;" onclick="openModal();currentSlide(1)" class="hover-shadow cursor">
  </div>
  <div class="col-md-4 mt-4">
    <img src="/assets/images/aboutus.png" style="width:100% ; height:220px; border-radius:20px;" onclick="openModal();currentSlide(2)" class="hover-shadow cursor">
  </div>
  <div class="col-md-4 mt-4">
    <img src="/assets/images/aboutus.png" style="width:100%; height:220px; border-radius:20px;" onclick="openModal();currentSlide(3)" class="hover-shadow cursor">
  </div>
  <div class="col-md-4 mt-4">
    <img src="/assets/images/aboutus.png" style="width:100%; height:220px; border-radius:20px;" onclick="openModal();currentSlide(4)" class="hover-shadow cursor">
  </div>
   <div class="col-md-4 mt-4">
    <img src="/assets/images/aboutus.png" style="width:100%; height:220px; border-radius:20px;" onclick="openModal();currentSlide(4)" class="hover-shadow cursor">
  </div>
</div>

<div id="myModal" class="modal">
  <span class="close cursor" onclick="closeModal()">&times;</span>
  <div class="modal-content">

    <div class="mySlides">
      <div class="numbertext">1 / 4</div>
      <img src="/assets/images/site-logo.jpg" style="width:100%; height:300px">
      <p class="centered">NIH has been continuously contributing to the health sector of Pakistan and since the development of NIH is working on the production of vaccines, research and development and other training ventures. Recently, NIH has established a Transformation and Excellence Center for Health (TECH) in order to provide tech services to the public. TECH is defined by the simple set of corporate values which shows  how we are operating every single day through technology for the betterment of the health of society. Our main objective is to ensure that our healthcare objectives are achieved with the highest level of assurance and capability.
</p>
    </div>

    <div class="mySlides">
      <div class="numbertext">2 / 4</div>
      <img src="/assets/images/aboutus.png" style="width:100%; height:300px">
    </div>

    <div class="mySlides">
      <div class="numbertext">3 / 4</div>
      <img src="/assets/images/site-logo.jpg" style="width:100%; height:300px">
    </div>
    
    <div class="mySlides">
      <div class="numbertext">4 / 4</div>
      <img src="/assets/images/aboutus.png" style="width:100%; height:300px">
    </div>
    
    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>

    <div class="caption-container" style="display:none">
      <p id="caption"></p>
    </div>


    <div class="column">
      <img class="demo cursor" src="" style="display:none;" onclick="currentSlide(1)" alt="">
    </div>
    <div class="column">
      <img class="demo cursor" src="" style="display:none;" onclick="currentSlide(2)" alt="">
    </div>
    <div class="column">
      <img class="demo cursor" src="" style="display:none;" onclick="currentSlide(3)" alt="">
    </div>
    <div class="column">
      <img class="demo cursor" src="" style="display:none;" onclick="currentSlide(4)" alt="">
    </div>
  </div>
</div>



<script>
function openModal() {
  document.getElementById("myModal").style.display = "block";
}

function closeModal() {
  document.getElementById("myModal").style.display = "none";
}

var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("demo");
  var captionText = document.getElementById("caption");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
  captionText.innerHTML = dots[slideIndex-1].alt;
}
</script>