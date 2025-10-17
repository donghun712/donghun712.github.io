<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>나의 취미</title>
  <style>
    .slideshow-container {
      max-width: 600px;
      height: 350px;
      position: relative;
      margin: auto;
      overflow: hidden;
    }
    .mySlides {
      display: none;
      width: 100%;
      height: 100%;
      object-fit: cover;
      position: absolute;
      top: 0;
      left: 0;
    }
    .slide-btn {
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      background: rgba(0,0,0,0.5);
      color: #fff;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      z-index: 2;
    }
    .prev { left: 10px; }
    .next { right: 10px; }
  </style>
</head>
<body>
  <h1>나의 취미</h1>
  <div class="slideshow-container">
    <button class="slide-btn prev" onclick="plusSlides(-1)">&#10094;</button>
    <button class="slide-btn next" onclick="plusSlides(1)">&#10095;</button>
    <img class="mySlides" src="featured1.jpg" alt="사진1">
    <img class="mySlides" src="featured2.jpg" alt="사진2">
    <img class="mySlides" src="featured3.jpg" alt="사진3">
    <img class="mySlides" src="featured4.jpg" alt="사진4">
  </div>
  <script>
    let slideIndex = 1;
    let timer = null;
    showSlides(slideIndex);
    function plusSlides(n) {
      clearTimeout(timer);
      showSlides(slideIndex += n);
    }
    function showSlides(n) {
      let i;
      let slides = document.getElementsByClassName("mySlides");
      if (n > slides.length) {slideIndex = 1}
      if (n < 1) {slideIndex = slides.length}
      for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
      }
      slides[slideIndex-1].style.display = "block";
      timer = setTimeout(function() { plusSlides(1); }, 2000);
    }
  </script>
</body>
</html>
