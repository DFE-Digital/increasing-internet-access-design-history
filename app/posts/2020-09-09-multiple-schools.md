---
title: Proposal for managing multiple schools
description: A design for quickly onboarding users who manage multiple schools
date: 2020-09-09
---

Some school users will need to order devices for multiple schools. We need a design so we can support these users quickly.

Borrowing from Publish teacher training courses, we can [try the "multiple organsations" screen they use](https://bat-design-history.netlify.app/publish-teacher-training-courses/multiple-organisations/).

## What happens when they sign in

- "You’re signed in" page, without a school name showing
- If it’s their first sign in, continue will take them to the privacy page
- Privacy page, and subsequent sign-ins take them to the Your schools page
- The first time they select each school, we take them through the wizard
- After they've completed the wizard, we take them to the home page

## What happens to the wizard

We:
- show them the school’s allocation as normal
- tell them when they can order as normal
- need to show them a custom "Invite to the Computacenter TechSource website" page, they will get 1 account for both schools
- ask if they want to add any users, as normal, the same rules will apply
- tell them what laptops they can order as normal
- ask them for Chromebook details if they haven’t already been provided, as normal
- show them the "What next" page, but tweak the button to say "Finish and go to school page"

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Your schools",
      img: { src: "01-your-schools.png" }
    }, {
      text: "School page",
      img: { src: "02-school-page.png" }
    }]
}) }}
