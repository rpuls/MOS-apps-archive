# Network: @app-dr jellyfin

Server capture: on, from `local`. 4 of 4 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## jellyfin

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `repo.jellyfin.org` | server | app | app:jellyfin, reset, restore:bucket | yes |
| `nyc2.mirror.jellyfin.org` | server | app | app:jellyfin | yes |
| `www.gstatic.com` | browser | jellyfin.mos.lab | app:jellyfin, verify:jellyfin | yes |
| `api.themoviedb.org` | server | app | app:jellyfin | yes |
| `www.omdbapi.com` | server | app | app:jellyfin | yes |
| `nyc1.mirror.jellyfin.org` | server | app | reset, restore:bucket | yes |

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `cdn.jsdelivr.net` | browser | home.mos.lab | app:jellyfin, restore:bucket, verify:jellyfin |  |
