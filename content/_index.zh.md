---
# Leave the homepage title empty to use the site title
title: 'Physics'
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '2rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: 查看简历
        url: /uploads/resume_Chinese.pdf

      headings:
        about: '个人简介'
        education: '教育经历'
        interests: '兴趣爱好'
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  



  - block: markdown
    id: research
    content:
      title: '🔬 我的研究方向'
      
      subtitle: ''
      text: |-
        我构建利用光和物质拓扑性质的光子集成电路 (PICs)，以实现具有晶圆级可重复性的即用型、鲁棒非线性器件。

        - **拓扑光子学。** 整数量子霍尔效应 (**[1985年诺贝尔奖](https://www.nobelprize.org/prizes/physics/1985/summary/)**)、分数量子霍尔效应 (**[1998年诺贝尔奖](https://www.nobelprize.org/prizes/physics/1998/summary/)**) 的发现，以及拓扑相现代框架的发展 (**[2016年诺贝尔奖](https://www.nobelprize.org/prizes/physics/2016/summary/)**) 揭示了拓扑不仅仅是数学抽象，而是量子物质的基本组织原则。这些相表现出标志性的性质，如量子化电导和鲁棒的边界模，即使面对无序和缺陷也能保持受保护状态。

            通过将这些概念转化到光子学中，我们设计出的光学结构，其能带继承了稳定电子边缘态的相同拓扑不变量。因此，这些系统支持受拓扑保护的光学边缘模，即使存在制造缺陷，光也能沿着边界传输而无背向散射。这种鲁棒性实现了免受无序影响的路由、光子的合成规范场，以及对非厄米和非线性拓扑物理新领域的探索。

        - **微腔光频梳。** 光学频率梳彻底改变了精密测量——这一突破获得了 **[2005年诺贝尔奖](https://www.nobelprize.org/prizes/physics/2005/summary/)** 的认可——它提供了一把极其稳定的“光尺”，能够以前所未有的精度测量光学频率。然而，传统光梳依赖于庞大且复杂的飞秒激光系统。在过去十年中，科学界的一大主要目标是将这种光尺微型化到芯片级平台上。

            微腔频率梳（或称微梳）通过将连续波激光限制在高 Q 值腔内来实现这一点，腔内强烈的循环场驱动克尔非线性，产生一系列等间距的光谱线。这些片上光梳可以在微波重复频率下工作，产生相干孤子，并能直接与光子电路集成。它们的紧凑性、稳定性和 CMOS 兼容性使微梳成为下一代精密计量、光通信以及新兴非线性与量子技术的有力工具。
      

    design:
      columns: '1'
      css_class: research-wide
  - block: collection
    id: papers
    content:
      title: 精选论文
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: 全部论文
      text: ''
      count: 10
      filters:
        folders:
          - publications
        exclude_featured: false
        exclude_publication_types:
          - "8"
    design:
      view: citation
  - block: collection
    id: patents
    content:
      title: 发明专利 (全为相同贡献)
      text: ""
      filters:
        folders:
          - patents
    design:
      view: citation

  - block: collection
    id: talks
    content:
      title: 近期演讲报告
      filters:
        folders:
          - events
    design:
      view: card
  - block: markdown
    content:
      title: ""
      subtitle: ""
      text: |
        <div style="display: flex; justify-content: center; margin-top: 20px;">
          <a href="https://info.flagcounter.com/AV3Q">
            <img src="https://s01.flagcounter.com/countxl/AV3Q/bg_FFFFFF/txt_000000/border_FFFFFF/columns_2/maxflags_10/viewers_0/labels_1/pageviews_1/flags_0/percent_0/" alt="Flag Counter" border="0">
          </a>
        </div>
    design:
      columns: "1"
#  - block: collection
#    id: news
#    content:
#      title: 新闻事记
#      subtitle: ''
#      text: ''
#      # Page type to display. E.g. post, talk, publication...
#      page_type: blog
#      # Choose how many pages you would like to display (0 = all pages)
#      count: 10
#      # Filter on criteria
#      filters:
#        author: ''
#        category: ''
#        tag: ''
#        exclude_featured: false
#        exclude_future: false
#        exclude_past: false
#        publication_type: ''
#      # Choose how many pages you would like to offset by
#      offset: 0
#      # Page order: descending (desc) or ascending (asc) date.
#      order: desc
#    design:
#      # Choose a layout view
#      view: card
#      # Reduce spacing
#      spacing:
#        padding: [0, 0, 0, 0]
#  - block: cta-card
#    demo: true # Only display this section in the Hugo Blox Builder demo site
#    content:
#      title: 👉 Build your own academic website like this
#      text: |-
#        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.
#
#        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>
#
#       Easily build anything with blocks - no-code required!
#
#        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
#      button:
#        text: Get Started
#        url: https://hugoblox.com/templates/
#    design:
#      card:
#        # Card background color (CSS class)
#        css_class: 'bg-primary-300 dark:bg-primary-700'
#        css_style: ''
---

