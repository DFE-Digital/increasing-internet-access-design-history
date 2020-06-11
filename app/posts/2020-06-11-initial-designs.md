---
title: Initial designs
description: First pages created for the service
date: 2020-06-11
---

First pages created for the service.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Home page",
      img: { src: "01-home-page.png" }
    }, {
      text: "How many eligible young people",
      img: { src: "02-how-many-eligible-young-people.png" }
    }, {
      text: "Form success",
      img: { src: "03-form-success.png" }
    }, {
      text: "Tell us about an eligible young person",
      img: { src: "04-tell-us-about-an-eligible-young-person.png" }
    }, {
      text: "Second form success",
      img: { src: "05-second-form-success.png" }
    }, {
      text: "Sign in",
      img: { src: "06-sign-in.png" }
    }, {
      text: "Check your email",
      img: { src: "07-check-your-email.png" }
    }]
}) }}
