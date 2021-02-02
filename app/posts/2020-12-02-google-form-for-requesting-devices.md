---
title: Google form for requesting devices
description: Support sends this form following an initial request
date: 2020-12-02
---

When a user contacts support with a request for devices for specific circumstances, we send them a link to this Google Form.

We could link to this form directly and pre-fill some of the required information.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Request a device for a shielding child",
      img: { src: "01-request-a-device-for-a-shielding-child.png" }
    }, {
      text: "Validation: Check all boxes",
      img: { src: "07-validation-check-all-boxes.png" }
    }, {
      text: "Contact information",
      img: { src: "02-contact-information.png" }
    }, {
      text: "Request a device for a child who is clinically extremely vulnerable",
      img: { src: "03-request-a-device-for-a-child-who-is-clinically-extremely-vulnerable.png" }
    }, {
      text: "Request a device for a child in a household with someone who is clinically extremely vulnerable",
      img: { src: "04-request-a-device-for-a-child-in-a-household-with-someone-who-is-cev.png" }
    }, {
      text: "Internet connectivity",
      img: { src: "05-internet-connectivity.png" }
    }, {
      text: "How many need internet connectivity",
      img: { src: "06-how-many-need-internet-connectivity.png" }
    }]
}) }}
