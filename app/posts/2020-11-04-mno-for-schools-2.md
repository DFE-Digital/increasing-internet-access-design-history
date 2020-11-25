---
title: Schools requesting extra mobile data (iteration)
description: Update eligibility and guidance, add routers
date: 2020-11-04
---

An [iteration of the original design](/mno-for-schools).

We needed to make eligibility clearer. Children are only eligible if they do not have broadband access at home and cannot afford extra data. Equally there's a distinction between making requests for specific circumstances and making requests when there’s a closure.

## No request limits

Networks are nervous about schools making too many requests, and making requests for children who are not eligible.

We originally proposed a limit of 10 requests which would be lifted when a school reports closures. In practice this limit was difficult to explain and justify, and was poorly understood in research. So we removed the limit of 10. Instead we have focused on putting the eligibility criteria up front.

If we observe schools making too many requests, we might respond by introducing a larger limit – one that could be communicated when schools are approaching it.

## Design changes

Changes include:

- remove the "Get the internet" and "Get laptops and tablets" differentiation – routers (which are devices for getting the internet) when requested will need to be ordered through Computacenter and the "Order devices" link. Instead add a new link to the top level, "Get internet access"
- introduce a new page for explaining specific circumstances and move requesting devices for specific circumstances beneath that page
- when making mobile data requests, separate "Your requests" page from an initial page of guidance
- use the new guidance page to explain eligibility and how to collect data

## Feature flags

For schools not in the mobile data rollout we should:

- hide the Get internet access link
- hide the new specific circumstances page in favour of request devices for specific circumstances
- keep a shorter breadcrumb on request devices for specific circumstances

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "School index page",
      img: { src: "01-school-index-page.png" }
    }, {
      text: "Get internet access",
      img: { src: "02-get-internet-access.png" }
    }, {
      text: "Request extra data for mobile devices",
      img: { src: "03-request-extra-data-for-mobile-devices.png" },
      caption: "Request limits were removed."
    }, {
      text: "Your requests",
      img: { src: "04-your-requests.png" }
    }, {
      text: "Get help for specific circumstances",
      img: { src: "05-get-help-for-specific-circumstances.png" }
    }, {
      text: "Request devices for specific circumstances",
      img: { src: "06-request-devices-for-specific-circumstances.png" },
      caption: "
This page now sits one level down, within the ‘Get help for specific circumstances’ section
      "
    }]
}) }}
