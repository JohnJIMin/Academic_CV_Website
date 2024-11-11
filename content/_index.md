---
# Leave the homepage title empty to use the site title
title: ""
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
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: white
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I am a multidisciplinary engineer, experienced in the fields of product design, mechanical engineering, robotics, and mechatronics. I am dedicated to developing systems that bridge the gap between innovative research and practical application. My work is centered on designing robotic solutions with robust mechanical, embedded, and control systems that perform reliably in real-world environments. I find purpose in pushing the boundaries of what machines can do autonomously, with a clear focus on how they impact and improve industries and day-to-day life.
    
        With a background in product development and a deep interest in real-world applications, my research aims to integrate robotics seamlessly into complex operational settings, advancing technologies that deliver both performance and adaptability. This work enables me to contribute to the practical evolution of robotics, with an eye toward creating meaningful, scalable solutions for the future.
    
    design:
      columns: '1'

  - block: collection
    id: skills
    content:
      title: Skills
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
    
    - block: collection
      id: papers
      content:
        title: Publications
        filters:
          folders:
            - publication
          featured_only: true
      design:
        view: article-grid
        columns: 2
---
