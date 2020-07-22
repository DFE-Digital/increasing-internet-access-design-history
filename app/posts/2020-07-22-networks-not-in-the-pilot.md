---
title: Requests for networks not in the pilot
description: How we handle these requests and what happens if they come on board
date: 2020-07-22
---

When schools go out to families we’re recommending they record the details of people who need more data but who are with a network that isn’t in the pilot yet. Specifically, these networks are only those that we are talking to and that we have some expectation to join the service at a later date. They do not include many of the much smaller networks that we are not approaching.

For these requests we need to:

- indicate that the request hasn't been made yet
- that the network is not on the service yet

## When a network joins the service

Should a network join at a later time we should:

- update each status from "unavailable" to "requested"
- send a text message to everyone on that network telling them:
  - their network is now on the service and we are requesting data for them
  - details of the offer now available to them

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Check your answers messaging",
      img: { src: "01-check-your-answers.png" },
      caption: "Append 'if they join the service' to the end of the check your answers message"
    }, {
      text: "Unavailable status",
      img: { src: "02-unavailable-status.png" },
      caption: "The success message has changed from 'request received' to 'request saved'. A grey status has been added and ‘(not on service yet)’ is appended to the network name."
    }]
}) }}
