---
title: Ordering devices at the school level
description: Designs for all variants of the order page
date: 2020-09-10
---

There are 5 variants of the Order devices page. They:

- cannot order yet
- cannot order yet, but only because their TechSource account isn’t ready yet
- can order devices for specific circumstances
- can order a full allocation because there are local coronavirus restrictions
- cannot order any more devices (but might be able to order more later)

These are an update on the [original design](/school-devices/#order-devices-order-now-local-restrictions-imposed).

This design aims to:
- callout the number of devices to order clearly
- give guidance on using TechSource and signing in (it’s not obvious on TechSource that User ID means an email address)
- warning that you must not order more than your allocation (orders will appear to go through but will get cancelled later)
- explain why only a few devices can be ordered when ordering for specific circumstances
- show how many devices have already been ordered and the total allocation

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "You cannot order devices yet",
      img: { src: "01-you-cannot-order-devices-yet.png" }
    }, {
      text: "School can order, but your TechSource account is not ready yet",
      img: { src: "10-techsource-account-not-ready-yet.png" }
    }, {
      text: "Order devices for specific circumstances",
      img: { src: "02-order-devices-specific-circumstances.png" }
    }, {
      text: "Order devices",
      img: { src: "03-order-devices.png" }
    }, {
      text: "Order devices with routers",
      img: { src: "04-order-devices-with-routers.png" }
    }, {
      text: "All devices ordered",
      img: { src: "05-all-devices-ordered.png" }
    }, {
      text: "Your school cannot order devices yet (non order user)",
      img: { src: "06-your-school-cannot-order-devices-yet-non-order-user.png" }
    }, {
      text: "Your school can order devices for specific circumstances (non order user)",
      img: { src: "07-your-school-can-order-devices-shielding-non-order-user.png" }
    }, {
      text: "Your school can order devices (non order user)",
      img: { src: "08-your-school-can-order-devices-non-order-user.png" }
    }, {
      text: "All devices ordered (non order user)",
      img: { src: "09-all-devices-ordered-non-order-user.png" }
    }]
}) }}
