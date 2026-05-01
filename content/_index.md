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
        url: uploads/CV.pdf
    design:
      css_class: dark
      background:
        color: black
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
        I apply network and machine learning approaches to understand social systems, including products, science, technology, law, firm, and the country. 
        
        Feel free to reach out for collaboration! 😃

    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: markdown
    id: news
    content:
      title: In the News
      text: |-
        - **Santa Fe Institute** (2025) — *New dataset reveals how US law has grown more complex over the past century.* [Read](https://www.santafe.edu/news-center/news/new-dataset-reveals-how-us-law-has-grown-more-complex-over-the-past-century)
    design:
      columns: '1'
  - block: collection
    id: reviewed-articles
    content:
      title: Reviewed Articles
      text: ""
      filters:
        folders:
          - publication
        publication_type: 'article-journal'
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: reports
    content:
      title: Reports
      text: ""
      filters:
        folders:
          - publication
        publication_type: 'report'
    design:
      view: citation
  - block: collection
    id: reviewed-articles-domestic
    content:
      title: Reviewed Articles (Domestic)
      text: ""
      filters:
        folders:
          - publication
        publication_type: 'article-journal-domestic'
    design:
      view: citation
  - block: collection
    id: under-review
    content:
      title: Manuscripts Under Review
      text: ""
      filters:
        folders:
          - publication
        publication_type: 'preprint'
    design:
      view: citation
  - block: collection
    id: under-review-rr
    content:
      title: Manuscripts in R&R
      text: ""
      filters:
        folders:
          - publication
        publication_type: 'preprint (R&R)'
    design:
      view: citation
# Working Papers section hidden by request — uncomment to restore
#  - block: collection
#    id: working-papers
#    content:
#      title: Working Papers
#      text: ""
#      filters:
#        folders:
#          - publication
#        publication_type: 'manuscript'
#    design:
#      view: citation
  - block: markdown
    id: data-software
    content:
      title: Data & Software
      text: |-
        - **A Century of Evolution in the Complexity of the United States Legal Code** — released with Jeong et al., *Scientific Data* (2026). [DOI](https://doi.org/10.6084/m9.figshare.29540039)
    design:
      columns: '1'
  - block: collection
    id: conference-talks
    content:
      title: Conference Presentations
      filters:
        folders:
          - event
        tag: 'conference'
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: invited-talks
    content:
      title: Invited Talks & Seminars
      filters:
        folders:
          - event
        tag: 'invited'
    design:
      view: article-grid
      columns: 1
---
