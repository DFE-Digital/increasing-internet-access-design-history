---
title: Service performance
description: Dashboards showing device, MNO and router stats
date: 2021-03-10
---

Changes from current dashboard include:

- a single table for all MNO requests
- MNO request status breakdown for each network
- tabs for devices, service and routers
- showing absolute numbers and percentages
- focuses more on what's been ordered and what's left, rather than how an RB or school is configured

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Service dashboard",
      img: { src: "01-service-dashboard.png" }
    }, {
      text: "Devices",
      img: { src: "02-devices.png" }
    }, {
      text: "Mno",
      img: { src: "03-mno.png" }
    }, {
      text: "Routers",
      img: { src: "04-routers.png" }
    }]
}) }}
