---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
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
        - title: Teaching Assistant for Advanced Geospatial Analysis 
          company: McGill University
          company_url: ''
          company_logo: org-gc
          location: Montreal
          date_start: '2021-01-01'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Designed and led instruction of the laboratory portion of the course
              * Provided feedback and guidance for class research proposal drafts for students projects.
              * Graded assignments and exams, and answered student questions to support the course instructor.
    
        - title: Teaching Assistant for Environmental Research Design Course
          company: McGill University
          company_url: ''
          company_logo: org-x
          location: Montreal
          date_start: '2016-01-01'
          date_end: '2020-12-31'
          description: |2-
              Responsibilities include:

              * Assisted in instruction on research design course, provided feedback and guidance for research proposal drafts for students projects.
              * Graded assignments and exams, and answered student questions to support the course instructor.
    design:
      columns: '2'

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
        - name: Urban Heat Island
          tag: UHI
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Contact 
      
      email: alexander.lam2@mail.mcgill.ca
      address:
        street: 845 Sherbrooke St W
        city: Montreal
        region: QC
        postcode: "H3A 0G4"
        country: Canada
        country_code: CA
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '45.50405466807675'
        longitude: '-73.57525080424266'  
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