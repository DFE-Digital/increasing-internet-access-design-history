---
title: Nudge emails for devices
description: Trying to get more schools signed in and prepared early
date: 2020-10-07
related:
  items:
  - text: Trello
    href: https://trello.com/c/zN97lyuD/810-design-nudges-for-schools-not-on-service-yet
---
{% from "email/macro.njk" import appEmail %}

As of 7 October we have:

* 14,000 schools with users
* 4,700 of them have signed in
* 3,000 of those are ready (they’ve signed in and completed their Chromebook details)
* 9,300 have not signed in
* 800 schools have not had a decision made about whether the responsible body or the school should order

Why have over 9,000 not responded to our invites, and how can we get them onto the service?

## When should we send a nudge email?

* a one-off email to all schools who have not signed in yet
* automatically 5 days after a new school is invited
* an email to any school eligible to order but has not yet signed in

## Nudge email to schools who have not responded

{{ appEmail({
  subject: "Tell us who in your school will order devices if there’s disruption to face-to-face education",
  content: "Dear colleague,

  We wrote to you recently requesting details of who in your school will place orders for laptops and tablets if face-to-face education is disrupted by coronavirus (COVID-19).

  We have not yet received complete information from you. We need it now as some schools in your area are closing because of coronavirus.

  If you do not give us the information we need, you’re likely to experience delays when ordering. This means children will not get devices promptly and may not be able to learn remotely.

  ### Give us contact details

  You need to sign in to our Get help with technology service to submit the information we’ve asked for. To do this, go to:
   [https://get-help-with-tech.education.gov.uk/start](https://get-help-with-tech.education.gov.uk/start])

  Once you’ve signed in using your email address ([quote email]), you can:

  * give us contact details for people who will order devices for your school
  * find out the number of devices allocated to your school
  * see the types of devices you can order
  * give us technical details for Chromebooks if you’ll be ordering them
  * place orders (once we confirm you’re able to do this)

  ### Find out more about the ordering process

  Be aware that the process for ordering devices is different from the one used earlier this year. See [How and when to order laptops and tablets during coronavirus](https://get-help-with-tech.education.gov.uk/devices/how-to-order) for more information.

  You can email [COVID.TECHNOLOGY@education.gov.uk](mailto:COVID.TECHNOLOGY@education.gov.uk) if you have any questions.

  Regards,

  The Digital Infrastructure Team"
}) }}
