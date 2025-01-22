---
name: Custom issue template
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

name: Project Update
description: Track project progress
title: "[PROJECT] "
labels: ["tracking"]
body:
  - type: input
    id: project-name
    attributes:
      label: Project Name
      required: true
  
  - type: dropdown
    id: status
    attributes:
      label: Current Status
      options:
        - Not Started
        - In Progress
        - Complete
      required: true
  
  - type: input
    id: progress
    attributes:
      label: Progress (%)
      description: Current completion percentage
  
  - type: textarea
    id: updates
    attributes:
      label: Recent Updates
