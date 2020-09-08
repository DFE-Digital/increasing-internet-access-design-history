---
title: What responsible bodies do for schools with no allocation
description: What changes for schools with a 0 device allocation
date: 2020-09-08
---

Some schools haven’t got an allocation of devices. Responsible bodies have been asking why.

## Reasons for no allocation

Reasons for a 0 allocation can include:
- the school has no children in the eligible year groups, years 3 to 10
- there are very few children on free school meals according to the most recent census data
- there was not sufficient data to calculate an allocation – for example it’s a new school

## What schools with no allocation can do

Schools and responsible bodies can still request devices for specific circumstances (shielding, etc). If they request devices and order them, we will need to know Chromebook details.

Individual schools may also be eligible for future offers, such as connectivity offers or 4G routers. Having their contact details will help us get those offers directly to them.

## How we approach approving device requests affects our design

When a school requests devices we could:
- check which parts of the country recommend shielding, and only permit requests in those areas
- treat each request as a case-by-case basis, and on recommendation from a medical professional, permit requests anywhere

If our approvals are strictly geography based, it would greatly limit any 0 allocation schools from getting devices – it would make little sense to devolve to them and bring contacts onto the schools service.

However, if our approvals are more permissive, and geography is only a minor factor, then schools from everywhere will be receiving devices for specific circumstances, and we’ll want 0 allocation schools to be included.

## Design notes

Erring on the side of permissive device approvals, we’ve opted to continue to bring schools onboard. These schools will also benefit from future connectivity offers.

This makes the changes to the responsible body journey minor – we only need to add a guidance section for schools with no allocation.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Schools with no allocation needing details",
      img: { src: "01-schools-with-no-allocation-needing-details.png" }
    }, {
      text: "School with no allocation details given",
      img: { src: "02-school-with-no-allocation-details-given.png" }
    }, {
      text: "Early design",
      img: { src: "03-early-design.png" },
      caption: "
This is an earlier design, more suited for restrictive device approvals. In this design all 0 allocation schools would have been managed centrally, and we’d treat them differently with a 'No allocation' status.
      "
    }]
}) }}
