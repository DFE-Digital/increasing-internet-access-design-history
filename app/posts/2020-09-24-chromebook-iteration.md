---
title: Iteration of Chromebook guidance and forms
description: Make it clearer what devices are available
date: 2020-09-24
---

Problems with the current form include:

- schools and responsible bodies believing that only Google Chromebooks are available to order
- this information is not always completed before ordering

## Design notes

- List all the devices available at the start to set the right context (except on the school wizard, where we set this context on a prior page)
- Introduce a "Before you can order" page which we show to all school users when they sign in to a school that hasn’t given this information yet

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "School wizard journey",
      img: { src: "01-school-wizard-journey.png" }
    }, {
      text: "School wizard journey – I don’t know selected",
      img: { src: "04-school-wizard-journey-i-dont-know.png" }
    }, {
      text: "School subsequent sign in, when details haven’t been given yet",
      img: { src: "02-school-subsequent-sign-in.png" }
    }, {
      text: "Responsible body – a school managed centrally",
      img: { src: "03-responsible-body-school-managed-centrally.png" }
    }]
}) }}
