---
override:tags: []
layout: collection
title: Data Workspace
description: The place to discover, access and analyse DIT data.
pagination:
  data: collections.data-workspace
  reverse: true
  size: 50
permalink: "data-workspace/{% if pagination.pageNumber > 0 %}page/{{ pagination.pageNumber + 1 }}{% endif %}/"
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    excerpt: "{{ description }}"
    parent: Home
---
