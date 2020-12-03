---
title: Responsible bodies ordering Chromebooks for schools with different G Suite domains
description: An edge case created by allow ordering for multiple schools (virtual caps)
date: 2020-11-27
related:
  items:
  - text: Trello (investigation into data)
    href: https://trello.com/c/xNNHcMXp/1025-look-up-data-on-trusts-that-have-set-different-chromebook-domain-names-for-their-schools
  - text: Trello (design ticket)
    href: https://trello.com/c/NVuGa9ye/1079-virtual-caps-and-chromebooks-design-ticket
---

## The problem

Moving to showing Responsible Bodies (RB) their device allocation for all schools (instead of per school)introduces a problem when ordering Chromebooks. 

Currently Computacenter configures Chromebooks using the ‘G Suite for Education’ domain of a URN given during checkout. However if the RB is reponsible for schools with different ‘G Suite for Education’ domains its not possible to tell TechSource how many Chromebooks are intended for which school. If the G suite domain is different to the school that will be using it, students and staff can’t use that Chromebook. It’s difficult for Computacenter to apply a new G Suite for Education licence to the Chromebook.

There are 57 RBs that manage schools with more than one G suite domain. [See a full breakdown of RBs with more than 1 domain](https://trello.com/c/xNNHcMXp/1025-look-up-data-on-trusts-that-have-set-different-chromebook-domain-names-for-their-schools)

## The solution

We have given TechSource a list of the RBs that manage schools with more than 1 domain and they have set the cap for those schools to 0. The RB can still place an order as normal, but the order will be processed manually by TechSource. If the order includes Chromebooks, TechSource will contact the RB by email to get the information on what emails.

These RBs will also see guidance in the ‘How to order’ section of the guidance.

## Screenshot

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Responsible bodies – order devices",
      img: { src: "01-responsible-body-devices-order.png" }
    }]
}) }}

