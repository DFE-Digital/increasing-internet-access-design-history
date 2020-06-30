---
title: Gathering mobile data requests
description: Exploration into collecting numbers and networks, etc.
date: 2020-06-30
related:
  items:
  - text: Prototype PR
    href: https://github.com/DFE-Digital/increasing-internet-access-prototype/pull/3
  - text: Trello
    href: https://trello.com/c/OjdJRJWY/198-design-bulk-upload-flow-for-rbs
---

We had two possible approaches:

1. Bulk upload of collated data
2. Inviting schools to enter content directly

We have technical capacity to build one of these, at best.

## Bulk upload

- Requires each responsibly body to use the same spreadsheet format
- Spreadsheet can have limited validation
- Responsible bodies will need to collate each spreadsheet from each school
- May miss nuances of data, for example "Pay as you go or contract" is a question we only need to ask for some networks

## Inviting schools

- Avoids schools needing to maintain a spreadsheet
- Validation provided at point of data entry/capture
- Do responsible bodies know who to invite?
- Will they need to authorise requests?

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Bulk upload: Requests for extra mobile data",
      img: { src: "01-requests-for-extra-mobile-data.png" }
    }, {
      text: "Bulk upload: Upload a spreadsheet",
      img: { src: "02-upload-a-spreadsheet.png" }
    }, {
      text: "Bulk upload: Results of upload",
      img: { src: "03-results-of-upload.png" }
    }, {
      text: "Inviting schools: Invited users",
      img: { src: "04-invited-users.png" }
    }, {
      text: "Inviting schools: Inviting a new user",
      img: { src: "05-inviting-a-new-user.png" }
    }]
}) }}
