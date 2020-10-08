---
title: Let schools request extra mobile data directly
description: Give schools the same features that responsible bodies have
date: 2020-10-07
related:
  items:
  - text: Prototype PR
    href: https://github.com/DFE-Digital/get-help-with-tech-prototype/pull/21
  - text: Research Trello card
    href: https://trello.com/c/chqiMS1P/814-research-capturing-mno-data-with-schools
---

When we reopen the mobile network (MNO) offer we will:

- change the eligibility to align with local restrictions and specific circumstances
- put the offer closer to end users by allowing schools to make requests directly

As a quick solution schools will see the same screens as responsible bodies, specifically:

- a table of requests with a "New request" button
- a choice about the type of request (manual or a bulk upload)
- a request form
- a spreadsheet upload form
- guidance on how to collect the data

When a school is part of the MNO offer the school index page changes in a way that mirrors responsible bodies, so that:

- all devices pages move beneath a "Get laptops and tablets" section
- a new "Get the internet" section appears

## Iterating the feature for schools

Responsible bodies were not the users gathering mobile networks and numbers from families. We created a guide for them to share with schools to make the process easier.

Schools will be the users collecting this information, it might be appropriate to switch from a batch process of uploading data once it’s been collected, to a service where information is entered at the point of collection. We could provide guidance and validation at the point of use which will minimise user error and improve the journey.

However that depends on the users of our system also being the ones talking to families, which might not be the case. We need to do research.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "School index",
      img: { src: "01-school-index.png" }
    }, {
      text: "Get the internet",
      img: { src: "02-get-the-internet.png" }
    }, {
      text: "Request extra data",
      img: { src: "03-request-extra-data.png" }
    }]
}) }}
