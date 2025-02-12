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
        Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

        I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
        
        Please reach out to collaborate 😃
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
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: markdown
    id: teaching
    content:
      title: Teaching
      subtitle: Courses, seminars, and supervision
      text: |-
        | Class | Institution | Term |
        | ----- | ----------- | ---- |
        | [Energy system modeling](https://www.oth-regensburg.de/studieren/zusatzangebot-detailansicht/modellieren-nachhaltiger-energiesysteme-teilnahmebescheinigung) | OTH Regensburg | WiSe24/25 |
        | [Energy system modeling](https://elearning.oth-regensburg.de/course/view.php?id=5641) | OTH Regensburg | SoSe24 |

        ### Open Thesis Projects
        - Master/Bachelor: Analysis and development of concrete financing options for hydrogen projects in countries with both high potential and high risk
        - Master/Bachelor: Development and financing of specific hydrogen supply chains in the Wake of German-African Hydrogen Partnerships
        - Master/Bachelor: Analysis and prerequisites for establishing sustainable hydrogen partnerships between Germany and African countries
        - Master/Bachelor: Technical, economic and regulatory design of potential concrete value chains of African countries with the EU

        ### Ongoing Thesis Projects
        - Master: Scaling up PV Production for domestic use, OTH, 2024
        - Master: Green Hydrogen on the African Continent – Financial demand of large-scale projects, OTH, 2024
        
        ### Past Thesis Projects
        - Bachelor: Charting the Path: Assessing the Potential Opportunities and Pitfalls of Green Hydrogen Production and Export in Africa - An Energy Justice Assessment of the Hyphen Hydrogen Energy Project in Namibia, OTH, 2024
        - Bachelor: The Impact of Green Hydrogen on Employment in South Africa’s Path to a Just Transition. A case study on the South African Hydrogen Valley, OTH, 2024
        - Bachelor: Sustainable Steel Production in the Desert: Economic and Technical Assessment of a Hydrogen-Powered Plant in Mauritania, OTH, 2024
  - block: collection
    id: talks
    content:
      title: Talks
      subtitle: 'Recent & Upcoming Talks - Speaking inquiries: [**anton@achhammer.me**](mailto:anton@achhammer.me)'
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]
  # - block: cta-card
  #   demo: true # Only display this section in the Hugo Blox Builder demo site
  #   content:
  #     title: 👉 Build your own academic website like this
  #     text: |-
  #       This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

  #       <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

  #       Easily build anything with blocks - no-code required!
        
  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/
  #   design:
  #     card:
  #       # Card background color (CSS class)
  #       css_class: "bg-primary-700"
  #       css_style: ""
---