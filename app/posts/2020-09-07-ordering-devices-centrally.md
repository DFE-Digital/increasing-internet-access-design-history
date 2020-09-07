---
title: Ordering devices centrally
description: The journey for responsible bodies who choose to order devices for some or all schools centrally
date: 2020-09-07
---

The journey for a responsible body who will be ordering devices centrally is more complex than the one needed for schools.

They need to know which schools they can order for, why they can order, and how many devices they can order.

There are 5 variants of the Order devices page. They:

- cannot order for anyone yet
- cannot order but schools they devolved to can
- can order devices for specific circumstances
- can order a full allocation because there are local coronavirus restrictions
- cannot order any more devices (but might be able to order more later)

## School tables

We show a row for each school that:
* devices can be ordered for
* devices have been ordered for

Rows are currently listed alphabetically. It might make more sense to order them by total devices left to order.

If there's a widespread lockdown, these tables could get very long. The design doesn’t account for this yet. We'd probably need to defer to filtering on the schools list somehow.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Get laptops and devices",
      img: { src: "01-get-laptops-and-devices.png" },
      caption: "
The 'Order devices' link is only shown to responsible bodies who are managing at least one school centrally.
      "
    }, {
      text: "You cannot order yet",
      img: { src: "02-you-cannot-order-yet.png" },
      caption: "
The 'X schools' link should link to the schools list, preferably to a filtered view of the list
      "
    }, {
      text: "You cannot order yet (but others can)",
      img: { src: "03-you-cannot-order-yet-others-can.png" },
      caption: "
There is an extra section, ‘Some schools can place their own orders’
      "
    }, {
      text: "Order devices for specific circumstances",
      img: { src: "04-order-devices-for-specific-circumstances.png" }
    }, {
      text: "Order devices now",
      img: { src: "05-order-devices-now.png" }
    }, {
      text: "You’ve ordered all the devices you can",
      img: { src: "06-ordered-all-devices.png" }
    }]
}) }}
