---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "3rem"

sections:

  - block: profile_custom
    content:
      username: admin
    
      # The user's folder name in `content/authors/`
      # Show a call-to-action button under your biography? (optional)
      # To link to a file, upload it to your `static/uploads/` folder
      button:
        text: CV
        url: uploads/cv.pdf
      button:
        text: Resume
        url: uploads/resume.pdf
        
  
    design:
      css_class: centering, custom-block
      banner:
        # Upload a cover image to `assets/media/` folder and reference its filename here (optional)
        filename: 'banner.jpg'
      biography:
        # Customize the CSS style of your biography text (optional)
        style: ''
      


  - block: collection_custom
    id: papers
    content:
      
      title: Featured Publications
      text: Diving into innovation—check out my featured publications!
      filters:
        folders:
          - publication
        featured_only: true
      
      button:
        text: view more
        url: publication

    design:
      css_class: custom-block , sombra
      view: article-grid
      columns: 4
      fill_image: false

    
  - block: resume-awards
    content:
      title: -------- Prizes and Awards --------
      text: Celebrating achievements! 🏆 Here are my awards and recognitions.
   
      username: admin
    design:
      css_class: custom-block
      view: community/citation


  - block: collection_custom
    id: projects
    content:
      title: Selected Projects
      text: Crafting solutions. Explore my selected projects!
      filters:
        folders:
          - project
    design:
      css_class: custom-block, sombra
      view: article-grid
      fill_image: false
      columns: 1

---
