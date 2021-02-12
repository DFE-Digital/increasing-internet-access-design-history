---
title: Opting in to Daily Mail scheme (early designs)
description: Original designs were shown on sign in
date: 2021-02-11
---

Earlier versions of the [Daily Mail scheme](/daily-mail-scheme) designs.

Originally we expected all donated devices to be Microsoft Windows Laptops, meaning we did not need to gather a preference for device types. We attempted a single page opt in, which we planned to show when users sign in.

As the journey became more complex – preferences, disclaimers, privacy implications, and plenty to explain about how this scheme differs from the Get help with tech one, we switched to a page-per-thing journey.

It was also felt by DfE that showing the scheme at sign in would interrupt users from their order devices journey. Instead we favoured links on the signed in homepages.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "School journey opt in to donated laptops",
      img: { src: "01-school-journey-opt-in-to-donated-laptops.png" }
    }, {
      text: "Responsible body journey opt in to donated laptops",
      img: { src: "02-responsible-body-journey-opt-in-to-donated-laptops.png" }
    }, {
      text: "Pick schools and devices together",
      img: { src: "03-pick-schooles-and-devices-together.png" }
    }]
}) }}
