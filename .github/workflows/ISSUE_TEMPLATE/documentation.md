
name: 📝 Documentation Update
description: Improve Documentation
title: "[Doc]: "
labels: [documentation]


body:
  - type: checkboxes
    id: existing-issue
    attributes:
      label: Is there an existing issue for this?
      description: Please search to see if an issue already exists for the updates you want to make.
      options:
        - label: I have searched the existing issues
          required: true
          

  - type: textarea
    id: issue-description
    attributes:
      label: Issue Description
      description: Please provide a clear description of the documentation update you are suggesting.
      placeholder: Describe the improvement or correction you'd like to see in the documentation.
    validations:
      required: true
      

  - type: textarea
    id: suggested-change
    attributes:
      label: Suggested Change
      description: Provide details of the proposed change to the documentation.
      placeholder: Explain how the documentation should be updated or corrected.
    validations:
      required: true
      

  - type: textarea
    id: rationale
    attributes:
      label: Rationale
      description: Why is this documentation update necessary or beneficial?
      placeholder: Explain the importance or reasoning behind the suggested change.
    validations:
      required: false
      

  - type: dropdown
    id: urgency
    attributes:
      label: Urgency
      description: How urgently do you believe this documentation update is needed?
      options:
        - High
        - Medium
        - Low
      default: 0
    validations:
      required: true
      

  - type: checkboxes
    id: terms
    attributes:
      label: Acknowledgements
      description: Ensure you have read and agree to the project's guidelines.
      options:
        - label: I'm a GSSOC'24-Extd contributor
        - label: I'm a Hacktoberfest contributor
        - label: I have starred the repository
          required: true
        - label: 'I am willing to work on this issue (optional)'
          required: false
        
        
    