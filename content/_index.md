---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: hero
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: Hugo Academic Theme
      image:
        filename: hero-academic.png
      cta:
        label: '**Get Started**'
        url: https://hugoblox.com/templates/
      cta_alt:
        label: Ask a question
        url: https://discord.gg/z8wNYzb
      cta_note:
        label: >-
          <div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Hugo Blox Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/theme-academic-cv" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
      text: |-
        **Generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 500,000+ sites.**

        **Easily build anything with blocks - no-code required!**

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Accelerator Physicist
          company: ANSTO - the Australian Synchrotron
          company_url: ''
          company_logo: ansto-logo
          location: Melbourne, Australia
          date_start: '2023-10-01'
          date_end: ''
          description: #|2-
           #   Responsibilities include:

#              * Analysing
 #             * Modelling
  #            * Deploying
        - title: Lecturer
          company: University of Liverpool / Cockcroft Institute
          company_url: ''
          company_logo: UoL-Logo
          location: Liverpool, UK
          date_start: '2020-09-01'
          date_end: '2023-09-01'
          description: Established research agenda and taught 2nd year electromagnetics.
        - title: Postdoc fellow
          company: CERN
          company_url: ''
          company_logo: CERN_logo
          location: Geneva, Switzerland
          date_start: '2017-06-01'
          date_end: '2020-09-01'
          description: Developed optics correction scheme for the e+/e- Future Circular Collider (FCC-ee).
    design:
      columns: '2'
#  - block: accomplishments
#    content:
#      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
#      title: 'Accomplish&shy;ments'
#      subtitle:
#      # Date format: https://docs.hugoblox.com/customization/#date-format
#      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
 #     items:
 #       - certificate_url: https://www.coursera.org
 #         date_end: ''
 #         date_start: '2021-01-25'
 #         description: ''
 #         icon: coursera
 #         organization: Coursera
 #         organization_url: https://www.coursera.org
 #         title: Neural Networks and Deep Learning
 #         url: ''
 #       - certificate_url: https://www.edx.org
 #         date_end: ''
 #         date_start: '2021-01-01'
 #         description: Formulated informed blockchain models, hypotheses, and use cases.
 #         icon: edx
 #         organization: edX
 #         organization_url: https://www.edx.org
 #         title: Blockchain Fundamentals
 #         url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
 #       - certificate_url: https://www.datacamp.com
 #         date_end: '2020-12-21'
 #         date_start: '2020-07-01'
 #         description: ''
 #         icon: datacamp
 #         organization: DataCamp
 #         organization_url: https://www.datacamp.com
 #         title: 'Object-Oriented Programming in R'
 #         url: ''
 #   design:
 #     columns: '2'
 # - block: collection
 #   id: posts
 #   content:
 #     title: Recent Posts
 #     subtitle: ''
 #     text: ''
 #     # Choose how many pages you would like to display (0 = all pages)
 #     count: 5
 #     # Filter on criteria
 #     filters:
 #       folders:
 #         - post
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
 #     view: compact
 #     columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Rings
          tag: Rings
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: collection
    id: news
    content:
      title: Recent News
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
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---