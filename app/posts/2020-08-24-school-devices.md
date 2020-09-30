---
title: Schools that will place their own orders
description: The user journey for school users invited by their responsible body
date: 2020-08-24
---

When a responsible body devolves ordering to a school we invite their nominated contact to the service. This is the journey that the first user for a school will go through.

A slightly different journey will be needed for users the school invites later.

## Onboarding

The first time a school user signs in they will see a sequence of pages.

These pages aim to collect the information we need immediately.

They ask:

- about who at the school will be placing orders
- for further contact details right away
- for Chromebook details right away

They give context about:

- how many devices they can order and when they can order them
- the accounts we will create for them

## After onboarding

After onboarding is completed, when the user signs in they are taken to the signed in home page.

From this page they can:

- order devices
- check their school details
- manage school users

### Order devices

This page changes depending on whether local restrictions are imposed or not.

TechSource does not:
- warn people about ordering more than their allocation
- prevent people from ordering when their allocation is 0 (their order will go into a list and later be rejected)
- tell people how many devices they can order

The design intends to act as a front-door to TechSource to alleviate those issues. In doing so it:

- prevents users from going to TechSource before they can order anything
- when they can order, it tells them how many devices they can order

TechSource accounts might be created months before they are needed – those emails might get lost, users might forget their password, or forget which email they need to use to sign in. This page can help by telling users which email to use and how to reset their password.

### Check school details

- Edit or set chromebook details
- Review and query allocations

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Welcome",
      img: { src: "01-welcome.png" }
    }, {
      text: "Privacy notice",
      img: { src: "02-privacy-notice.png" }
    }, {
      text: "Your allocation",
      img: { src: "03-your-allocation.png" }
    }, {
      text: "Order restrictions",
      img: { src: "04-order-restrictions.png" }
    }, {
      text: "Are you ordering (did not build)",
      img: { src: "05-are-you-ordering.png" },
      caption: "
We chose not to build this page. Instead we defaulted the first user as being someone who can order. This means we have certainty that every school has someone who can place orders.

We needed this when schools were limited to 2 TechSource accounts, but we managed to bump that up to 3.
      "
    }, {
      text: "You will get an account",
      img: { src: "06-you-will-get-an-account.png" }
    }, {
      text: "Give someone else an account",
      img: { src: "07-give-someone-else-an-account.png" }
    }, {
      text: "Ordering chromebooks",
      img: { src: "08-ordering-chromebooks.png" }
    }, {
      text: "What happens next",
      img: { src: "09-what-next.png" }
    }, {
      text: "Signed in home page after onboarding",
      img: { src: "10-signed-in-home-page-after-onboarding.png" }
    }, {
      text: "Order devices: You cannot order yet",
      img: { src: "11-order-devices-you-cannot-order-yet.png" }
    }, {
      text: "Order devices: Order now (local restrictions imposed)",
      img: { src: "12-order-devices-order-now.png" }
    }, {
      text: "Check your school details",
      img: { src: "13-check-your-school-details.png" }
    }, {
      text: "Manage who can order devices",
      img: { src: "14-manage-who-can-order-devices.png" }
    }]
}) }}
