---
title: Devolving devices – Iteration
description: Changes to the responsible body journey
date: 2020-08-15
---

Following research on the [original design](/devolving-device-orders-to-schools), we made some changes.

## Fixing a broken journey

The journey from "Get devices" through to the schools list had a number of issues that research participants kept tripping up on.

### It wasn’t clear when the journey ended

People would make their decision on how to devolve to schools, get to the schools list and ask "what happens next?".

In this new design the first screens – [giving guidance](#tell-us-who-will-order), [choosing a default](#who-will-order), and a new ‘[what's next screen](each-school-will-order)’, have been reshaped as their own 3-step process.

After choosing a default, the user is told their changes have been saved and is instructed what to do next.

The next steps are clearer, and when proceeding to the schools list it is now a new journey – one of setting the specifics for each school. The schools list is no longer perceived as a dead end, but a place to come and go from as details are completed.

### Set a default, then edit individual schools

[There were 3 states](/devolving-device-orders-to-schools/#who-will-order-devices-some-schools-selected), each leading to slightly different designs of the schools list and school pages:

1. All schools devolved
2. Some managed centrally
3. All managed centrally

After making a choice, it wasn’t clear if that choice could be changed later. And if it could, what would happen. This mattered because it affected the layouts and forms of the subsequent pages.

"All managed centrally" previously took users to a list of responsible body accounts. For anyone who selected this option, they could not see a list of schools. It was updated to also take users to the list of schools, while [management of accounts was promoted to the index page](/managing-responsible-body-users).

The schools list and school pages have been simplified to show the same table and design no matter what choice was made. This means the overall setting now acts not as a switch, but as a default for all schools, a default that can then be edited at the school level – for any exceptions to the rule.

With a default and per–school editing, we could also remove the ‘Some managed centrally’ option.

### Users needed more context following Wave 1

In Wave 1 allocations were per responsible body, devices were sometimes delivered to responsible bodies and devices could be ordered immediately.

In research we found that:
- users were misinterpreting the GOV.UK announcement
- users were not given enough context about what had changed compared to Wave 1

They were frequently coming to the wrong conclusions about Wave 2.

We updated the in-service guidance based on questions participants asked. The guidance now:
- indicates that schools can now order devices
- is explicit about recommending that schools be the ones to order devices
- indicates that allocations are per school and that the allocations will change depending on future outbreaks

### Fixing school statuses

There were two statuses:
- not started
- completed

Not started was fairly obvious, but what did "completed" mean, specifically – what had been completed.

For devolved schools we need contact details.

For centrally managed schools we need to know some specific technical information regarding Google Chromebooks, if the school intends to order them. (For devolved schools we’ll ask for the same information, but the schools will enter those details themselves).

We refined the statuses to be:
- needs a contact (for schools who need to order themselves)
- school contacted (once a contact has been added)
- needs information (for schools a local authority will order for)
- ready (once all missing information has been added)

### Adding headteachers as a default choice

Users told us that they’d often give the headteacher as the main contact. This was especially true for primary schools, which make up the majority of any schools list.

We have all the contact details for headteachers, so rather than asking them to find and fill each one out – we instead let them select the headteacher, showing them the name and email address we have.

## Other design changes

Design changes also include:
- a first pass at adding the Chromebook information for each centrally managed school
- adding a filter to the schools so users can find the schools they need to
- indicating allocation numbers in the schools table
- indicating school types in the table (Primary, Secondary, Special school)
- giving a link to support for responsible bodies querying the schools list

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "Signed in home page",
      img: { src: "01-signed-in-home-page.png" }
    }, {
      text: "Tell us who will order",
      img: { src: "02-tell-us-who-will-order.png" }
    }, {
      text: "Who will order",
      img: { src: "03-who-will-order.png" }
    }, {
      text: "Each school will order",
      img: { src: "04-each-school-will-order.png" }
    }, {
      text: "All orders managed centrally",
      img: { src: "05-all-orders-managed-centrally.png" }
    }, {
      text: "Schools list",
      img: { src: "06-schools-list.png" }
    }, {
      text: "Is a school missing?",
      img: { src: "07-is-a-school-missing.png" }
    }, {
      text: "School: Local authority ordering",
      img: { src: "08-school-local-authority-ordering.png" }
    }, {
      text: "School: School ordering",
      img: { src: "09-school-school-ordering.png" }
    }, {
      text: "School: Changes saved",
      img: { src: "10-changes-saved.png" }
    }, {
      text: "School: Edit who will order devices",
      img: { src: "11-edit-who-will-order-devices.png" }
    }, {
      text: "School: Edit Chromebook details",
      img: { src: "12-edit-chromebook-details.png" }
    }, {
      text: "School: Edit contact details",
      img: { src: "13-edit-contact-details.png" }
    }, {
      text: "School: Saved after adding a contact",
      img: { src: "14-saved-after-adding-a-contact.png" }
    }, {
      text: "Example school statuses after completing details",
      img: { src: "15-example-school-statuses.png" }
    }]
}) }}
