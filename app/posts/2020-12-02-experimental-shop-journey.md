---
title: Experimental order journey
description: How might ordering look in service
date: 2020-12-02
---

Many of the problems with our service stem from how we wrap another service, Computacenter’s TechSource.

TechSource cannot be easily updated to suit the journey we need for schools and responsible bodies, leading to workarounds such as:

- asking schools to check how many devices they can order before they go to TechSource
- asking users to sign in to multiple services
- asking schools to look up and enter their URN numbers
- virtual caps to allow responsible bodies to order devices for multiple schools to one place
- emails telling users when their TechSource account has been created
- instructions on how to sign in to TechSource

## A journey without visiting TechSource

We could collect order information directly and send that data to TechSource via an API. This would mean that all orders we send to TechSource could be trusted, there would be no need for their manual queue, meaning fewer delays.

We would probably need some sort of stock feed from them.

A generic ordering journey could allow us to order devices through a different supplier in the future.

## Benefits to our users

For our users it would mean:

- ordering directly through one service through a simpler, linear journey
- no delays waiting for TechSource accounts
- seeing how many devices they can order, with validations preventing over ordering
- contextual guidance about the devices being ordered (eg standard vs restricted)
- contextual fields asking for Chromebook and Apple iPad information, only when needed, with appropriate validation

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Which devices do you need?",
      img: { src: "01-which-devices-do-you-need.png" }
    }, {
      text: "How many? (of one type)",
      img: { src: "02-how-many-of-one-type.png" }
    }, {
      text: "How many? (of multiple types)",
      img: { src: "03-how-many-of-multiple-types.png" }
    }, {
      text: "What type of Windows devices?",
      img: { src: "04-what-type-of-windows-devices.png" }
    }, {
      text: "Delivery address",
      img: { src: "05-delivery-address.png" }
    }, {
      text: "Confirm order",
      img: { src: "06-confirm-order.png" }
    }, {
      text: "Confirmation",
      img: { src: "07-confirmation.png" }
    }]
}) }}
