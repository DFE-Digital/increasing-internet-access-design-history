---
title: Responsible bodies requesting extra mobile data
description: Match school design with extra guidance
date: 2020-11-25
related:
  items:
  - text: Trello
    href: https://trello.com/c/DTLTjG1j/918-rbs-can-make-mno-requests-on-behalf-of-schools
---

An iteration on the [wave 1 design](/pilot-launch/#request-extra-mobile-data) to bring it inline with the more recent [schools design](/mno-for-schools-2/).

Our decision to keep mobile data requests open for all schools (rather than tying availability to whether they were open or closed for ordering) has simplified the responsible body journey. We do not need to judge the eligibility criteria of each school to determine if the feature should be available, and we do not need to assign each request to a specific school (which would have made bulk requests tricky and added design and development work for selecting schools in the manual flow).

## Responsible bodies that have devolved to all schools

When a local authority or trust has devolved all ordering to schools, then each school can also make data requests and request routers. We do not need to show any connectivity features to these responsible bodies.

## Responsible bodies that manage some or all schools centrally

Only 75 of 3235 had a mix of schools managed centrally or devolved.

For clarity, on the "Get internet access" page there is a section explaining:

> If you are ordering devices for a school, you must also make their requests for extra mobile data and routers.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Responsible body home page (managing some or all schools centrally)",
      img: { src: "01-index-managing-some-or-all-centrally.png" }
    }, {
      text: "Responsible body home page (devolved to all schools)",
      img: { src: "02-index-devolved-to-all.png" }
    }, {
      text: "Get internet access",
      img: { src: "03-get-internet-access.png" }
    }, {
      text: "Request data – new ‘use guide’ guidance",
      img: { src: "04-request-data-use-guide-guidance.png" }
    }, {
      text: "Request data – new ‘enter info’ guidance",
      img: { src: "05-request-data-enter-info-guidance.png" }
    }, {
      text: "How we ended the pilots",
      img: { src: "06-page-showing-pilots-ended.png" }
    }]
}) }}
