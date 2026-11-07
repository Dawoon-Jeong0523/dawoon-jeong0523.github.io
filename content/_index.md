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
      title: 'Research'
      subtitle: ''
      text: |-
        **Product evolution and technological capabilities**

        How do new capabilities emerge, persist, and spread? I reconstruct product lineages to study inheritance, recombination, and changes in technical capabilities, with applications to mobile products and semiconductors.

        **Connections between science and technology**

        I link products, patents, and research papers to examine how technologies draw on scientific knowledge, how atypical research is cited, and whether patterns of knowledge assembly recur across industries.

        **Institutional evolution and complexity**

        I use historical records and network analysis to study the evolution of laws and regulatory systems, including the United States Legal Code and the Laws of Cricket.

        [Explore research projects](/projects/) · [Get in touch](mailto:jdwoon0523@uchicago.edu)

    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      count: 4
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
      title: Peer-Reviewed Publications
      text: "Published and accepted articles. Author contribution notes are available on each paper's page."
      count: 0
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
      count: 0
      filters:
        folders:
          - publication
        publication_type: 'report'
    design:
      view: citation
  - block: collection
    id: reviewed-articles-domestic
    content:
      title: Peer-Reviewed Publications (Domestic)
      text: ""
      count: 0
      filters:
        folders:
          - publication
        publication_type: 'article-journal-domestic'
    design:
      view: citation
  - block: collection
    id: under-review
    content:
      title: Submitted & Under Review
      text: ""
      count: 0
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
      count: 0
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
        **Science of Science Metrics Dashboard**

        Explore metrics of scientific and technological evolution, novelty, atypicality, and knowledge structure. [Open dashboard](https://dawoon-jeong0523.github.io/SciSci/metrics_dashboard.html)

        **Economic Complexity Dashboard**

        Explore economic complexity, diversification, product space, and national capabilities. [Open dashboard](https://dawoon-jeong0523.github.io/EC_dashboard/dashboard.html)

        **A Century of Evolution in the Complexity of the United States Legal Code**

        A historical dataset for studying the changing complexity of US law, released with Jeong et al., *Scientific Data* (2026). [View dataset](https://doi.org/10.6084/m9.figshare.29540039) · [Read paper](https://doi.org/10.1038/s41597-025-06313-w)
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
