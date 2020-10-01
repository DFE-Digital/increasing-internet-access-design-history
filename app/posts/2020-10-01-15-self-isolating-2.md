---
title: Iterate design for covering self-isolating children
description: Disruption will now be reported via the ed-settings form, rather than requesting through the service
date: 2020-10-01
related:
  items:
  - text: Original design
    href: /15-self-isolating
  - text: Prototype PR
    href: https://github.com/DFE-Digital/get-help-with-tech-prototype/pull/20
---

When a school has 15 or more self-isolating children, this will now be reported through the DfE education settings status form, which schools complete daily. This is also how we are notified of school closures, meaning the self-isolating and confirmed local restrictions eligibility criteria are aligned.

There is no longer a hybrid case where a full allocation must be requested through the service, as [we originally designed for](/15-self-isolating).

This means the new design only needs to:
- update the eligibility criteria for when a full allocation can be ordered
- be explicit about how we know there is disruption

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Responsible body cannot order yet",
      img: { src: "01-responsible-body-cannot-order-yet.png" }
    }, {
      text: "School cannot order yet",
      img: { src: "02-school-cannot-order-yet.png" }
    }, {
      text: "School wizard cannot order right away",
      img: { src: "03-school-wizard-cannot-order-right-away.png" }
    }]
}) }}
