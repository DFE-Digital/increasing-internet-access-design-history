---
title: Order devices from each school page
description: Allow responsible bodies to order from the school page
date: 2020-09-14
---

We prefer responsible bodies to place 1 order per school. The current "Order devices" screen, which shows all schools and what can be ordered for each could encourage a single order delivered to a central place.

Problems with the current Order devices screen:
- when the schools list is long, the order button gets missed at the bottom
- users navigate to the school expecting to order from there

Users on the schools list may find it difficult to reach the order devices page.

## Design updates

Match the place order designs for the devolved to schools journey:

- use a [similar panel on the school page as the school order journey uses](/ordering-devices-school/#order-devices-for-specific-circumstances)
- use a [similar "Order now" page for each school](/ordering-devices-school/#order-devices)

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Schools can order",
      img: { src: "01-schools-can-order.png" }
    }, {
      text: "Devolved school details",
      img: { src: "02-devolved-school-details.png" }
    }, {
      text: "Centrally managed school",
      img: { src: "03-centrally-managed-school.png" }
    }, {
      text: "Order devices now",
      img: { src: "04-order-devices-now.png" }
    }]
}) }}
