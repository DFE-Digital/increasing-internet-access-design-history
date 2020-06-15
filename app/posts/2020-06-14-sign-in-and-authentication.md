---
title: Sign in and authentication
description: Putting request forms behind a sign-in
date: 2020-06-11
---

In the [current prototype](/initial-designs), each form is open to the public, and for each request the user (a local authority or trust) will need to give their name, email and organisation.

Repeating the same details multiple times:
- makes filling out each form more difficult
- increases the likelihood of error (for example typos and inconsistent data)

## Hypothesis

If we put all forms behind a sign in, then we’ll know each user’s organisation, name and email address. We will have confirmed that their email address is a valid one (they will have verified it), and a user’s name and organisation will not need to be repeated.

## Who can sign up?

We don’t want to introduce any barriers to collecting the initial data.

If we keep sign up open, then all local authorities and trusts can quickly create accounts and give us their data.

Of course, anyone could sign up and give data. Once an account has been created, we should authorise that account somehow. This might mean that they can submit data and requests to us, but we won't act on them until the user is deemed to be an authorised one.

This would probably be represented as an internal state.

## How will we authorise a user?

- Check the email is valid
- Check if the email is one we recognise and have been in contact with before (for example in the devices service)
- Check if the email domain is from a suitable organisation, perhaps checking a whitelist
