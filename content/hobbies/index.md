---
title: "나의 취미"
widget: slider
headless: true
weight: 40

header:
  text: "## 나의 취미"   # 제목 출력용

design:
  slide_height: "350px"
  loop: true
  interval: 3000

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
