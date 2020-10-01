---
title: Update service to cover self-isolating children
description: A new policy means a school’s full allocation is available when 15 children are self-isolating
date: 2020-09-25
related:
  items:
  - text: Trello
    href: https://trello.com/c/ZVplguD0/681-update-service-to-cover-self-isolating-children
  - text: Suggested content changes
    href: https://docs.google.com/document/d/1tlPOmF9oF8PJ4FKy6NEatcavC-2Koe9305EvzKQ_eKA/
  - text: Prototype PR
    href: https://github.com/DFE-Digital/get-help-with-tech-prototype/pull/19
---

{% from "govuk/components/warning-text/macro.njk" import govukWarningText %}
{{ govukWarningText({
  html: 'The reporting was simplified and we are building <a href="/15-self-isolating-2">a simpler design</a>',
  iconFallbackText: "Warning"
}) }}

A new policy was introduced meaning that schools can order their full allocation of devices if they have 15 or more self-isolating children in years 3 to 11.

Currently we say that:
- you can only order your full allocation when there are local restrictions
- you can request some devices for children under specific circumstances

This policy is awkward from a design perspective because:
- it’s new eligibility criteria for ordering all devices
- that eligibility does not happen automatically, we must be told by schools directly
- the request for devices is not necessarily for those who are self-isolating (the allocation can be more than 15 for instance)

## Design notes

In this design we’ve needed to:
- change guidance on when you can order a full allocation to include the new policy
- separate the two cases that allow you to order a full allocation. We have to indicate that one will happen automatically, and the other must be requested
- incorporate guidance for making this request in a logical place, which is a similar action to requesting devices for specific circumstances requests, but asking for different information and with a different outcome

For the two types of requests we tried a few options before settling on a version with tabs. Tabs were a last resort after trying:
- separate pages – on their own these pages worked, but when trying to add links to them from the index pages they appeared too similar and were difficult to distinguish
- one long page - after describing the different cases, the important information about where to send the request was pushed too far down the page
- a page with an accordion – the accordion did not sit well within the page

## Dev notes

Following a request because children are self-isolating, the process of allowing a school to order its full allocation is no different than if local restrictions were confirmed. ie The school should go into the same state and see the same order pages.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "School: Index",
      img: { src: "01-school-index.png" }
    }, {
      text: "School: Order devices – cannot order yet",
      img: { src: "02-school-cannot-order-yet.png" }
    }, {
      text: "School: Request devices for disadvantaged children",
      img: { src: "03-school-request-devices-disadvantaged.png" }
    }, {
      text: "School: Request devices if children are self-isolating",
      img: { src: "04-school-request-devices-self-isolating.png" }
    }, {
      text: "School: Onboarding wizard - You cannot order yet",
      img: { src: "05-school-wizard-you-cannot-order-yet.png" },
      caption: "
If a school can already order its full allocation this page should be skipped in the onboarding wizard.
      "
    }, {
      text: "Responsible body: Devices index",
      img: { src: "06-responsible-body-devices-index.png" }
    }, {
      text: "Responsible body: Order devices – cannot order yet",
      img: { src: "07-responsible-body-cannot-order-yet.png" }
    }, {
      text: "Responsible body: Request devices for disadvantaged children",
      img: { src: "08-responsible-body-request-devices-disadvantaged.png" }
    }, {
      text: "Responsible body: Request devices if children are self-isolating",
      img: { src: "09-responsible-body-request-devices-self-isolating.png" }
    }]
}) }}
