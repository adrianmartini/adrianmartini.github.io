---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Welcome
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: featured
    content:
      title: Publications
      filters:
        folders:
          - publication
        featured_only: false
    design:
      columns: '2'
      view: card
  - block: contact
    id: contact
    content:
      email: martini@stats.ox.ac.uk
      address:
        street: Department of Statistics, 24-29 St Giles
        city: Oxford
        postcode: OX1 3LB
        country: United Kingdom
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
    design:
      columns: '2'
---
