---
title: Devolving for multi-academy trusts
description: What’s different between trusts and local authorities
date: 2020-08-24
related:
  items:
  - text: Prototype PR
    href: https://github.com/DFE-Digital/increasing-internet-access-prototype/pull/12
---

Multi-academy trusts (MATs) will see a very similar service to local authorities (LAs).

## We do not make a recommendation on devolving or managing centrally

When making a choice whether to devolve or not, unlike for LAs where we recommend devolving to schools, instead we do not recommend an option. The best option will depend on how the trust is set up.

Content on the ‘Tell us who’ page has been tweaked and ‘recommended’ removed from the following radio buttons

## Other design differences

- ‘Managing trust users’ rather than ‘Managing local authority users’
- When managing centrally, it’s the "Trust" that orders, rather than "Local authority"
- Trusts can have 2 or more schools, when there’s 10 or fewer we hide the filters
- In the ‘Is there a school missing’ help text we do not refer to maintained and special schools

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Signed in home page",
      img: { src: "01-signed-in-home-page.png" }
    }, {
      text: "Tell us who",
      img: { src: "02-tell-us-who.png" }
    }, {
      text: "Who will place orders",
      img: { src: "03-who-will-place-orders.png" }
    }, {
      text: "Orders placed centrally",
      img: { src: "04-orders-placed-centrally.png" }
    }, {
      text: "Schools",
      img: { src: "05-schools.png" }
    }, {
      text: "School",
      img: { src: "06-school.png" }
    }]
}) }}
