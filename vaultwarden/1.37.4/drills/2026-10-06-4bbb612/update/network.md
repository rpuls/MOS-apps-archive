# Network: @update vaultwarden

Server capture: on, from `local`. 1 of 1 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## vaultwarden

Updated in `update:vaultwarden`: Before is everything until that step, After is from it on.

| Host | Channel | From | Steps | Before | After | In review |
| --- | --- | --- | --- | --- | --- | --- |
| `api.pwnedpasswords.com` | browser | vaultwarden.r37506725076.lab.my-demo-domain.site | app:vaultwarden | ✓ |  | yes |

New after the update: none.

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `cdn.jsdelivr.net` | browser | home.r37506725076.lab.my-demo-domain.site | app:vaultwarden, platform-update:wait |  |
