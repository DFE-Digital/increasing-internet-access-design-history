---
title: Devolving device orders to schools
description: How responsible bodies choose to devolve, and how we’ll ask them for contact details
date: 2020-08-10
related:
  items:
  - text: GOV.UK Announcement
    href: https://www.gov.uk/guidance/get-laptops-and-tablets-for-children-who-cannot-attend-school-due-to-coronavirus-covid-19
  - text: Miro board
    href: https://miro.com/app/board/o9J_kpby-6s=/
  - text: Research notes
    href: https://docs.google.com/document/d/1EYZ9Y4naK4fp9EmbPnBVWPrpFJcSh0316bl-UDq6pVE/edit
---

A first pass at giving responsible bodies the opportunity to devolve managing of device orders to schools.

Responsible bodies can choose to:

- devolve to all schools
- devolve to some schools
- manage all schools centrally

Responsible bodies will need to:

- give contact details for each school being devolved (name, email and telephone number)
- give contact details for anyone managing orders centrally
- choose whether each school is devolved or managed centrally (if it’s a mixed picture)

We’ll use those contact details to:

- create users on our service
- allow those users to add or edit who can manage orders
- create accounts on TechSource for those users so they can order devices

{% from "figure/macro.njk" import appFigure with context %}
{{ appFigure({
  image: {
    file: "high-level-flow.png"
  },
  caption: 'A high level overview of the process'
}) }}

## Which responsible bodies should devolve to schools?

### Local authorities should devolve

Research from the connectivity pilots and wave 1 of devices has shown us that going to local authorities (LAs) rather than to schools puts us too far from the end user.

There are too many hops from DfE to the end user (the families who will use the device or voucher). We lose visibility of how vouchers or devices are being distributed, how many are given to families and what success they are having with them. By going direct to schools we shorten the distance between DfE and the end user.

Schools understand the needs of their children best. In a scenario where they need to choose what to order they’ll have a greater understanding than the local authority.

A minority of LAs have centralised IT services, those LAs might be better suited to managing devices centrally.

#### Hypotheses

If schools are managing orders directly, then they will order and configure their devices more quickly, meaning children will access remote education more quickly.

If we use guidance and warnings to nudge LAs in the design, then more will choose to devolve device management, meaning more schools will be in a position to directly order devices.

### Trusts could manage centrally

Many multi-academy trusts (MATs) have services, such as IT management, shared across schools. For MATs the total number of schools to manage will be much lower and centrally managed devices orders should be efficient.

## How many schools?

On average a local authority will need to give contact details for 140 maintained schools. There are some LAs who manage many more.

Giving that many details will be a significant effort. We need to understand:

- how LAs would approach this task
- if they already have some of the contact details
- how they would go through a list of schools (by type, A-Z, some other way)
- if this task is too big to complete and some schools will be left without details

| Local authority | Number of schools |
|--|--|
| Lancashire | 629 |
| Kent | 583 |
| Essex | 556 |
| Hertfordshire | 533 |
| Hampshire | 528 |

### Hypotheses

If we make it easy to go from one school to the next, then LAs will find it easier to complete each school’s contact details, so that we have a more complete collection of contact details.

If LAs can’t complete contact details for us, then we will default to contact details we’ve gathered from elsewhere (eg Get info about schools – this will probably end up being the headteacher), so that we can contact someone, even if it’s not the most appropriate person.

## Design notes

Notable things that are missing:

* when a responsible body chooses some schools to be centrally managed there’s currently no way to manage the responsible body’s central users
* when starting the journey and coming back again later, users shouldn’t be asked how they want to devolve, they should be taken straight to the list of schools
* what happens once all contact details are added is unclear

We might want more in-depth statuses showing whether schools have received our comms, and whether they have logged into the system.

## User research

We tested this design with large local authorities:

* They were very supportive of devolving to schools, based on the guidance published to GOV.UK they were already intending to ensure this. The participant selected the option 'Schools will manage their own orders' immediately. They didn't need to check with schools, they just made this decision.
* In phase 1 of devices, they were just a 'middle admin layer' - they only did the admin for forecast and allocation appeals (which involved loads of back and forth between schools and DfE) and took the orders/deliveries, all the configuration and onward distribution was delegated to social workers or schools.
* Huge admin task - the task of inputting all the contact data is a huge one, and the participant felt unnecessary. The majority of school in the list of about 600 are primary, so they would only be putting in headteacher details. For the 70-80 (maintained) secondary schools they may have contact details of an IT person, but may still opt to use headteacher contact details.
* Next steps? - They expect that the headteacher would access the service and put in the correct details of who would manage this at the school. It would have to be senior leadership and probably someone from IT. They thought there was definitely a role for the LA in communicating with schools. If they could see a list of which schools hadn't engaged/accessed the service, they could do targeted comms to make sure no schools missed out.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Logged in home page",
      img: { src: "01-logged-in-home-page.png" },
      caption: "
A [repurposed homepage](/pilot-launch/#logged-in-home-page) giving a direct choice between internet and devices.

For responsible bodies with access to the connectivity pilots it makes sense to keep these two things separate – those pilots will continue to be managed at the responsible body level, while devices will largely be devolved.

Post-pilot, the connectivity offers may also be devolved to schools.
      "
    }, {
      text: "Get devices",
      img: { src: "02-get-devices.png" },
      caption: "
A preamble explaining what we need responsible bodies to do and why.
      "
    }, {
      text: "Who will order devices: Some schools selected",
      img: { src: "03-who-will-order-some-selected.png" }
    }, {
      text: "Who will order devices: Centrally managed selected",
      img: { src: "04-who-will-order-centrally-selected.png" }
    }, {
      text: "All schools devolved: Give us contact details for each school",
      img: { src: "05-give-us-contact-details-for-each-school.png" }
    }, {
      text: "All schools devolved: Contact details for school",
      img: { src: "07-contact-details-for-school.png" }
    }, {
      text: "Some devolved: Tell us who will manage orders for each school",
      img: { src: "06-tell-us-who-will-manage-orders-for-each-school.png" },
      caption: "
When only some schools are devolved, there’s an extra column to indicate who is manage orders.
      "
    }, {
      text: "Some devolved: Who will order devices for school",
      img: { src: "08-who-will-order-devices-for-school.png" },
      caption: "
A choice must be made about who is managing orders for each school.
      "
    }, {
      text: "Some devolved: Who will order devices school selected",
      img: { src: "09-who-will-order-devices-school-selected.png" },
      caption: "
If the school will be managing orders, then we need to collect contact details.
      "
    }, {
      text: "Some devolved: Tell us who will manage some completed",
      img: { src: "10-tell-us-who-will-manage-some-completed.png" },
      caption: "
Once a choice is made and/or contact details gathered, we show the school as being completed.
      "
    }, {
      text: "Centrally managed: Who can order devices",
      img: { src: "11-who-can-order-devices.png" },
      caption: "
When managing centrally no list of schools will be shown. Instead the responsible body will be asked to give details of their own users, ie those who will be managing orders centrally.
      "
    }, {
      text: "Centrally managed: Give someone access to order devices",
      img: { src: "12-give-someone-access-to-order-devices.png" }
    }, {
      text: "An example full list of schools",
      img: { src: "13-an-example-full-list-of-schools.png" }
    }]
}) }}
