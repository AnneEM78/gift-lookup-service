# GiftTrackr API

## Overview

### GiftTracker—Gift Smart

Ever bought a gift for someone, given it to them—and realized as they're opening it that you've already given them that gift?! So embarrassing—and so preventable.

If you've got a lot of friends and family to buy gifts for, you've definitely seen this more than once. But who has the time to keep track of everything? Excel files, paper lists—none of it's convenient.

Now there's GiftTrackr, an easy-to-install API that lets users keep track of gift history, and avoid repeating gifts. GiftTrackr's API can be integrated with calendar apps, shopping list apps, address books, and more.

There are two resources, recipients and gifts.

With GiftTrackr, you can:

- [Create a list of all gifts you've entered, the receipients, and the dates given](api/read_all_gift_info.md)—or [get lists of gifts by recipient](api/read_gift_by_recipient.md)

- [Retrieve gifts by gift name](api/read_gift_by_title.md)

- [Retrieve recipients by birthdate](api/read_recipient_by_birthdate.md)

## Quickstart

[Click here for the quickstart guide](quickstart.md)

## Tutorials

Learn how to do common tasks within the GiftTrackr service.

After your system is ready, these tutorials show you how to perform common tasks.

### Recipients

- [Add a recipient](tutorials/add_a_recipient.md)
- Get a list of recipients
- Edit recipient info

### Gifts

- Add a gift

## API reference docs

The API reference docs refer to a {server_url} when they refer to the URL of a resource. The {server_url} value depends on the installation of the service. When running a local test, the {server_url} is generally `http://localhost:3000`.

CREATE (POST)

- [CREATE gift](api/create_gift.md)
- [CREATE recipient](api/create_recipient.md)

DELETE

- [DELETE gift](api/delete_gift.md)
- [DELETE recipient](api/delete_recipient.md)

READ (GET)

- [READ all gift info](api/read_all_gift_info.md)
- [READ gift by recipient](api/read_gift_by_recipient.md)
- [READ gift by title](api/read_gift_by_title.md)
- [READ recipient by first name](api/read_recipient_by_first_name.md)
- [READ recipient by birthdate](api/read_recipient_by_birthdate.md)

UPDATE (PUT/PATCH)

- [UPDATE recipient](api/update_recipient.md)
- [UPDATE gift](api/update_gift.md)

## Related information

- [Handling errors](handling_errors.md)
