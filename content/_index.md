---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing
widget: hero


design:
  # Default section spacing
  spacing: "5rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/CV_LuisPerez.pdf

    design:
      css_class: dark
      background:
        color: white
        image:
          # Add your image background to `assets/media/`.
          filename: SMU_color.png
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
      spacing: 
        padding: ["20px", "0", "30px", "0"]
      
  - block: markdown
    content:
      title: 'Research Profile'
      subtitle: ''
      text: "**I am a macroeconomist interested in Market Power, Aggregate Productivity, and Public Finance**. 
      
      My work seeks to advance three research agendas:
      
        - The first quantifies different sources of market power—monopoly and monopsony—and their impact on the macroeconomy. 
      
        - The second addresses the question, Why are some countries more productive than others? 
      
        - The third is concerned with policy and works toward detecting market failures in different aspects of economic life to propose optimal interventions. 
        
    
  To learn more, please read my research statement <https://luiscanyamel.github.io/website_materials/Research_Statement_LuisPerez.pdf>."


    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Research
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Working papers & publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
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

---
