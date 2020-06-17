---
title: Asking for names
description: Minimising the data we collect from responsible bodies
date: 2020-06-17
---

We started by asking for the name of the eligible young person. We then added fields to check if they were the account holder or not.

We don’t intend on sharing this data with mobile networks, meaning we might not need to collect it.

In this design we omit the name, and assume that:

- responsible bodies do not need the eligible young person’s name for tracking purposes
- responsible bodies will enter the correct name if they’ve been given more than one name (for example child and parent names from a school)
- account holders are always over 18 and never a child (this might not be the case for Pay as you go (PAYG) users)

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Only asking for account holder",
      img: { src: "04-only-asking-for-account-holder.png" }
    }, {
      text: "Check answers",
      img: { src: "05-check-answers.png" }
    }, {
      text: "Asking for eligible person and account holder (old design)",
      img: { src: "01-eligible-person-and-account-holder.png" }
    }, {
      text: "Check answers (not account holder)",
      img: { src: "02-check-answers-not-account-holder.png" }
    }, {
      text: "Check answers (is account holder)",
      img: { src: "03-check-answers-is-account-holder.png" }
    }]
}) }}
