---
title: State-funded pupils at independent special settings
description: Adding a new type of school so local authorities can order laptops for state&#8209;funded pupils at independent special settings
date: 2021-03-19
related:
  items:
  - text: Trello – LA to order devices on behalf of Independent Special Schools
    href: https://trello.com/c/60deUvx9/1642-la-to-order-devices-on-behalf-of-independent-special-schools
---

{% from "figure/macro.njk" import appFigure with context %}

Laptops are now available for pupils who have state funding to attend an independent special setting (ISS) and are eligible for free school meals (or do not have access to a suitable device for remote education or catch-up learning). Each LA has been allocated laptops based on the ’January 2020 Alternative provision census’ data. This is approximately 4,000 pupils at 600 schools, in most of the local authorities in England.

Giving an independent special settings access to Get help with technology wasn’t possible. Instead the decision was taken to create a ‘placeholder school’ for each local authority. The placeholder schools are allocated laptops for the state-funded pupils the LA is responsible for. This means the LA needs to manage finding out what laptop types each pupil needs and distributing it to them. The LA is also responsible for the laptop and will need to manage maintenance and redistribution.

### Adding users to our service

The users who are going to manage getting laptops for these state-funded pupils are not likely to be the same members of the LA who are already using the service. We’ve emailed LAs to get contact details of who they think is best placed to manage this.

Once we have these contacts, we need to know if their allocation is correct and their delivery address. Getting this information up-front allows us to create TechSource accounts as soon as possible and not slow-down ordering. To get this information we decided to use a Google form. This should give us relatively clean data (in comparison to managing this through emails). 

Once we have this data we can add these users to our service.

#### Google form

{{ appFigure({
  image: {
    file: "google-form/google-form-01.png"
  }
}) }}

{{ appFigure({
  image: {
    file: "google-form/google-form-02.png"
  }
}) }}

{{ appFigure({
  image: {
    file: "google-form/google-form-03.png"
  }
}) }}

If ‘No, someone else will place orders’, go to section 'Who will place orders for these laptops?'

Else go to next section.

{{ appFigure({
  image: {
    file: "google-form/google-form-03-a-01.png"
  }
}) }}

{{ appFigure({
  image: {
    file: "google-form/google-form-03-a-02.png"
  }
}) }}

If ‘No, the allocation is wrong’, go to section ’Tell us why your allocation is wrong’

Else submit the form.

{{ appFigure({
  image: {
    file: "google-form/google-form-03-a-03-b-01.png"
  }
}) }}

Submit the form.

{{ appFigure({
  image: {
    file: "google-form/google-form-03-b-01.png"
  }
}) }}

If ‘Yes, I can nominate someone else', go to section ‘Nominated person to place orders for latops’

Else submit the form.

{{ appFigure({
  image: {
    file: "google-form/google-form-03-b-02.png"
  }
}) }}

Submit the form.

### ‘School’ user journey

When we add users they could either belong to the LA or the placeholder school. We decided against adding the user to the LA exposes them to the rest of the service the LA can see (all the actual schools, opting-in to the Daily&nbsp;Mail campaign). Although this has the benefit of giving a consistent experience to users who belong to the same organisation, it potentially shows the user parts of the service they don’t need to see and means the user won’t see the first-time flow for schools.

By adding the user to the placeholder school directly reduces what they’ll see to whats immediately relevant and has the benefit of taking them through the setup screens that all school users see when signing-in to the service for the first time.

#### First-time sign-in flow

To introduce the user to the service we’re using the same flow as the first-time flow for a school with some adjustments.

The flow for the placeholder school:

1. Get laptops for state-funded pupils at independent settings (formerly: You’re signed in as [ school name ])

{{ appFigure({
  image: {
    file: "school_welcome.png"
  }
}) }}

2. How we look after personal information as part of the Get help with technology service (unchanged)

3. Allocation (content changed)

