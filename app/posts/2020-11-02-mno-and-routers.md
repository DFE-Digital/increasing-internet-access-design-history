---
title: Routers and mobile data for schools
description: Exploring how these offers sit together
date: 2020-11-02
---

There are many pieces to this design puzzle, and getting them to fit neatly together is proving difficult.

## Design constraints

- Devices, routers and mobile data all have the same eligibility
- We want schools to compare the two connectivity offers and pick what’s best for each family
- We need to design and build something simple so we can ship the first version within a week

### Routers

We have a limited stock of routers leftover from Wave 1 of devices in the summer. More routers are on the way, but the type of routers, path to ordering, volume of stock and time until ready is unknown. Our process must be focussed only on the leftover Wave 1 stock for now.

Wave 1 routers will be ordered through Computacenter.

We do not know the need each school has for internet connectivity. We do not have enough data to estimate an allocation for each school. Each school starts with an allocation of zero, and must request routers if they need them. (We need to research ways of gathering this data through the service)

Right now we ask schools to request their routers when they become eligible to order devices, or earlier for specific circumstances.

We do not want to burn through our stock of routers immediately – promoting requests and making routers too prominent might mean we run out of stock long before we get our new routers. Considering the whereabouts of many of the original Wave 1 routers, is it safer to distribute them more slowly to those with a clearly defined need?

### Extra data for mobile devices

We will launch without all networks on board, as we go we hope to add more.

Networks are nervous about volumes of requests, even though uptake during the pilot was low. They may want to see that we are only giving data to those we know are eligible. Some networks will limit requests.

Our original feature was at the responsible body level, with very different eligibility criteria. Now it might be that a responsible body can only make requests when one or more of its schools are eligible too. Each request may also need to be attributed to a school, rather than just the responsible body.

### Devolve to schools or manage centrally

Responsible bodies chose whether to devolve device ordering to schools or to manage centrally, who should manage ordering of routers and requesting mobile data may be different.

If a school is devolved for some features but not others, that creates a complex product that’s difficult to design, build and iterate. For now we must assume that where device ordering was managed centrally, so too will routers and mobile data – even though we know that requesting mobile data works best at the school level.

### Timescales

Except for specific circumstances, these offers will be made available when a school reports disruption (self-isolating year groups, closure, etc). For groups who are self-isolating, isolation is typically for a couple of weeks.

Given the following steps, it’s reasonable to expect that support may only arrive after isolation has finished:

Once the features are activated (ie from day 2), for routers schools need to:

- determine how many children without internet access need routers
- request those routers from DfE along with evidence
- wait for those requests to be approved by DfE (eg 3 days)
- order routers through Computacenter and await delivery (eg 5 days)
- receive routers and distribute to families (later they can collect and redistribute these devices)

For mobile data requests, schools need to:

- determine how many children without internet access need extra mobile data
- collect name, number, network and permission from each family
- enter data into the Get help with technology service
- wait until networks receive, process and approve the request (eg 2 to 5 days)

### Eligibility

All offers have the same eligibility. We do not want to overly repeat that eligibility throughout the service.

### School order states

The service has 4 states a school can be in:

- cannot order devices yet
- can order devices for specific circumstances
- can order full allocation of devices
- school reopened (can no longer order devices)

These states map well for ordering routers, but not necessarily for requesting mobile data.

Consider a request for mobile data for a child that’s shielding. Ideally we would use the "can order devices for specific circumstances" state to enable requests for mobile data. But that would also change how the "Order devices" screens look – if no devices were requested they would say "Order 0 of X devices for specific circumstances".
