<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>나의 취미</title>
  <style>
    .slideshow-container {
      max-width: 600px;
      position: relative;
      margin: auto;
    }
    .mySlides {
      display: none;
      width: 100%;
      height: 350px;
      object-fit: cover;
    }
  </style>
</head>
<body>
  <div class="slideshow-container">
    <img class="mySlides" src="featured1.jpg" alt="사진1">
    <img class="mySlides" src="featured2.jpg" alt="사진2">
    <img class="mySlides" src="featured3.jpg" alt="사진3">
  </div>
  <script>
    let slideIndex = 0;
    showSlides();
    function showSlides() {
      let slides = document.getElementsByClassName("mySlides");
      for (let i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
      }
      slideIndex++;
      if (slideIndex > slides.length) {slideIndex = 1}
      slides[slideIndex-1].style.display = "block";
      setTimeout(showSlides, 2000); // 2초마다 이미지 변경
    }
  </script>
</body>
</html>
