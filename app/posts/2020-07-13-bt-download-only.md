---
title: Download BT log-ins
description: The user journey for our initial, much simplified, BT only service
date: 2020-07-13
---

Following the [initial design](/tell-us-who-needs-access), we expect to widen the BT pilot:

* before the mobile network offer is launched
* without needing responsible bodies to gather numbers on who needs access and who is eligible

We’ve pre-calculated allocations of log-ins based on free school meals (FSM) and school census data.

We don’t need:

* forms to gather numbers on who need access or eligibility
* forms for the mobile network offer
* a start page before signing in (it would only say ‘Sign in to download’)
* a summary page before downloading log-ins (there is nothing to summarise)

When the mobile network offer is enabled, we’ll need a new start page and summary page.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Sign in",
      img: { src: "01-sign-in.png" }
    }, {
      text: "Check email",
      img: { src: "02-check-email.png" }
    }, {
      text: "Download logins",
      img: { src: "03-download-logins.png" }
    }]
}) }}
