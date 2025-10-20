---
# An instance of the Contact widget.
# Documentation: https://docs.hugoblox.com/getting-started/page-builder/
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 40

title: 연락하기
subtitle:

content:
  # Automatically link email and phone or display as text?
  autolink: true

  # Email form provider
  form:
    provider: netlify
    formspree:
      id:
    netlify:
      # Enable CAPTCHA challenge to reduce spam?
      captcha: false

design:
  columns: '1'
---
<div class="text-justify">
  궁금한 사항이 있으시면 아래 양식으로 언제든지 연락주세요. 빠른 시일 내에 답변드리겠습니다.
</div>