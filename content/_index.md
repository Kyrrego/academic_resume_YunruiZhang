---
# Leave the homepage title empty to use the site title
title:
date: 2023-09-18
commentable: true # enable Giscus comments
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

  # Featured Publications
  - block: collection
    id: featured
    content:
      title: Publications & Patents
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card


  # Experience
  - block: experience
    id: experience
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
        - title: Summer Research Internship
          company: Beckman Institute, University of Illinois at Urbana-Champaign
          company_url: 'https://beckman.illinois.edu/'
          # company_logo: org-gc
          location: Urbana-Champaign, IL, US
          date_start: '2023-07-17'
          date_end: '2023-09-12'
          description: |2-
              * Proposed a self-supervised learning-based (k,t)-space interpolation method, (k,t)-RAKI, that is useful for further accelerating MRSI acquisition, in combination with subspace methods.
              * Devised specialized convolutional kernels and a complex convolutional neural network architecture to enhance both the efficiency of training and the quality of reconstruction.
              * Effectively reconstructed data for different undersampling designs in in vivo brain MRSI, leading to improved subsequent spatiospectral processing results.
  
        - title: Co-organizer, IEEE ICRA24 Workshop
          company: Tsinghua University
          company_url: 'https://www.tsinghua.edu.cn/en/'
          # company_logo: org-x
          location: Beijing, China
          date_start: '2024-05-13'
          date_end: '2024-05-17'
          description: |1-
            Co-organizer of IEEE ICRA24 (International Conference on Robotics and Automation) Workshop on Intelligent Surgical Robots. 

            * Co-organizers: Prof. Xiao Long (Peking Union Medical College Hospital), Prof. Gangtie Zheng (Tsinghua University) , Prof. Richard M. Voyles (Purdue University)

        - title: Leader, Intelligent Surgical Robot Team
          company: Tsinghua University
          company_url: 'https://www.tsinghua.edu.cn/en/'
          # company_logo: org-x
          location: Beijing, China
          date_start: '2022-10-01'
          date_end: 
          description: |2-
            * Pioneered the utilization of surgical robotics in clinical facial injection-based plastic surgery treatments.
            * Innovated the creation of a comprehensive 3D multi-modal deep digital facial model for precise surgical planning.
            * Engineered advanced facial 3D spatial navigation control and path planning algorithms specifically tailored for surgical robots, alongside cutting-edge probe localization and pose matching algorithms.

        - title: Research Assistant, Quantum Control and Quantum Computation Lab
          company: Department of Automation, Tsinghua University
          company_url: 'https://scholar.google.com/citations?user=rIaG61EAAAAJ&hl=zh-CN&oi=ao'
          # company_logo: org-x
          location: Beijing, China
          date_start: '2021-11-01'
          date_end: '2022-11-01'
          description: |2-
            * Conceived and conducted the design and simulation of quantum circuits tailored for the integration of nonlinear activation functions within quantum neural networks, leveraging the Quantum Singular Value Transformation paradigm.
            * Pioneered the application of topological data analysis methodology to provide empirical evidence that, during the traversal process, the quantum control landscape remains unburdened by the challenge of becoming ensnared in local optima.

    design:
      columns: '2'

  # 10/09: Deleted this block because it can be merged with "Projects"
  # # Accomplishments
  # - block: accomplishments
  #   content:
  #     # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
  #     title: 'Accomplish&shy;ments'
  #     subtitle:
  #     # Date format: https://wowchemy.com/docs/customization/#date-format
  #     date_format: May 2023
  #     # Accomplishments.
  #     #   Add/remove as many `item` blocks below as you like.
  #     #   `title`, `organization`, and `date_start` are the required parameters.
  #     #   Leave other parameters empty if not required.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - certificate_url: https://cloud.tsinghua.edu.cn/f/07f8871794434bdbb6eb/
  #         date_end: '2023-05-18'
  #         date_start: '2022-10-01'
  #         description: 'First Prize in 2023 Beijing Challenge Cup'
  #         organization: 
  #         organization_url: https://bj.tiaozhanbei.net
  #         title: Intelligent Surgical Robot System
  #         url: ''
  #       - certificate_url: https://cloud.tsinghua.edu.cn/f/f26d5a2f28bc4512b075/
  #         date_end: '2021-10-30'
  #         date_start: '2021-10-15'
  #         description: QBronze is QWorld’s introductory level quantum workshop series (16 to 20 hours) on the basics of quantum computing and quantum programming created in October 2018. Successful participants used ProjectQ library to solve real-world quantum computation problems.
  #         organization: QWorld
  #         organization_url: https://qworld.net/workshop-bronze/#list
  #         title: Quantum Computation Programming
  #         url: https://qworld.net/qbronze69-china-october-2021/

  #   design:
  #     columns: '2' 

  # Portfolio
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
        - name: Biomedical Imaging
          tag: Biomedical Imaging
        - name: Robotics
          tag: Robotics
        - name: Quantum Computation
          tag: Quantum Computation
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false


  - block: markdown
    id: gallery
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
        Please feel free to reach out at any time! The best way to reach me would be via email or WeChat.
      # Contact (add or remove contact options as necessary)
      email: yrzhang0722@gmail.com
      phone: (+86) 136 9911 9108
      appointment_url: 'https://yunrui-zhang.me'
      address:
        street: Tsinghua University
        city: Beijing
        region: China
        postcode: '100084'
        country: China
        country_code: CN
      # directions: 
      # office_hours:
      #   - 'Monday - Sunday 08:00 to 22:00(CST)'
      contact_links:
        - icon: weixin
          icon_pack: fab
          name: DM Me via [WeChat](https://yunrui-zhang.me/authors/admin/wechat_QR.jpg)
          link: 'null'
        - icon: camera-retro
          icon_pack: fas
          name: Avatar image taken by [Jida](https://giddazhang.github.io) on 09/10/2023 :)
          link: 'null'
        # - icon: video
        #   icon_pack: fas
        #   name: Zoom Me
        #   link: 'https://zoom.com'
        # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
---
