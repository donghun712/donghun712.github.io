---
title: "나의 취미"
widget: slider
headless: true             # 래퍼 숨김
weight: 3
design:
  slide_height: "350px"
  loop: true
  interval: 3000

# page bundle 내 이미지 리소스 사용
resources:
  - src: "arrow.jpg"
    name: "slide1"
  - src: "game.jpg"
    name: "slide2"
  - src: "cook.jpg"
    name: "slide3"

content:
  slides:
    - title: "국궁"
      background:
        media: "slide1"
        position: center
        fit: cover
        brightness: 0.7
    - title: "게임"
      background:
        media: "slide2"
        position: center
        fit: cover
        brightness: 0.7
    - title: "요리"
      background:
        media: "slide3"
        position: center
        fit: cover
        brightness: 0.7
---
