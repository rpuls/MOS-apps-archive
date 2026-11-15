# Network: @update immich

Server capture: on, from `local`. 13 of 13 app containers showed their control lookup and connection.
Browser capture: on.

The server capture records every DNS lookup an app container makes and every connection it opens to a public address; the browser capture records every request to a host outside the suite. Neither decrypts traffic, and both see only what this run made the apps do.

## Problems

None.

## immich

Updated in `update:immich`: Before is everything until that step, After is from it on.

| Host | Channel | From | Steps | Before | After | In review |
| --- | --- | --- | --- | --- | --- | --- |
| `www.modelscope.cn` | server | immich-machine-learning | app:immich | ✓ |  | no, before the update only |
| `huggingface.co` | server | immich-machine-learning | app:immich | ✓ |  | yes |
| `cas-server.xethub.hf.co` | server | immich-machine-learning | app:immich | ✓ |  | yes |
| `us.aws.cdn.hf.co` | server | immich-machine-learning | app:immich | ✓ |  | yes |

New after the update: none.

## Platform (not checked against a review)

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `cdn.jsdelivr.net` | browser | home.mos.lab | app:immich, platform-update:wait, verify:immich |  |
