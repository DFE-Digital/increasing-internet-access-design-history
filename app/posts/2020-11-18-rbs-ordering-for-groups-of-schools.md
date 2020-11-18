---
title: Responsible bodies ordering for groups of schools
description: Allow ordering for multiple schools (virtual caps)
date: 2020-11-18
related:
  items:
  - text: "Trello: Virtual caps epic"
    href: https://trello.com/c/Blj9SZ65/1007-virtual-cap
---

## The problem

Many trusts and some local authorities have chosen to manage the ordering of devices centrally on behalf of their schools. Some of these responsible bodies will place an order for each school, and ship those devices directly to the school. But for others it’s more complicated.

Consider a multi-academy trust with a central IT function – these trusts need to ship all devices to a single location (for example a specific school) where they can be prepared before they reach schools. These trusts are placing 1 order for multiple schools.

Orders that don’t meet certain criteria end up in a manual queue that Computacenter has to process. About 25% of orders are ending up in this queue – this slows down ordering and can lead to orders being cancelled.

Ordering more devices to a school than that specific school is allowed will always end up in the manual queue.

We can pool schools together to create a virtual limit to fix these issues.

### Worked example

A trust manages orders for:

| School | Devices they can order | Limit on TechSource |
|--|--|--|
| School A | 25 | 25 |
| School B | 50 | 50 |
| School C | 10 | 10 |

All the schools are eligible to order.

The trust places an order for 85 devices to be delivered to school B. Because 85 is more than 50, TechSource flags the order for manual processing.

## Pooling schools together (also referred to as virtual caps)

With a pool the idea is to take the total of all devices available for eligible schools and to make that the limit for all schools. When an order is made the overall total will then reduce.

As a single pool, a trust can order 85 devices (25 + 50 + 10).

| School | Devices they can order | Limit on TechSource |
|--|--|--|
| School A | 25 | 85 |
| School B | 50 | 85 |
| School C | 10 | 85 |
| Total (pool) | 85 | |

Now when an order of 75 devices is placed against school B, 75 is smaller than 85 so TechSource automatically approves the order. They then report back how many have been ordered using an API call to the DfE service.

After ordering we update the limits on TechSource

| School | Devices they can order | Devices ordered | Limit on TechSource |
|--|--|--|--|
| School A | 25 | Unknown | 10 |
| School B | 50 | Unknown | 10 |
| School C | 10 | Unknown | 10 |
| Total (pool) | 85 | 75 | |

This means that the trust can still place an order for 10 more devices and that order will be automatically approved.

## Limits to a pool of schools

When a responsible body orders its devices we cannot know which schools they are destined for. This has the following effect:

- we do not know if any given school has had devices ordered for it
- we cannot remove a school from a pool (ie when they reopen) as we do not know the number of devices left in the pool because we do not know what proportion of their devices were ordered
- if the order is for Chromebooks, and if the schools have different Chromebook domains, we will not know which domains to use and in what proportion

## Design changes

Our [current design](/ordering-devices-centrally/#order-devices-now) recommends placing an order for each school, and we list the schools they need to order for. Orders could also be placed [from each school page](/order-from-schools-page/).

We have removed ordering from a school page – because we do not accurately know the numbers per school, we need to defer to a central place for ordering.

We’ve replaced the table of schools with a panel showing the total number of devices that can be ordered across all schools. By removing the table we also remove links to each school – which was a source of error in the old design, with users sometimes heading down that route to try and order devices.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Order devices",
      img: { src: "01-order-devices.png" }
    }, {
      text: "Simplified school page",
      img: { src: "02-simplified-school-page.png" },
      caption: "
The order panel and order page have been removed
      "
    }, {
      text: "Simplified schools list",
      img: { src: "03-simplified-schools-list.png" },
      caption: "
'Get schools ready' and '17 schools' has been consolidated into a single title
      "
    }, {
      text: "Get laptops and tablets",
      img: { src: "04-get-laptops-and-tablets.png" },
      caption: "
Title updated from 'Get schools ready' and an updated 'use this section' list
      "
    }]
}) }}
