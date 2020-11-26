---
title: Ordering devices through TechSource
description: An overview of the user journey through TechSource
date: 2020-08-05
related:
  items:
  - text: Video of journey
    href: https://www.youtube.com/watch?v=EfbMs7mqCV8
---

The following screenshots show a standard journey through TechSource, the Computacenter tool that schools and responsible bodies will use to order devices. The screenshots represent the Wave 1 journey – there will be some small differences for Wave 2.

See the notes for each screen.

There is also a [video guide](https://www.youtube.com/watch?v=EfbMs7mqCV8).

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Sign in",
      img: { src: "01-sign-in.png" },
      caption:"
Users are asked for a 'User ID', but should be signing in with their email address.
      "
    }, {
      text: "Home page",
      img: { src: "02-home-page.png" }
    }, {
      text: "Home page: Support",
      img: { src: "03-home-page-support.png" }
    }, {
      text: "Home page: Available bundles",
      img: { src: "04-home-page-available-bundles.png" }
    }, {
      text: "Bundle page",
      img: { src: "05-bundle-page.png" }
    }, {
      text: "Bundle page showing bundle contents",
      img: { src: "06-bundle-contents.png" }
    }, {
      text: "Add to basket",
      img: { src: "07-add-to-basket.png" }
    }, {
      text: "Continue or checkout",
      img: { src: "08-continue-or-checkout.png" }
    }, {
      text: "Another bundle page",
      img: { src: "09-another-bundle-page.png" }
    }, {
      text: "Microsoft laptop bundle page",
      img: { src: "10-microsoft-laptop-bundle-page.png" }
    }, {
      text: "Basket",
      img: { src: "11-basket.png" }
    }, {
      text: "Basket showing summary",
      img: { src: "12-basket-showing-summary.png" }
    }, {
      text: "Checkout",
      img: { src: "13-checkout.png" }
    }, {
      text: "Checkout: Payment details",
      img: { src: "14-checkout-payment-details.png" }
    }, {
      text: "Checkout: Google domain and recovery",
      img: { src: "15-checkout-google-domain-and-recovery.png" },
      caption: "
These are required fields if selecting Google or Apple devices. Note that the recovery field asks for different things – an email address or an organisation ID. It's not clear what happens if the user is buying both Apple and Google, but that might be unlikely.
      "
    }, {
      text: "Checkout: Delivery address",
      img: { src: "16-checkout-delivery-address.png" },
      caption: "
Delivery addresses are associated with the URN of the user. They cannot add a new delivery address. Their user may be associated with many schools, which will make finding addresses difficult. The hints/tips on the right suggests using 'ctrl+f' to find the right one. By default only the first 3 are shown.
      "
    },{
      text: "Checkout: See more addresses",
      img: { src: "18-checkout-see-more-addresses.png" },
      caption: "
Clicking 'see more addresses' reveals all the addresses.
      "
    }, {
      text: "Checkout: Delivery contact details",
      img: { src: "17-checkout-delivery-contact-details.png" }
    }, {
      text: "Checkout: Additional information",
      img: { src: "19-checkout-additional-information.png" },
      caption: "
The additional information fields are standard and can’t be removed. In reality they aren't being looked at, and users aren't encouraged to fill them in. The instructions should already be known. There are separate instructions in the support hub.
      "
    }, {
      text: "Checkout: Delivery method",
      img: { src: "20-checkout-delivery-method.png" },
      caption: "
While this shows 5 working days, for Wave 2 they will be delivered next working day if ordered before 4pm, or otherwise within 48 hours.
      "
    }, {
      text: "Checkout: Review and confirm",
      img: { src: "21-checkout-review-and-confirm.png" }
    }, {
      text: "Checkout: Review and confirm (scrolled)",
      img: { src: "22-checkout-review-and-confirm-2.png" }
    }, {
      text: "Checkout: Submit order button",
      img: { src: "23-checkout-submit-order.png" },
      caption: "
On submitting an order the user will see a flash screen confirming the order. No confirmation email is sent, but the 'delivery contact' will receive a despatch confirmation. Users can find their orders in the order history.
      "
    }, {
      text: "Order history",
      img: { src: "24-order-history.png" }
    }]
}) }}
