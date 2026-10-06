# Network: @app-dr immich

Server capture: on, from `local`. 8 of 8 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## immich

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `huggingface.co` | server | immich-machine-learning | app:immich, backup:bucket | yes |
| `cas-server.xethub.hf.co` | server | immich-machine-learning | app:immich, backup:bucket | yes |
| `us.aws.cdn.hf.co` | server | immich-machine-learning | app:immich, backup:bucket | yes |
| `www.modelscope.cn` | server | immich-machine-learning | app:immich, backup:bucket | yes |
| `cdn-lfs-cn-1.modelscope.cn` | server | immich-machine-learning | app:immich | yes |

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `api.github.com` | server | mos-homepage | app:immich |  |
| `cdn.jsdelivr.net` | browser | home.mos.lab | app:immich, restore:bucket, verify:immich |  |
