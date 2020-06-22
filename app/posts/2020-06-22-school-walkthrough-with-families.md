---
title: A walkthrough with families
description: How we might give access to someone
date: 2020-06-22
related:
  items:
  - text: Prototype
    href: https://increasing-access-prototype.herokuapp.com/schools
---

These designs are a very quick exploration of what questions we need to ask the family to check they:

* are eligible
* can connect to a BT wifi hotspot
* can otherwise get mobile data

This will likely be someone from a school, possibly a teacher, calling a family to walkthrough their options.

## The BT walkthrough is complex

The BT wifi questions are very technical and could prove difficult for whoever is conducting the call. Depending on the family’s technical ability, they might need to:

* explain how to look for a wifi network
* explain how to connect to a network
* troubleshoot when a network is low quality
* know how to do this on a variety of devices
* describe how to visit a URL to sign in
* know how to do that on a variety of browsers
* share usernames and passwords

In contrast, getting extra mobile data is a relatively simple data gathering exercise.

When the number of logins has been exhausted, we can default to a mobile data only journey.

### Reducing that complexity

In this walkthrough we attempt to design away some of the BT wifi complexity.

We:

* don’t give out a username and password until we know there’s a strong chance of success, meaning we don’t waste our limited supply of credentials
* automate the sending of a username and password, only revealing the details to the person conducting the call if necessary
* manage and track which credentials have been used ourselves, without depending on spreadsheets being shared around responsible bodies
* eliminate transcription errors when distributing the credentials
* check eligibility upfront and unambiguously

## Mobile data offer

The mobile data offer is a lot simpler, but there are some key design points to highlight.

We:

* ask which network they are on and fail fast if their network isn’t in the offer
* we check if they’re on Pay as you go only if a supported network does not have an offer for it’s Pay as you go customers
* when an offer is identified, we tell them what they are going to get
* we confirm with them over the phone that they are happy for us to share their details, then immediately request data

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Help someone get internet access",
      img: { src: "01-help-someone-get-internet-access.png" }
    }, {
      text: "Who are you about to talk to?",
      img: { src: "02-who-are-you-about-to-talk-to.png" }
    }, {
      text: "Are they ready?",
      img: { src: "03-are-they-ready.png" }
    }, {
      text: "Do they have broadband?",
      img: { src: "04-do-they-have-broadband.png" }
    }, {
      text: "Do they have a device?",
      img: { src: "05-do-they-have-a-device.png" }
    }, {
      text: "Can they connect to a BT wifi hotspot?",
      img: { src: "06-can-they-connect-to-a-BT-wifi-hotspot.png" }
    }, {
      text: "Can they connect from another room?",
      img: { src: "07-can-they-connect-from-another-room.png" }
    }, {
      text: "How do they want to get username and password?",
      img: { src: "08-how-do-they-want-to-get-username-and-password.png" }
    }, {
      text: "Confirm they got username and password",
      img: { src: "09-confirm-they-got-username-and-password.png" }
    }, {
      text: "Can they log in from BT Wifi?",
      img: { src: "10-can-they-log-in-from-BT-wifi.png" }
    }, {
      text: "Can they access the internet?",
      img: { src: "11-can-they-access-the-internet.png" }
    }, {
      text: "Success",
      img: { src: "12-success.png" }
    }, {
      text: "When no BT Wifi is available",
      img: { src: "13-when-no-bt-access-is-available.png" }
    }, {
      text: "What network are they on?",
      img: { src: "14-what-network-are-they-on.png" }
    }, {
      text: "Pay as you go or contract?",
      img: { src: "15-pay-as-you-go-or-contract.png" }
    }, {
      text: "Details of offer (if available)",
      img: { src: "16-details-of-offer.png" }
    }, {
      text: "What mobile number?",
      img: { src: "17-what-mobile-number.png" }
    }, {
      text: "Who is the account holder?",
      img: { src: "18-who-is-the-account-holder.png" }
    }, {
      text: "Can we send details to network?",
      img: { src: "19-can-we-send-details-to-network.png" }
    }, {
      text: "Success and what happens next",
      img: { src: "20-success-and-what-happens-next.png" }
    }]
}) }}
