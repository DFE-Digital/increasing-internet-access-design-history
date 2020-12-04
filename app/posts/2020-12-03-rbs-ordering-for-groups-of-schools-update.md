---
title: Responsible bodies ordering for groups of schools (iteration)
description: After 3 rounds of testing, how we improved the feature to allow ordering for multiple schools (virtual caps)
date: 2020-12-03
related:
  items:
  - text: "Trello: Virtual caps epic"
    href: https://trello.com/c/Blj9SZ65/1007-virtual-cap
  - text: Data on Chromebook domains within a trust
    href: https://trello.com/c/xNNHcMXp/1025-look-up-data-on-trusts-that-have-set-different-chromebook-domain-names-for-their-schools
---

## Adding summary of devices to the overview of schools

After watching the first participant in user research was saw that going from the page with an overview of schools, to a single school and then ordering for all schools didn’t reflect the user’s understanding of ordering for a group of their schools.

Adding the summary of devices available with an order ‘button’ to the list of schools communicates ordering for all schools more clearly.

## Simplifying the sumary of devices

Changing ‘You’ve ordered N or N devices’ to ‘You’ve ordered N devices’ on the summary simplifies the primary message of the page. The ‘...of N devices’ doesn’t appear to be useful and the complexity of explaining it (the sum total of devices available to schools that have reported some form of disruption or have a been allocated devices for specific cirumstances) isn’t worth the user’s time.

## Splitting the school tables

Splitting the school tables by the disruption the schools have reported:
- shows more simply where the total devices available to order comes from
- allows for guidance on different states to be given in context
- means the status tag only communicates action users need to take to provide information about a school

## Adding context to ordering guidance

We added guidance to the ordering page to help users order for a group using TechSource. Because of this additional content we combined all the ordering information into a ‘How to order’, moving the ‘Before you start’ content into ‘Using TechSource for the first time’. 

This also gives a place to add guidance about ordering Chromebooks when necessary.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Schools list",
      img: { src: "01-shools-list.png" }
    }, {
      text: "Order devices",
      img: { src: "02-order-devices.png" }
    }]
}) }}