---
title: See your Huawei router password
description: Users will need to reset their 4G routers before 16 July 2021. To do this, they’ll need their password.
date: 2021-05-07
related:
  items: 
  - text: Trello ticket — Allow users to retrieve passwords for huawei routers
    href: https://trello.com/c/xyQMVKQB/1963-allow-users-to-retrieve-passwords-for-huawei-routers
---

If user do not reset their Huawei routers, they will not be able to use it after 31 July 2021. To reset the Huawei routers, the user needs a password. The password is the same for all routers provided by DfE, but not widely available.

To share the password with users but keep it relatively secure, we’ve added a page in the signed-in part of the service to show user’s their Huawei router password.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "School home",
      img: { src: "01-school-home.png" }
    }, {
      text: "Router home",
      img: { src: "02-router-home.png" }
    }, {
      text: "Internet home",
      img: { src: "03-internet-home.png" }
    }, {
      text: "Router password",
      img: { src: "04-router-password.png" }
    }]
}) }}