{{ appFigure({
  image: {
    file: "school_allocation.png"
  }
}) }}

4. Do you need to give someone else access? (content changed)

{{ appFigure({
  image: {
    file: "school_other-ordering.png"
  }
}) }}

5. Laptops you can order (content changed)

{{ appFigure({
  image: {
    file: "school_devices-you-can-order.png"
  }
}) }}

As well as content changes, this flow skips:
- Will you order Chromebooks? – because this becomes a much more complex question when ordering for an unspecified and possibly unknown number of schools we have moved it to the ordering part of the flow
- What happens next – this is no longer as necessary as these users will have a TechSource account and be able to order

###  State-funded pupils school views

#### Homepage

Once the user has finished the flow they are on the account homepage for that school. 

There are a few content changes and we hide the option to Opt-in to Daily&nbsp;Mail’s donated device scheme.

{{ appFigure({
  image: {
    file: "school.png"
  }
}) }}

#### Ordering flow

To give more guidance to assist users with some of the additional complexity these users need to contend with, the ordering flow has been split out into a few more pages.

1. Get laptops

The first screen after 'Get laptops' is a summary of the number of devices, and give the user an overview of information they need before ordering.

{{ appFigure({
  image: {
    file: "la-funded-pupils.png"
  }
}) }}

If the user has ordered some, but all laptops, the card adds information about how many laptops have been ordered.

{{ appFigure({
  image: {
    file: "la-funded-pupils--some-devices-ordered.png"
  }
}) }}

If the user has ordered all laptops, the page changes to:

{{ appFigure({
  image: {
    file: "la-funded-pupils--all-devices-ordered.png"
  }
}) }}

1.1 Find out what type of laptop pupils need

Because the user is managing ordering for multiple schools, each with their own requirements and no shared IT infrastructure we added a screen to help the user get a summary of what is available and explain they may need to collect G Suite license information.

{{ appFigure({
  image: {
    file: "la-funded-pupils_laptops-types-for-la-funded-pupils.png"
  }
}) }}

2. Will you order include Google Chromebooks? 

To answer this question the user needs to have spoken to all the ISSs they are placing orders for. We’ve given the users up-front guidance about needing this information, but we anticipate most users will still not know the answer to this question. We don’t want to block users from progressing, so they can answer ’I’m not sure’.

Unlike the question as it appears for schools that are managing ordering for themselves, 'Yes, we’ll order Chromebooks' doesn't ask user for the Chromebook details.

Once the user has set their Chromebook preference, this page is skipped in the journey.

{{ appFigure({
  image: {
    file: "la-funded-pupils_chromebooks.png"
  }
}) }}

3. Order laptops

This page is the same as 'Order devices' page, but with updated content. 

{{ appFigure({
  image: {
    file: "la-funded-pupils_order.png"
  }
}) }}

We also replay the user’s Chromebook preference. This allows the user to change their preference before they order if this or subsequent orders will include Chromebooks.

If the user will order Chromebooks:

{{ appFigure({
  image: {
    file: "la-funded-pupils_order--chromebooks-yes.png"
  }
}) }}

If the user will not order Chromebooks:

{{ appFigure({
  image: {
    file: "la-funded-pupils_order--chromebooks-no.png"
  }
}) }}

If the user isn’t sure if they’ll order Chromebooks:

{{ appFigure({
  image: {
    file: "la-funded-pupils_order--chromebooks-not-sure.png"
  }
}) }}

### Responsible-body user journey

To reduce the risk of devices not being ordered by LAs we can increase visibility of laptops being made available to state-funded pupils by adding all LA users to the placeholder school.

#### Interstitial screen

Temporary change to the 'welcome' view. 

{{ appFigure({
  image: {
    file: "rb_interstitial.png"
  }
}) }}

#### Your organisation

Update to 'Your organisation' 

{{ appFigure({
  image: {
    file: "rb_your-organisation.png"
  }
}) }}
