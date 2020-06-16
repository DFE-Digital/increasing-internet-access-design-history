---
title: Initial flow for mobile network operators (MNO)
description: Sign in journey and downloading requests
date: 2020-06-16
---

Mobile network operators (MNO) will have accounts set up for them, we don’t need to design a sign-in flow.

They will use a magic link to sign in and won’t need to set a password.

After signing in they will see a page showing data requests, ordered by request date.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Sign in",
      img: { src: "01-sign-in.png" }
    }, {
      text: "Check email",
      img: { src: "02-check-email.png" }
    }, {
      text: "Requests for extra data",
      img: { src: "03-requests-for-extra-data.png" }
    }]
}) }}
