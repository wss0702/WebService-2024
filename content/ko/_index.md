---
# Leave the homepage title empty to use the site title
title: "WooSangSoo Web"
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"


sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: 재학증명서 다운로드
        url: uploads/registration.pdf
    design:
      css_class: dark
      background:
        color: green
        image:
          # Add your image background to `assets/media/`.
          filename: background.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: collection
    id: skills
    content:
      title: 기술
      filters:
        folders:
          - skills
        featured_only: true
    design:
      view: article-grid
      columns: 3

  - block: collection
    id: projects
    content:
      title: 프로젝트
      text: ''
      page_type: projects
      count: 5
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      offset: 0
      # 최근 프로젝트가 먼저 나오게 끔
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [1, 1, 1, 1]
  - block: collection
    id: hobbies
    content:
      title: 취미
      filters:
        folders:
          - hobbies
        featured_only: true
    design:
      view: article-grid
      columns: 3
  - block: slider
    design:
      slide_height: "300px" # 슬라이드의 높이 설정
      is_fullscreen: false  # 슬라이드가 전체 화면을 차지할지 여부
    content:
      title: 관심분야
      slides:
        - title: "DB"
        - title: "Front end"
        - title: "back end"
       
---
