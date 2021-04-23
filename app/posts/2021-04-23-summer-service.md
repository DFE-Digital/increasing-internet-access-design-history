---
title: Ordering through the service (Summer service)
description: An order journey that does not use TechSource
date: 2021-04-23
related:
  items:
  - text: Expanding order journey PR
    href: https://github.com/DFE-Digital/get-help-with-tech-prototype/pull/48
  - text: Adding responsible body journey PR
    href: https://github.com/DFE-Digital/get-help-with-tech-prototype/pull/49
---

In March we explored designs for ordering devices directly through the service, rather than through Computacenter’s TechSource platform. These designs built upon the [experimental order journey](/experimental-shop-journey/), which identified a number of user benefits to having the entire journey in a single place.

We focused on this because:

- Computacenter were planning on scaling down their own operation based on budgets, avoiding TechSource would reduce their costs and support burden
- We wanted to trial a supplier agnostic ordering approach
- The risk of trying a new way of ordering was low because order volumes were small

The designs were reviewed and iterated, and presented and demo'd many times, but they did not reach user research. The plans for the summer service were stopped when the decision was made not to turn off TechSource. At this point the designs were mature, but no development work had started.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Order devices (School)",
      img: { src: "01-order-devices-school.png" }
    }, {
      text: "Order devices (Responsible body)",
      img: { src: "02-order-devices-responsible-body.png" }
    }, {
      text: "Which devices?",
      img: { src: "03-which-devices.png" },
      caption: "
If the organisation does not have a router allocation, routers would not show in this list. For an MVP, the process of request a router allocation via support has not changed. A later iteration might instead incorporate an order for routers instead of an allocation request, where DfE would then approve or cancel the order.
      "
    }, {
      text: "How many routers?",
      img: { src: "04-how-many-routers.png" },
      caption: "We include a shortcut as we expect many users to order their full allocation."
    }, {
      text: "How many devices?",
      img: { src: "05-how-many-devices.png" }
    }, {
      text: "What type of Windows?",
      img: { src: "06-what-type-of-windows.png" },
      caption: "This screen only shows if Windows devices are chosen, and then only if DfE decides to continue offering built devices."
    }, {
      text: "Chromebook details",
      img: { src: "07-chromebook-details.png" },
      caption: "This screen only shows if Chromebooks are being ordered. If an organisation has previously given these details they will be pre-filled. By asking for these details at point of ordering, we could also remove all prompts elsewhere in the service that ask for this information (eg the school wizard at first sign in, or on the schools list for a responsible body)"
    }, {
      text: "Pick delivery address (Responsible body only)",
      img: { src: "08-pick-delivery-address-responsible-body.png" },
      caption: "Only responsible bodies need to make a choice about where the order will be delivered. Rather than a list of addresses, because the list can be very long and addresses are hard to parse, we use school names. The following delivery page then confirms the delivery address – that same screen is used for the school journey."
    }, {
      text: "Delivery address",
      img: { src: "09-delivery-address.png" }
    }, {
      text: "Delivery contact (I am the delivery contact)",
      img: { src: "10-delivery-contact-i-am.png" },
      caption: "We do not have telephone details for all users, but Computacenter require a telephone number so they or a courier can contact them about an order."
    }, {
      text: "Delivery contact (Someone else is the delivery contact)",
      img: { src: "11-delivery-contact-someone-else.png" },
      caption: "If someone else is the delivery contact, only they will receive the dispatch notification from Computacenter. The user placing the order will not receive anything."
    }, {
      text: "Safeguarding",
      img: { src: "12-safeguarding.png" }
    }, {
      text: "Check and confirm",
      img: { src: "13-check-and-confirm.png" }
    }, {
      text: "Order placed",
      img: { src: "14-order-placed.png" },
      caption: "The order ID shown used a form defined by Computacenter"
    }, {
      text: "Order history",
      img: { src: "15-order-history.png" },
      caption: "We did not decide where in the information architecture this page would sit."
    }, {
      text: "Previous order",
      img: { src: "16-previous-order.png" }
    }]
}) }}
