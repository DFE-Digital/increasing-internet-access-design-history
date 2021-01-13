---
title: Let networks bulk update MNO requests
description: Networks are currently limited to 20 at a time
date: 2021-01-13
related:
  items:
  - text: Prototype PR
    href: https://github.com/DFE-Digital/get-help-with-tech-prototype/pull/34
  - text: Miro board from co-design session
    href: https://miro.com/app/board/o9J_lZbcRsg=/
  - text: CSV upload Trello ticket
    href: https://trello.com/c/w80Ydy7m/1288-mno-bulk-allow-mno-users-to-upload-a-csv-of-requests-to-update-their-statuses
  - text: Find multiple requests Trello ticket
    href: https://trello.com/c/gQk4sysp/1289-mno-bulk-add-feature-to-search-for-multiple-requests
---

Mobile networks can sign in, download requests as a CSV and manually update requests. They update requests by selecting them in the table and then use the form at the bottom to change their status. Requests are limited to 20 per page, so a maximum of 20 at a time can be processed. Or they report a problem. [Reporting a problem must be done 1 at a time on its own page](/pilot-launch/#mno-report-a-problem-form).

These designs work for low volumes, but now with hundreds of requests coming in the networks need new features to stay on top of them.

We ran a [co-design session with networks](https://miro.com/app/board/o9J_lZbcRsg=/) to explore what’s working, what’s not and how we can best fix these issues.

Findings can be broken down into:

- [small improvements we can ship quickly](#small-improvements-to-our-current-features)
- [bulk updating using a CSV](#csv-upload)
- [finding requests to update them](#find-requests-feature)
- [showing requests by status](#requests-by-status)

## Small improvements to our current features

We identified that 20 requests per page is not enough and [increased them to 100](https://github.com/DFE-Digital/get-help-with-tech/pull/1104).

In the list of statuses you can update, we’ve suggested showing all the problem states too, so they can be handled in bulk.

{% from "figure/macro.njk" import appFigure with context %}
{{ appFigure({
  image: {
    file: "08-updating-list-of-statuses.png"
  }
}) }}

We should remove error types that aren’t being used:

- No longer on the network, "we would use no account found"
- No account with that name, "we are flexible with names"
- Not a valid mobile number, should be handled by validation

## CSV upload

Networks strongly supported the idea of updating requests by uploading a CSV. It would be the same CSV as the one they download from the service, only modified with new statuses.

For networks who are automating updates internally, they can automate the CSV update too and then the only manual task left is uploading the CSV.

Technical notes, the CSV upload should:
- be idempotent (you should be able to upload the same file multiple times)
- should _probably_ ignore requests that have a newer last updated date in the database than shown in the CSV
- the CSV download should incorporate different problem types as their own statuses (much like the form has been updated) – this means users only need to update 1 column rather than 2

{% from "screenshots/macro.njk" import appScreenshots with context %}
{{ appScreenshots({
  hideContents: true,
  items: [{
      text: "Current design with link to upload CSV",
      img: { src: "01-current-design-with-link-to-upload-csv.png" }
    }, {
      text: "Upload CSV",
      img: { src: "02-upload-csv.png" }
    }, {
      text: "CSV uploaded",
      img: { src: "03-csv-uploaded.png" }
    }]
}) }}

## Find requests feature

This feature was designed before the session and was demoed to the networks. It was thought by us that a CSV upload might be too technical and this was presented first – conversations naturally led to the idea of a CSV upload as an alternative.

Some networks thought the feature would be useful, especially if numbers could be pasted from a spreadsheet. It is still a very manual process, and a CSV upload was preferable.

{{ appScreenshots({
  hideContents: true,
  items: [{
      text: "Find requests feature",
      img: { src: "04-find-requests-feature.png" }
    }, {
      text: "Requests found",
      img: { src: "05-requests-found.png" }
    }]
}) }}

## Requests by status

We also demoed a design that shows requests by status. Networks noted that this would be useful, but there was little feedback. Downloading only certain types of request in a CSV was considered the most useful.

{{ appScreenshots({
  hideContents: true,
  items: [{
      text: "Request by status feature",
      img: { src: "06-request-by-status-feature.png" }
    }, {
      text: "Example completed requests page",
      img: { src: "07-example-completed-requests-page.png" }
    }]
}) }}
