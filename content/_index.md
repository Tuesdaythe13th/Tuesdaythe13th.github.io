---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
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

      # Name heading sizing to accommodate long or short names
      name:
        size: balanced # Options: compact (long names), balanced (default), display (short names)

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    id: research
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        My work centers on **AI safety, mechanistic interpretability, and socio-technical risk analysis** across agentic, multimodal, and quantum-adjacent systems. This includes:

        - **Clinical diagnostic frameworks for AI behavioral pathologies**: SCAI risk (Socio-Cognitive Attachment Interference), epistemic coercion, dissociative reasoning — developing a "DSM for AI Systems"
        - **Mechanistic interpretability**: Circuit-level interventions including activation patching, circuit pruning, activation clamping, and engineered discontinuities
        - **Multi-agent systems evaluation**: Taxonomies, agentic maturity frameworks, cascade failures, and failure modes in recommender and multi-agent setups
        - **AI safety & security**: Red teaming, jailbreak analysis, socio-affective benchmarking, post-quantum threat modeling, and security standards
        - **American Emotional Infrastructure (AEI)**: Treating national affect and socio-technical stacks as critical infrastructure with quantum-inspired metrics for stress, trust, and polarization
        - **Digital equity & anti-addiction research**: Aspirational Game Design, digital hygiene, and cybernetics for human agency

        I collaborate with **MLCommons, Humane Intelligence, Open Compute Project, Google programs, academic labs, and public-interest institutions** to develop open benchmarks, security metrics, socio-technical taxonomies, and secure-by-design infrastructure.

        **Please reach out to collaborate on AI safety, evaluation design, or quantum-for-good research.**
    design:
      columns: '1'
  - block: collection
    id: publications
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
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 10
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: markdown
    id: contact
    content:
      title: '📬 Get in Touch'
      subtitle: ''
      text: |-
        **Email**: [tuesday@artifex.fun](mailto:tuesday@artifex.fun)

        **Schedule a Meeting**: [zcal.co/tuesday](https://zcal.co/tuesday)

        **Links**: [Linktree](https://linktr.ee/artifexlabs) | [GitHub](https://github.com/tuesdaythe13th) | [Google Scholar](https://scholar.google.com/citations?user=z71m_nIAAAAJ) | [LinkedIn](https://linkedin.com/in/222tuesday)

        **Locations**: Portland · Los Angeles · New York (remote-first lab)
    design:
      columns: '1'
---
