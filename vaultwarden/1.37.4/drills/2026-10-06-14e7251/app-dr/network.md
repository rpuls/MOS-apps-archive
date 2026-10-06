# Network: @app-dr vaultwarden

Server capture: on, from `local`. 3 of 3 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## vaultwarden

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `api.pwnedpasswords.com` | browser | vaultwarden.r37509511472.lab.my-demo-domain.site | app:vaultwarden, verify:vaultwarden | yes |

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `cdn.jsdelivr.net` | browser | home.r37509511472.lab.my-demo-domain.site, home.mos.lab | app:vaultwarden, restore:bucket, dns01, verify:vaultwarden |  |
