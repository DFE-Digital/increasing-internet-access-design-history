---
title: Give each MNO request its own page
description: Make a space to explain each request
date: 2021-01-22
---

In research with schools and trusts we’ve found that users do not:

- understand all the MNO statuses
- know where to find details about what each network offers
- know how to respond to a request with a problem

In this design we've created a page for each request. On each request we:

- give details about the request
- re-iterate the network offer that’s available for this request
- give next steps when the request has a problem

On the request page we’ve also:

- added a statuses key
- included a requested date on the requests table
- sorted the table by requested date, newest first

In early research we’ve seen that users know to click on these requests.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Updated requests table",
      img: { src: "01-updated-requests-table.png" }
    }, {
      text: "Key for statuses",
      img: { src: "02-key-for-statuses.png" }
    }, {
      text: "Completed request",
      img: { src: "03-completed-request.png" }
    }, {
      text: "Unknown number",
      img: { src: "04-unknown-number.png" }
    }, {
      text: "Unknown name",
      img: { src: "05-unknown-name.png" }
    }, {
      text: "Not eligible",
      img: { src: "06-not-eligible.png" }
    }, {
      text: "Other problem",
      img: { src: "07-other-problem.png" }
    }, {
      text: "Unavailable",
      img: { src: "08-unavailable.png" }
    }]
}) }}
