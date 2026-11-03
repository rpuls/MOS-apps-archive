# Network: @app-dr actual-budget

Server capture: on, from `local`. 4 of 4 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `cdn.jsdelivr.net` | browser | home.r41638540002.lab.my-demo-domain.site, home.mos.lab | app:actual-budget, restore:bucket, dns01, verify:actual-budget |  |
