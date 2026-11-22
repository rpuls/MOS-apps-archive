# Network: @app-dr stirling-pdf

Server capture: on, from `local`. 3 of 3 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `api.github.com` | server | mos-homepage | app:stirling-pdf |  |
| `cdn.jsdelivr.net` | browser | home.mos.lab | app:stirling-pdf, restore:bucket, verify:stirling-pdf |  |
