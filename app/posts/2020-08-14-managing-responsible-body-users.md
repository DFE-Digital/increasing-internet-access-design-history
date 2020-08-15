---
title: Managing responsible body users
description: Separate the management of users from the devices journey
date: 2020-08-14
---

As part of the [iteration of the "devolve to schools" journey](/devolving-devices-iteration), we split out the management of responsible body users into its own section on the index page.

It was initially called "Manage users", but research participants frequently misinterpreted this as being the place to add school users. It was renamed to "Manage local authority users" to avoid that confusion.

Every user can add or edit any other user.

Not all users need to have a corresponding TechSource account (for example senior users who want oversight but aren’t going to be ordering anything). When adding a user, you can decide if the new user should have access to TechSource.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Signed in home page",
      img: { src: "01-signed-in-home-page.png" }
    }, {
      text: "Manage local authority users",
      img: { src: "02-manage-local-authority-users.png" }
    }, {
      text: "Invite a new user",
      img: { src: "03-invite-a-new-user.png" }
    }]
}) }}
