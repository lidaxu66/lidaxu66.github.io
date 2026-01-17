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
        text: Download CV 
        url: uploads/resume.pdf

      headings:
        about: ''
        education: ''
        interests: ''
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
      title: '🔬 My Research'
      
      subtitle: ''
      text: |-
        I build photonic integrated circuits (PICs) that utilize the topological properties of light and matter to realize turnkey, robust nonlinear devices with wafer-scale reproducibility.

        - **Topological photonics.** The discoveries of the integer quantum Hall effect (**[1985 Nobel Prize](https://www.nobelprize.org/prizes/physics/1985/summary/)**), the fractional quantum Hall effect (**[1998 Nobel Prize](https://www.nobelprize.org/prizes/physics/1998/summary/)**), and the development of the modern framework of topological phases (**[2016 Nobel Prize](https://www.nobelprize.org/prizes/physics/2016/summary/)**) revealed that topology is not merely a mathematical abstraction, but a fundamental organizing principle of quantum matter. These phases exhibit hallmark properties such as quantized conductance and robust boundary modes that remain protected against disorder and imperfections.

            By translating these concepts into photonics, we design optical structures whose bands inherit the same topological invariants that stabilize electronic edge states. As a result, these systems support topologically protected optical edge modes that guide light along boundaries without backscattering, even in the presence of fabrication imperfections. This robustness enables disorder-immune routing, synthetic gauge fields for photons, and exploration of new regimes in non-Hermitian and nonlinear topological physics.

        - **Microresonator frequency combs.** Optical frequency combs revolutionized precision measurement—a breakthrough recognized by the **[2005 Nobel Prize](https://www.nobelprize.org/prizes/physics/2005/summary/)**—by providing an exquisitely stable ruler for measuring optical frequencies with unprecedented accuracy. Traditional combs, however, rely on large, complex femtosecond laser systems. In the past decade, a major scientific push has aimed to miniaturize this Nobel-Prize–winning capability onto chip-scale platforms. 

          Microresonator frequency combs, or microcombs, achieve this by confining continuous-wave laser light inside a high-Q cavity, where intense circulating fields drive Kerr nonlinearities and generate a series of equally spaced spectral lines. These chip-based combs can operate at microwave repetition rates, produce coherent solitons, and integrate directly with photonic circuits. Their compactness, stability, and CMOS compatibility position microcombs as powerful tools for next-generation precision metrology, telecommunications, and emerging nonlinear and quantum technologies.


    design:
      columns: '1'
      css_class: research-wide
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ''
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
      title: Patents (all equal share)
      text: ""
      filters:
        folders:
          - patents
    design:
      view: citation

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
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
#      title: Recent News
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

