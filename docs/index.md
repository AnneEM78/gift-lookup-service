# GiftTrackr API

## Overview

### GiftTrackr—Gift Smart

Ever bought a birthday gift for someone, given it to them—and realized as they're opening it that you've already given them that gift?! So embarrassing—and so preventable.

If you've got a lot of friends and family to buy gifts for, you've definitely seen this more than once. But who has the time to keep track of everything? Excel files and paper lists—none of them are convenient.

Now there's GiftTrackr, an easy-to-install API that lets users keep track of gift history, and avoid repeating gifts. GiftTrackr's API can be integrated with calendar apps, shopping list apps, address books, and more.

Giftrackr uses two resources: recipients and gifts.

With GiftTrackr, you can do the following and more:

- [Add gifts to the system](api/create_gift.md)

- [Add recipient info](api/create_recipient.md)

- [Retrieve gifts by gift name](api/read_gift_by_title.md)

- [Retrieve recipients by birthdate](api/read_recipient_by_birthdate.md)

## Quickstart

[Click here for the quickstart guide on getting your system ready](quickstart.md)

## Tutorials

Once your system is ready, these tutorials show you how to perform common tasks.

- [Add a recipient](tutorials/add_a_recipient.md)
- [Add a gift](tutorials/add_a_gift.md)

## API reference docs

The API reference docs refer to a {server_url} when they refer to the URL of a resource. The {server_url} value depends on the installation of the service. When running a local test, the {server_url} is generally `http://localhost:3000`.

CREATE (POST)

- [Create gift](api/create_gift.md)
- [Create recipient](api/create_recipient.md)

DELETE

- [Delete gift](api/delete_gift.md)
- [Delete recipient](api/delete_recipient.md)

READ (GET)

- [Read gift by title](api/read_gift_by_title.md)
- [Read recipient by birthdate](api/read_recipient_by_birthdate.md)
- [Read recipient by first name](api/read_recipient_by_first_name.md)

UPDATE (PUT/PATCH)

- [Update recipient](api/update_recipient.md)
- [Update gift](api/update_gift.md)

## Related information

- [Handling errors](handling_errors.md)

Note: This is a mock API meant to simulate the REST interface of an imaginary service.
