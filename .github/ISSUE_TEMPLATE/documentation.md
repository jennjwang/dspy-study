---
name: Documentation
about: Link to any documentation or examples that you are referencing.
title: ''
labels: documentation
assignees: ''

---

name: 📝 Documentation Update
description: Suggest an improvement, addition, or fix to the documentation.
title: "[Docs]: "
labels: [documentation]
assignees: []
body:
  - type: markdown
    attributes:
      value: |
        Thanks for helping improve our documentation! Please fill out the details below.
  
  - type: textarea
    id: summary
    attributes:
      label: Summary
      description: Briefly describe what needs to be updated or added.
      placeholder: "Explain the issue or improvement clearly..."
    validations:
      required: true

  - type: dropdown
    id: doc_type
    attributes:
      label: Type of Documentation
      options:
        - README / Getting Started
        - API Reference
        - User Guide / Tutorial
        - Architecture / Design
        - Other
    validations:
      required: true

  - type: textarea
    id: location
    attributes:
      label: Affected Page(s) or File(s)
      description: Provide links or paths to the relevant docs.
      placeholder: "e.g., docs/getting-started.md, README.md"
  
  - type: textarea
    id: proposal
    attributes:
      label: Suggested Changes
      description: What should be changed, added, or clarified?
      placeholder: "Provide details or examples of the improvements."
  
  - type: textarea
    id: context
    attributes:
      label: Additional Context
      description: Any extra information, screenshots, or related issues.
  
  - type: checkboxes
    id: checklist
    attributes:
      label: Checklist
      options:
        - label: "I've checked existing issues for duplicates"
          required: true
        - label: "I've read the contributing guidelines"
          required: false
