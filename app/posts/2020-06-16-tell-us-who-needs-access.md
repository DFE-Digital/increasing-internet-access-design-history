---
title: Tell us who needs internet access
description: A first pass at capturing data from responsible bodies
date: 2020-06-16
---

A first pass at capturing the data we need from responsible bodies:

* how many eligible young people they know about
* how many of them can access a BT hotspot
* who needs additional mobile data

Things these designs are missing:

* guidance on collecting "how many" numbers
* support page for changing those numbers after submission
* easier choice of mobile network
* explanation of data offer for each network
* what happens when network isn’t part of offer
* questions about who is the device owner
* questions about privacy of end user

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "First login",
      img: { src: "01-first-login.png" }
    }, {
      text: "How many young people are eligible",
      img: { src: "02-how-many-young-people-are-eligible.png" }
    }, {
      text: "Check answers",
      img: { src: "03-check-answers.png" }
    }, {
      text: "Success",
      img: { src: "04-success.png" }
    }, {
      text: "Request extra mobile data",
      img: { src: "05-request-extra-mobile-data.png" }
    }, {
      text: "New request",
      img: { src: "06-new-request.png" }
    }, {
      text: "Check answers for request",
      img: { src: "07-check-answers-for-request.png" }
    }, {
      text: "Request success",
      img: { src: "08-request-success.png" }
    }, {
      text: "All steps started",
      img: { src: "09-all-steps-started.png" }
    }]
}) }}
