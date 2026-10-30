# Network: @update paperless-ngx

Server capture: on, from `local`. 4 of 4 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `api.github.com` | server | mos-homepage | app:paperless-ngx |  |
| `cdn.jsdelivr.net` | browser | home.mos.lab | app:paperless-ngx, platform-update:wait, verify:paperless-ngx |  |
