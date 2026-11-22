# Network: @update stirling-pdf

Server capture: on, from `local`. 2 of 2 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## stirling-pdf

Updated in `update:stirling-pdf`: Before is everything until that step, After is from it on.

| Host | Channel | From | Steps | Before | After | In review |
| --- | --- | --- | --- | --- | --- | --- |
| `api.iconify.design` | browser | stirling-pdf.mos.lab | app:stirling-pdf | ✓ |  | no, before the update only |

New after the update: none.

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `cdn.jsdelivr.net` | browser | home.mos.lab | app:stirling-pdf, platform-update:wait, verify:stirling-pdf |  |
