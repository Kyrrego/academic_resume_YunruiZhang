---
# Leave the homepage title empty to use the site title
title:
date: 2023-09-18
type: landing

sections:
  # Delete template block
  # Biography
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  # - block: features
  #   content:
  #     title: Skills
  #     items:
  #       - name: Python
  #         description: 90%
  #         icon: r-project
  #         icon_pack: fab
  #       - name: Statistics
  #         description: 100%
  #         icon: chart-line
  #         icon_pack: fas
  #       - name: Photography
  #         description: 10%
  #         icon: camera-retro
  #         icon_pack: fas


  # Experience
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jul 2023
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Summer Intern
          company: Beckman Institute, University of Illinois at Urbana-Champaign
          company_url: 'https://beckman.illinois.edu/'
          # company_logo: org-gc
          location: Urbana-Champaign, IL, US
          date_start: '2023-07-17'
          date_end: 
          description: |2-
              Responsibilities include:

              * Improving performance of MRSI reconstruction
              * Designing and training deep learning neural networks
              * Volunteering in MRI data acquisition
        - title: Co-organizer, IEEE ICRA24 Workshop
          company: Tsinghua University
          company_url: 'https://www.tsinghua.edu.cn/en/'
          # company_logo: org-x
          location: Beijing, China
          date_start: '2024-05-13'
          date_end: '2024-05-17'
          description: Co-organizer of IEEE ICRA24 Workshop on Intelligent Surgical Robots. 

        - title: Leader, Intelligent Surgical Robot Team
          company: Tsinghua University
          company_url: 'https://www.tsinghua.edu.cn/en/'
          # company_logo: org-x
          location: Beijing, China
          date_start: '2022-10-01'
          date_end: '2023-12-31'
          description: |2-
            * (For the first time) Applied surgical robotics in clinical facial injection-based plastic surgery treatment.
            * Established a 3D multimodal digital facial model for surgical planning.
            * Developed facial 3D spatial navigation control and path planning algorithms for surgical robots, as well as probe localization and pose matching algorithms.

        - title: Research Assistant, Quantum Control and Quantum Computation Lab
          company: Department of Automation, Tsinghua University
          company_url: 'https://scholar.google.com/citations?user=rIaG61EAAAAJ&hl=zh-CN&oi=ao'
          # company_logo: org-x
          location: Beijing, China
          date_start: '2021-11-01'
          date_end: '2022-11-01'
          description: |2-
            * Developed Universal Frame for Quantum Machine Learning based on Quantum Singular Value Transformation. 
            * Explored quantum control landscape problem with topological data analysis method.

    design:
      columns: '2'


  # Accomplishments
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: May 2023
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://cloud.tsinghua.edu.cn/f/07f8871794434bdbb6eb/
          date_end: '2023-05-18'
          date_start: '2022-10-01'
          description: 'First Prize in 2023 Beijing Challenge Cup'
          organization: 
          organization_url: https://bj.tiaozhanbei.net
          title: Intelligent Surgical Robot System
          url: ''
        - certificate_url: https://cloud.tsinghua.edu.cn/f/f26d5a2f28bc4512b075/
          date_end: '2021-10-30'
          date_start: '2021-10-15'
          description: QBronze is QWorld’s introductory level quantum workshop series (16 to 20 hours) on the basics of quantum computing and quantum programming created in October 2018. Successful participants used ProjectQ library to solve real-world quantum computation problems.
          organization: QWorld
          organization_url: https://qworld.net/workshop-bronze/#list
          title: Quantum Computation Programming
          url: https://qworld.net/qbronze69-china-october-2021/

    design:
      columns: '2'


  # Protfolio
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
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false


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
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="life_yr" >}}
    design:
      columns: '1'


  # Collection
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


  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: |-
  #       {{% callout note %}}
  #       Quickly discover relevant content by [filtering publications](./publication/).
  #       {{% /callout %}}
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: true
  #   design:
  #     columns: '2'
  #     view: citation
  # Talks
  
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact
  
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Please feel free to reach out at any time!
      # Contact (add or remove contact options as necessary)
      email: yrzhang0722@gmail.com
      phone: (+86)136 9911 9108
      appointment_url: 'https://yunrui-zhang.netlify.app'
      address:
        street: Zijing Building, Tsinghua University
        city: Beijing
        region: China
        postcode: '100084'
        country: China
        country_code: CN
      directions: 
      office_hours:
        - 'Monday - Sunday 08:00 to 22:00(CST)'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/yrzhang0722'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
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
      columns: '2'
---
