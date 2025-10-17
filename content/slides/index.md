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
  </style>
</head>
<body>
  <h1>나의 취미</h1>
  <div class="slideshow-container">
    <img class="mySlides" src="featured1.jpg" alt="사진1">
    <img class="mySlides" src="featured2.jpg" alt="사진2">
    <img class="mySlides" src="featured3.jpg" alt="사진3">
    <img class="mySlides" src="featured4.jpg" alt="사진4">
  </div>
  <script>
    let slideIndex = 0;
    const slides = document.getElementsByClassName("mySlides");
    function showSlides() {
      for (let i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
      }
      slideIndex++;
      if (slideIndex > slides.length) {slideIndex = 1}
      slides[slideIndex-1].style.display = "block";
      setTimeout(showSlides, 2000);
    }
    window.onload = function() {
      showSlides();
    };
  </script>
</body>
</html>
