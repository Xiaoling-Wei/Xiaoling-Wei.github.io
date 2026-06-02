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
      username: admin
      text: ""
      button:
    design:
      css_class: dark
      background:
        color: black
        image:
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    id: research
    content:
      title: '🔬 My Research'
      subtitle: ''
      text: |-
        I am a PhD student at the **University of Washington** working on **AI security for autonomous systems**. My research investigates adversarial threats against UAVs (drones) — including GPS spoofing, jamming attacks, and anomaly-based intrusion — and develops machine learning-driven countermeasures to improve system resilience.

        Previously at **Texas Tech University**, I applied machine learning and statistical modeling to medical data analysis, building predictive systems to support clinical decision-making for knee disease treatment.

        I am interested in the intersection of **machine learning**, **cybersecurity**, and **autonomous systems**. Feel free to reach out to discuss research or collaboration opportunities.
    design:
      columns: '1'
  - block: collection
    content:
      title: Selected Projects
      text: ''
      filters:
        folders:
          - project
    design:
      view: article-grid
      fill_image: false
      columns: 3
---
