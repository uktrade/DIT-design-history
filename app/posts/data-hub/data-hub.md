---
override:tags: []
layout: collection
title: Data Hub
description: An internal tool for seeing a single-view of DIT contact with a company and it's contacts.
pagination:
  data: collections.data-hub
  reverse: true
  size: 50
permalink: "data-hub/{% if pagination.pageNumber > 0 %}page/{{ pagination.pageNumber + 1 }}{% endif %}/"
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    excerpt: "{{ description }}"
    parent: Home
---
