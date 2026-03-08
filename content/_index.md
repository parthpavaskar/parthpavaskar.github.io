---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
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
      text: |-
        I am a final year Ph.D. candidate working in the Theoretical Astro-Particle Physics (THAT) group at the Deutsches Elektronen-Synchrotron (DESY), and the Plasma Astrophysics group at the University of Potsdam.
        
        <div class="bio-buttons-container" style="display: flex; gap: 1rem; flex-wrap: wrap; margin-top: 1rem;">
          <a href="resume" class="inline-flex items-center px-8 py-4 bg-gradient-to-r from-primary-600 to-secondary-600 hover:from-primary-700 hover:to-secondary-700 text-white font-bold text-lg rounded-xl shadow-lg hover:shadow-xl hover:scale-105 transition-all duration-300">
            <svg class='w-5 h-5 mr-3' xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M20.25 14.15v4.25c0 1.094-.787 2.036-1.872 2.18-2.087.277-4.216.42-6.378.42s-4.291-.143-6.378-.42c-1.085-.144-1.872-1.086-1.872-2.18v-4.25m16.5 0a2.18 2.18 0 0 0 .75-1.661V8.706c0-1.081-.768-2.015-1.837-2.175a48.114 48.114 0 0 0-3.413-.387m4.5 8.006c-.194.165-.42.295-.673.38A23.978 23.978 0 0 1 12 15.75c-2.648 0-5.195-.429-7.577-1.22a2.016 2.016 0 0 1-.673-.38m0 0A2.18 2.18 0 0 1 3 12.489V8.706c0-1.081.768-2.015 1.837-2.175a48.111 48.111 0 0 1 3.413-.387m7.5 0V5.25A2.25 2.25 0 0 0 13.5 3h-3a2.25 2.25 0 0 0-2.25 2.25v.894m7.5 0a48.667 48.667 0 0 0-7.5 0M12 12.75h.008v.008H12v-.008Z"/></svg>
            View Short CV
          </a>
          <a href="uploads/pavaskar_cv.pdf" target="_blank" rel="noopener noreferrer" class="inline-flex items-center px-8 py-4 bg-gradient-to-r from-primary-600 to-secondary-600 hover:from-primary-700 hover:to-secondary-700 text-white font-bold text-lg rounded-xl shadow-lg hover:shadow-xl hover:scale-105 transition-all duration-300">
            <svg class='w-5 h-5 mr-3' xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M3 16.5v2.25A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75V16.5M16.5 12 12 16.5m0 0L7.5 12m4.5 4.5V3"/></svg>
            Full CV (.pdf)
          </a>
        </div>
      headings:
        about: 'About me'
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: 'My Research'
      subtitle: ''
      text: |-
        My research primarily focuses on the study of magnetized turbulence in astrophysical plasmas. Plasma turbulence is a highly complex system which is dynamically governed by magneto-hydrodynamics (MHD), and is a fundamental component in broader astrophysical research. It offers insights into phenomena such as cosmic-ray physics, star formation, and more. 

        I investigate plasma turbulence through a combination of theory, state-of-the-art fluid (MHD) and kinetic (PIC) simulations, and analysis of observational data to try and uncover these secrets. I'm also interested in topics such as cosmic-ray acceleration and transport in the ISM.
    design:
      columns: '1'
  - block: collection
    id: feat_research
    content:
      title: Featured Work
      filters:
        folders:
          - research
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    id: recent_papers
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        featured_only: true
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: upcoming_talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - talks
        featured_only: true
    design:
      view: citation
---
