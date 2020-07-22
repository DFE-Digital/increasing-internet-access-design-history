---
title: Text messages we send
description: What we send when a request for data is made
date: 2020-07-22
related:
  items:
  - text: Trello
    href: https://trello.com/c/nNKhfK4c/305-text-message-for-all-mno-extra-mobile-data-requests
---

Each time a responsible body requests data for someone we need to send a text message to them.

In the privacy notice, we promise:

> If you decide to take up the offer, you’ll get a text message from the Department for Education with more information about your data protection rights.

The sender of the text message will be:
__GOVUK__

The message will be prepended with our service name:
__Department for Education: Increasing internet access for children__

If the network is in the pilot, when a request is received we will send:

> We’ve received your name and mobile number and passed them on to [name of mobile network operator] to request more data. You should hear from them within 14 days.
>
> See https://get-help-with-tech.education.gov.uk/mobile-privacy for details about how we use your personal information.

If the network is not in the pilot:

> We’ve received your name and mobile number. Unfortunately, [name of mobile network operator] is not taking part in our pilot, so you won’t get an increase in mobile data for now. We’ll let you know if they join at a later stage.
>
> See https://get-help-with-tech.education.gov.uk/mobile-privacy for details about how we use your personal information.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Message preview",
      img: { src: "01-message-preview.jpg" }
    }, {
      text: "Message received",
      img: { src: "02-message-received.png" }
    }]
}) }}
