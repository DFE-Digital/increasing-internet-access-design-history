---
title: Adding further education providers
description: Increasing allocations for schools with sixth forms and adding further education providers
date: 2020-12-11
related:
  items:
  - text: Prototype PR
    href: https://github.com/DFE-Digital/get-help-with-tech-prototype/pull/30
  - text: Trello
    href: https://trello.com/c/HYkgnfmW/1155-design-hill-bringing-fe-into-the-service
---

This post covers the ordering part of the service, but not guidance outside the ordering part of the service or TechSource.

At a high-level, we are either increasing a school’s allocation and not introducing a new entity, or adding an FE provider which is equivalent to a Single Academy Trust (don’t belong to a Local Authority).

### Conditional content

We could make content refering to schools and FE providers conditional depending on what educational setting the user is from (for example, ‘children in years 3 to 11’ will need to switch between that, ‘students in years 3 to 13’ and ‘students’ depending on the user). This adds a lot of complexity and I want to see if it’s possible to make changes seen by all users and keep the app simpler.

It’s also not possible to do this for most of the guidance so this keeps the service consistent.

I don’t think the changes to accommodate FE providers creates much, if any additional burden on the user but it’s something to be aware of in research.

## Increasing allocation for schools and academies with sixth forms

To communicate to users their allocation has increased to include sixth-form students we’ve used the notification banner. The banner has two states depending on if the school can order (because it has reported disruption or can [order devices proactively](/push)) or not.

Ideally, the banner would show the number of devices added but then it would need conditional states based on what has been ordered. For example it should potentially hide once the user has placed an order. But there’s no way to know if the user has seen the banner or the devices ordered are from the devices allocated to sixth form students.

The banner is identical for schools and Responsible Bodies.

The banners shouldn’t last long, probably removed within a week of the last users getting notified their allocation has increased.

#### School’s allocation is increased and can order

<img src="/images/fe-providers/01-sixth-form-banner--can-order.png"
     alt="Banner with second level heading 'Important', large bold text 'Your allocation has increased to include students in years 12 and 13' and regular text 'You can order more devices.' the 'order more devices' is a link">

The text in the banner links to the order page.

#### School’s allocation is increased but cannot order

<img src="/images/fe-providers/02-sixth-form-banner--cannot-order.png"
     alt="Banner with second level heading 'Important', large bold text 'Your allocation has increased to include students in years 12 and 13' and regular text 'You can order 30 more devices when you report a closure or 15 or more pupils self-isolating at the same time.'">

### Not showing how many devices are allocated for sixth form students as a separate number in the service

We'll tell users what their allocation has increased by in an email. We could also show users how many devices are allocated to sixth form students in the service. I don’t see much advantage to this as we don’t show allocation by year (or any other grouping) anywhere else and it adds complexity to the numbers we show in the service.

## Adding new further education providers to the service

There are a number of content changes to make the service inclusive of further education providers.

### First login flow

These changes are mostly adding further education provider or changing the scope of the students described.

Because users no longer get an email when a TechSource account is created for them we can remove the ‘Use the TechSource website to place orders’ page to shorten the first login flow.

#### Privacy notice

<img src="/images/fe-providers/03-privacy-statement.png"
     alt="Text from the privacy statement with the added text ', trusts and further education providers' highlighted">

#### Allocation

<img src="/images/fe-providers/04-allocation.png"
     alt="Text from the allocation description with the changed text 'students in year 3 or above' highlighted">

#### Chromebooks

<img src="/images/fe-providers/05-chromebooks.png"
     alt="Will you order chromebooks? question page, with 'Yes, we will order chromebooks' selected and the added text ', or college' highlighted">

## School’s non-flow changes

#### Homepage

Changes Get help for specific circumstances from ‘understand when children can get support’ to ‘understand when children and students can get support’.

Removes:
- ‘school’ from ‘Check your school details’
- ‘in your school’ from ‘Use this section to give others in your School’

<img src="/images/fe-providers/07-index.png"
     alt="Get help with technology homepage">

#### Making the ordering guide for schools consistent with Responsible bodies with virtual cap

We made some improvements to the order guidance for RBs when introducing virtual caps, this makes the guidance for everyone consistent.

<img src="/images/fe-providers/08-how-to-order-guidance.png"
     alt="Ordering guidance">

#### Check your details

Changes:
- heading from ‘Check your schools details’ to ‘Check your details’
- row heading  from ‘School type’ to ‘Setting’
- allocation description from ‘children in years 3 to 11’ to ‘students in year 3 or above’

For push change the description of ‘pupils unable to attend school’ to ‘students unable to take part in face-to-face education’ in guidance on when to request more devices.

<img src="/images/fe-providers/09-check-your-details.png"
     alt="Changes to ordering guidance">

#### Get help for specific circumstances

Changes:
- ‘children’ to ‘children or students’ in 2 places
- ‘cannot attend school – even though theirs is open’ to ‘cannot take part in face-to-face education – even though their school or college is open’

<img src="/images/fe-providers/10-specific-circumstances.png"
     alt="Changes to specific circumstances">

## Responsible bodies non-flow changes

### Homepage

Changes ’give schools access to the services they need’ to ‘give school and college staff access to this service and TechSource’.

<img src="/images/fe-providers/11-rb-homepage.png"
     alt="Changes to RBs homepage">

#### Get laptops and tablets

Adds ‘and/or colleges’ to ‘schools’.

Removes ‘for each school’ from ‘give contacts and technical information’.

Changes ‘cannot attend school because restrictions prevent them from going’ to ‘live in a different area to their school or college and are subject to local coronavirus restrictions’.

<img src="/images/fe-providers/12-get-laptops-and-tablets.png"
     alt="Changes to RBs homepage">

#### Your schools – pull

Adds ‘and/or colleges’ to ‘schools’

<img src="/images/fe-providers/13-your-schools--pull.png"
     alt="Changes to RBs homepage">

#### Your schools – push

Adds ‘and/or colleges’ to ‘schools’

<img src="/images/fe-providers/14-your-schools--push.png"
     alt="Changes to RBs homepage">

#### Order devices

Rewording of the ‘ordering devices for more than one school’ guidance to make it work for schools and colleges.

<img src="/images/fe-providers/15-order-devices.png"
     alt="Guidance on how to combine allocations into a single order">

#### Request devices for specific circumstances

Changes:
- all mentions of ‘children’ to ‘students’
- ‘cannot attend school – even though theirs is open – because they live in a different area with local coronavirus restrictions’ to ‘cannot take part in face-to-face education – even though their school or college is open – because they live in a different area with local coronavirus restrictions’

<img src="/images/fe-providers/16-request-for-specific-circumstances.png"
     alt="Changes to RBs homepage">
