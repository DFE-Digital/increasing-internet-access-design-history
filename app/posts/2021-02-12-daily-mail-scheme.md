---
title: Opting in to the Daily Mail’s donated devices scheme
description: How schools and responsible bodies will get these donated devices delivered to them
date: 2021-02-12
related:
  items:
  - text: School journey in prototype
    href: https://ghwt-prototype.herokuapp.com/school/donated
  - text: Trust journey in prototype
    href: https://ghwt-prototype.herokuapp.com/responsible-body/donated
  - text: Trello
    href: https://trello.com/c/vRo4CKNy
  - text: Prototype PR
    href: https://github.com/DFE-Digital/get-help-with-tech-prototype/pull/39
---

The Daily Mail is running a Computers For Kids scheme through its Mail Force charity. They are collecting donations for new devices and donations of old devices that will be refurbished.

The Department for Education is using its Get help with technology service as a way for schools and trusts to opt in and receive these devices. It must be clear that this is not a DfE scheme, and that our role in the distribution and allocation of these devices is minimal.

There are two journeys:

- school journey
- responsible body (RB) journey, where schools are being managed centrally

## Design notes

### No opt out

Schools can opt in, but there is no explicit opt out. If any school is not interested, we do not record that decision. If they return to this section of the service again they go through the same journey.

### Opting in some schools

For RBs there's a shortcut to opt in all schools, rather than having to select each one individually.

If an RB chooses to opt in only some of its schools, it can return and opt in the rest later. Those schools will have the same number of devices per school and accepted devices as the others.

### Delivery contact

The user that opts in a school will be the delivery contact. Their name, email address and telephone number will be shared with Computacenter and Mail Force. Their name will be shown on the delivery address.

We indicate this by showing their name and address on the Your details will be shared page. For an RB we should show the address of the first opted in school.

### Delivery

All deliveries must go to the school, they cannot be delivered centrally. They go to the address associated with the URN. We indicate the delivery address but it is not editable.

### Device types for responsible bodies

Research with trusts did not reveal a need for responsible bodies to independently set the device types needed at a school level. In the design the devices accepted apply to all schools. This simplifies the journey, especially for those RBs with many schools.

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  items: [{
      text: "School: Home page",
      img: { src: "01-school-home-page.png" },
      caption: "
There’s a new section linking to opting in
      "
    }, {
      text: "School: Do you want donated devices?",
      img: { src: "02-school-do-you-want-donated-devices.png" }
    }, {
      text: "School: No, not interested",
      img: { src: "03-school-no-not-interested.png" }
    }, {
      text: "School: Yes interested, About devices",
      img: { src: "04-school-yes-interested-about-devices.png" }
    }, {
      text: "School: There’s a queue for devices",
      img: { src: "05-school-theres-a-queue-for-devices.png" }
    }, {
      text: "School: Still interested?",
      img: { src: "06-school-still-interested.png" }
    }, {
      text: "School: Which devices?",
      img: { src: "07-school-which-devices.png" }
    }, {
      text: "School: How many devices?",
      img: { src: "08-school-how-many-devices.png" }
    }, {
      text: "School: Your details will be shared",
      img: { src: "09-school-your-details-shared.png" }
    }, {
      text: "School: Disclaimer",
      img: { src: "10-school-disclaimer.png" }
    }, {
      text: "School: Check answers",
      img: { src: "11-school-check-answers.png" }
    }, {
      text: "School: Confirmation",
      img: { src: "12-school-opted-in.png" }
    }, {
      text: "School: Updated home page after opting in",
      img: { src: "13-school-updated-home-page.png" }
    }, {
      text: "Responsible body: Home page",
      img: { src: "14-responsible-body-home-page.png" }
    }, {
      text: "Responsible body: Get laptops and tablets",
      img: { src: "15-responsible-body-get-laptops-and-tablets.png" }
    }, {
      text: "Responsible body: Do you want donated devices?",
      img: { src: "16-responsible-body-do-you-want-donated-devices.png" }
    }, {
      text: "Responsible body: No, not interested",
      img: { src: "17-responsible-body-no-not-interested.png" }
    }, {
      text: "Responsible body: Yes interested, About devices",
      img: { src: "18-responsible-body-yes-interested-about-devices.png" }
    }, {
      text: "Responsible body: There’s a queue for devices",
      img: { src: "19-responsible-body-theres-a-queue-for-devices.png" }
    }, {
      text: "Responsible body: Still interested?",
      img: { src: "20-responsible-body-still-interested.png" }
    }, {
      text: "Responsible body: Opt in all or some schools?",
      img: { src: "21-responsible-body-opt-in-all-or-some-schools.png" }
    }, {
      text: "Responsible body: Pick which schools",
      img: { src: "22-responsible-body-pick-which-schools.png" }
    }, {
      text: "Responsible body: Which devices?",
      img: { src: "23-responsible-body-which-devices.png" }
    }, {
      text: "Responsible body: How many devices?",
      img: { src: "24-responsible-body-how-many-devices.png" }
    }, {
      text: "Responsible body: Your details will be shared",
      img: { src: "25-responsible-body-your-details-shared.png" }
    }, {
      text: "Responsible body: Disclaimer",
      img: { src: "26-responsible-body-disclaimer.png" }
    }, {
      text: "Responsible body: Check answers (some schools)",
      img: { src: "27-responsible-body-check-answers-some-schools.png" }
    }, {
      text: "Responsible body: Confirmation (some schools)",
      img: { src: "28-responsible-body-opted-some-in.png" }
    }, {
      text: "Responsible body: Check answers (all schools)",
      img: { src: "29-responsible-body-check-answers-all-schools.png" }
    }, {
      text: "Responsible body: Confirmation (all schools)",
      img: { src: "30-responsible-body-opted-all-in.png" }
    }]
}) }}
