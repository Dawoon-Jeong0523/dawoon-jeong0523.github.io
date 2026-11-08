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
      overview:
        image: /uploads/research/research-overview.webp
        alt: "Dawoon Jeong's career, including Santa Fe Institute visits, alongside product lineages linking papers, patents and devices, rule evolution, and schematic scaling analysis."
        width: 1448
        height: 1086
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
    id: research
    content:
      title: ''
      subtitle: ''
      text: |-
        <h2 class="research-heading">Research</h2>
        <div class="research-themes">
          <article class="research-theme">
            <figure class="research-theme-figure">
              <a class="research-image-link" href="/uploads/research/product-evolution.webp" target="_blank" rel="noopener" aria-label="Open the product evolution illustration at full size">
                <img src="/uploads/research/product-evolution.webp" alt="Branching and recombining mobile-phone and semiconductor lineages, with inherited capabilities represented by colored symbols." width="1536" height="1024" loading="lazy" decoding="async">
              </a>
            </figure>
            <h3>Product evolution and technological capabilities</h3>
            <p>How do new capabilities emerge, persist, and spread? I reconstruct product lineages to study inheritance, recombination, and changes in technical capabilities, with applications to mobile products and semiconductors.</p>
          </article>
          <article class="research-theme">
            <figure class="research-theme-figure">
              <a class="research-image-link" href="/uploads/research/science-technology.webp" target="_blank" rel="noopener" aria-label="Open the science and technology illustration at full size">
                <img src="/uploads/research/science-technology.webp" alt="A knowledge network connecting scientific papers, patent drawings and products, with an atypical connection highlighted by an orange dashed line." width="1536" height="1024" loading="lazy" decoding="async">
              </a>
            </figure>
            <h3>Connections between science and technology</h3>
            <p>I link products, patents, and research papers to examine how technologies draw on scientific knowledge, how atypical research is cited, and whether patterns of knowledge assembly recur across industries.</p>
          </article>
          <article class="research-theme">
            <figure class="research-theme-figure">
              <a class="research-image-link" href="/uploads/research/rule-evolution.webp" target="_blank" rel="noopener" aria-label="Open the rule evolution illustration at full size">
                <img src="/uploads/research/rule-evolution.webp" alt="The U.S. Code and cricket rules alongside changing rule hierarchies and a schematic log-log scaling plot." width="1536" height="1024" loading="lazy" decoding="async">
              </a>
            </figure>
            <h3>Rule evolution and complexity</h3>
            <p>I use historical records and network analysis to study the evolution and complexity of rule systems, including the U.S. Code, sports rules, and regulations.</p>
          </article>
        </div>
        <div class="research-links">
          <a href="/projects/">Explore research projects</a>
          <a href="mailto:jdwoon0523@uchicago.edu">Get in touch</a>
        </div>
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
        - **Santa Fe Institute** (2025) — *New dataset reveals how US law has grown more complex over the past century.* [Read](https://www.santafe.edu/news-center/news/new-dataset-reveals-how-us-law-has-grown-more-complex-over-the-past-century) · **Role:** Co-first author
        - **SBS News** (2024) — *이차전지 인재 수요 7년새 2.5배로 증가…수도권 절반 차지* [Read (Korean)](https://n.news.naver.com/article/055/0001213963) · **Role:** Data analyst
        - **KBS시사** (2023) — *30살 수능, 길을 잃다 [풀영상] | 창 411회 (KBS 23.03.28)* [Watch (Korean)](https://www.youtube.com/watch?v=a4O3L_jZFoE&t=2s) · **Role:** Data analysis
    design:
      columns: '1'
  - block: collection
    id: reviewed-articles
    content:
      title: Peer-Reviewed Publications
      journal_logos:
        - scientific-data
        - scientometrics
        - technovation
        - epj-data-science
        - hssc
        - ieee-tem
        - industrial-corporate-change
        - evolutionary-economics
        - technology-analysis
      text: ""
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
      title: Papers Under Review
      text: ""
      count: 0
      filters:
        folders:
          - publication
        publication_type: 'preprint'
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

        <p class="data-software-description">Explore metrics of scientific and technological evolution, novelty, atypicality, and knowledge structure. <a href="https://dawoon-jeong0523.github.io/SciSci/metrics_dashboard.html">Open dashboard</a></p>

        <a href="https://dawoon-jeong0523.github.io/SciSci/metrics_dashboard.html" target="_blank" rel="noopener"><img src="/uploads/data-software/scisci-dashboard.jpg" alt="First screen of the Science of Science Metrics Dashboard, showing the Metrics Ledger overview and research data summaries." width="1440" height="960" loading="lazy" decoding="async" style="width:100%;height:auto;border:1px solid #e5e7eb;border-radius:12px;"></a>

        <hr class="data-software-divider">

        **Economic Complexity Dashboard**

        <a href="https://dawoon-jeong0523.github.io/EC_dashboard/dashboard.html" target="_blank" rel="noopener"><img src="/uploads/data-software/economic-complexity-dashboard.jpg" alt="First screen of the Economic Complexity Dashboard, showing dataset selectors, country summaries, and ranking charts." width="1440" height="960" loading="lazy" decoding="async" style="width:100%;height:auto;border:1px solid #e5e7eb;border-radius:12px;"></a>

        Explore economic complexity, diversification, product space, and national capabilities. [Open dashboard](https://dawoon-jeong0523.github.io/EC_dashboard/dashboard.html)

        <hr class="data-software-divider">

        **A Century of Evolution in the Complexity of the United States Legal Code**

        <a href="https://doi.org/10.6084/m9.figshare.29540039" target="_blank" rel="noopener"><img src="/uploads/data-software/us-legal-code-dataset.png" alt="Figshare page for the US Legal Code dataset, showing its title, DOI, authors, and description." width="1298" height="856" loading="lazy" decoding="async" style="width:100%;height:auto;border:1px solid #e5e7eb;border-radius:12px;"></a>

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
