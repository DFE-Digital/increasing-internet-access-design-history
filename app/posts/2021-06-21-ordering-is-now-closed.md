---
title: Ordering is now closed
description: Simplify the service while its closed for ordering devices and internet access.
date: 2021-06-21
---
Users will not be able to order laptops, tablets or routers, or request internet access after 4pm 30 July 2021.

Users will still be able to:
- access TechSource (if their account has access)
- access the Computacenter ‘Support Portal’ (if their account has access)
- invite other users
- check MNO request
- see their Huawei router password, until 30 July

These are the changes we propose to make to user’s accounts.

## We did not recognise that email address

Change ‘How to access this service to order laptops, tablets and internet connectivity’ to ‘How to access this service’

{% from "figure/macro.njk" import appFigure with context %}

{{ appFigure({
  image: {
    file: "01-we-did-not-recognise-that-email-address.png"
  }
}) }}

## Interstitial

Updated summary of what users can do when signed-in.

Makes interstitial the same for all school, placeholder school and responsible body users.

{{ appFigure({
  image: {
    file: "02-interstitial.png"
  }
}) }}

## Account homepage

The account page is the largest single change. The aim is to give an overview of that the user can do, prioritised by the expected user needs. Given the reduction in features we’ve simplified the journeys and removed most of the pages.

The grey ‘card’ component is moved to this page and instead of telling users how many devices they can order it tells users they cannot order and summarises their activity.

The primary user need we need to meet after 30 June is to help users reset their devices. The page prioritises linking to the Support Portal and managing accounts so users can access the Support Portal.

The user can also see their existing MNO requests and orders in TechSource.

As the page is summarising what a user can do its conditional on a number of states.

Everything else has been removed.

{{ appFigure({
  image: {
    file: "03-account-homepage.png"
  }
}) }}

### Summary states

The order summary has a number of states depending on what the user ordered:

If the user’s organisation didn't receive any laptops, tablets, routers or extra data:

{{ appFigure({
  image: {
    file: "04-summary--nothin.png"
  }
}) }}

If the user’s organisation received just laptops and tablets, just routers or just extra data:

{{ appFigure({
  image: {
    file: "05-summary--just-devices.png"
  }
}) }}

{{ appFigure({
  image: {
    file: "06-summary--just-routers.png"
  }
}) }}

{{ appFigure({
  image: {
    file: "07-summary--just-data.png"
  }
}) }}

If the user received 2 or more of 1 either laptops and tablets, routers, or extra data:

{{ appFigure({
  image: {
    file: "08-summary--two-things.png"
  }
}) }}

If the user received all types of assistance:

{{ appFigure({
  image: {
    file: "09-summary--three-things.png"
  }
}) }}

If the user belongs to a setting that is part of a virtual pool or a responsible body, summarise all schools that belong to that repsonsible body and use the type of responsible body:

{{ appFigure({
  image: {
    file: "10-summary--responsible-bodies.png"
  }
}) }}

### Access the Support Portal

If the user belongs to a school and does not have access to TechSource:

{{ appFigure({
  image: {
    file: "11-access-to-the-support-portal--school-no-access.png"
  }
}) }}

If the user belongs to a school and has access to TechSource:

{{ appFigure({
  image: {
    file: "12-access-to-the-support-portal--school-with-access.png"
  }
}) }}

If the user belongs to a responsible body:

{{ appFigure({
  image: {
    file: "13-access-to-the-support-portal--responsible-body.png"
  }
}) }}

### Reset devices

This section is only shown to user’s organisation received laptops and tablets, or routers.

If the organisation received laptops or tablets, but no routers:

{{ appFigure({
  image: {
    file: "14-reset-devices--laptops.png"
  }
}) }}

If the organisation received no laptops or tablets, but routers:

{{ appFigure({
  image: {
    file: "15-reset-devices--routers.png"
  }
}) }}

If the organisation received laptops or tablets and routers:

{{ appFigure({
  image: {
    file: "16-reset-devices--all.png"
  }
}) }}

### Order history

#### School users

If the user belongs to a school, has access to TechSource and their school – or responsible body, if part of a virtual pool – did not request any extra data:

{{ appFigure({
  image: {
    file: "17-order-history--school--techsource.png"
  }
}) }}

If the user belongs to a school school – or responsible body, if part of a virtual pool – does not have access to TechSource but their organisation requested extra data:

{{ appFigure({
  image: {
    file: "18-order-history--school--extra-data.png"
  }
}) }}

If the user belongs to a school school – or responsible body, if part of a virtual pool – has access to TechSource and their organisation requested extra data:

{{ appFigure({
  image: {
    file: "19-order-history--school--all.png"
  }
}) }}

If the user belongs to a responsible body, the behaviour is the same as the school but the user can see the list of their schools and colleges.

{{ appFigure({
  image: {
    file: "20-order-history--responsible-body.png"
  }
}) }}


## Manage users

The content has been tweaked to emphasise access to the Support Portal.

School users:

{{ appFigure({
  image: {
    file: "21-manage-users--school.png"
  }
}) }}

Responsible body users:

{{ appFigure({
  image: {
    file: "22-manage-users--responsible-body.png"
  }
}) }}

## Invite users

The school user invite allows users to choose if the new user has access to the Support Portal:

{{ appFigure({
  image: {
    file: "23-invite-user--school.png"
  }
}) }}

Updated invite error message:

{{ appFigure({
  image: {
    file: "24-invite-user--school--error.png"
  }
}) }}

## Extra data

Removes the order now button and explains the end of the scheme.

{{ appFigure({
  image: {
    file: "25-mno-requests.png"
  }
}) }}

## Setting list

The list is now a single table, simplified now users cannot take any action.

List of settings not in a virtual pool:

{{ appFigure({
  image: {
    file: "26-school-list--no-v-cap.png"
  }
}) }}

List of settings in a virtual pool:

{{ appFigure({
  image: {
    file: "27-school-list--v-cap.png"
  }
}) }}

## School summary

Summary of the setting, for a school that in not part of a virtual pool:

{{ appFigure({
  image: {
    file: "28-school-summary--no-v-cap.png"
  }
}) }}

Summary of the setting, for a school that in part of a virtual pool:

{{ appFigure({
  image: {
    file: "29-school-summary--v-cap.png"
  }
}) }}
