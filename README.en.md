🇧🇷 [Português](README.md) | 🇺🇸 English

# Web app testing — Urban Routes

Sprint 3 project from the TripleTen QA Engineer program: testing the web interface of **Urban Routes**, a service that builds routes for different types of transport, with checklists, test cases and bug reports in Jira.

## Goal

Check whether the Urban Routes layout and logic follow the requirements: home screen, transport modes, map, fares, payment method, "Book" button and car booking.

## What was done

- **Layout checklist** (19 checks), tested on Google Chrome (800x600) and Firefox (1920x1080): initial form state, Personal mode, map and Casual fare.
- **Checklist for the "Payment method" and "Add card" windows** (27 checks): Number and Code fields, using equivalence partitioning and boundary values (for example: code 00, 01, 99 and 100; number with fewer and more than 12 digits).
- **Test cases for the "Book" button** (5 cases): combinations with and without driver's license, card and addresses.
- **Test cases for the car booking** (3 cases): booking, cancelling and not cancelling.
- **22 bug reports** logged in Jira, each linked to a failed check.

## Results

| Part | Total | Passed | Failed | Blocked |
|---|---|---|---|---|
| Layout checklist | 19 | 12 | 7 | 0 |
| Payment checklist | 27 | 16 | 11 | 0 |
| "Book" button test cases | 5 | 1 | 3 | 1 |
| Booking test cases | 3 | 1 | 1 | 1 |

### Examples of bugs found

- When a card is added, the interface does not show the last 4 digits of the number.
- The Code field accepts the invalid values 00 and 100.
- The Number field accepts more than 12 digits and symbols outside the requirements.
- The "Add" button stays enabled with an invalid number or code.
- Cancelling a booking does not work.
- The route on the map shows the wrong "From" and "To" address names.

All 22 reports are in [`BUGS.md`](BUGS.md) (in Portuguese), with steps to reproduce, expected result and actual result.

## Files

- [`checklists-e-casos-de-teste-urban-routes.xlsx`](checklists-e-casos-de-teste-urban-routes.xlsx): spreadsheet with four tabs (in Portuguese):
  1. Layout checklist
  2. Checklist for "Payment method" and "Add card"
  3. Test cases for the "Book" button
  4. Test cases for the rental (car booking)

  Each failed item has its bug report ID (S3-1 to S3-22).
- [`BUGS.md`](BUGS.md): the 22 bug reports copied from Jira, since the project's Jira is private.

## What I learned

- **User interface testing:** checking the layout and logic of a web interface across different browsers and resolutions, using checklists and test cases.
- **Bug tracking:** linking each failed check to its bug report, with steps to reproduce, expected result and actual result.
- **Jira:** logging and organizing the 22 bugs found.
- **Equivalence partitioning and boundary values:** applying test design techniques to real fields, such as card number and code.
