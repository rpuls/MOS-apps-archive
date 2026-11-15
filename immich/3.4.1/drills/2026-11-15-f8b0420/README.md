# immich drill on f8b0420bec97

Pull request: [#355](https://github.com/rpuls/my-own-suite/pull/355)

On `f8b0420bec97`: `@update immich` passed, `@app-dr immich` passed.

#### `@update immich` passed

✓ reset · ✓ owner · ✓ drive · ✓ install:immich · ✓ app:immich · ✓ platform-update:wait · ✓ update:immich · ✓ verify:immich · ✓ routes · ✓ compare · ✓ network

- `app:immich`: ✓ register the admin and sign in · ✓ upload photos · ✓ its background jobs make previews · ✓ put them in an album · ✓ copy a photo onto the drive and plug it back in
- `verify:immich`: ✓ sign in · ✓ the photos, their files and the album are still there · ✓ the photo on the drive is still there

Screens that changed: immich/photos 0.1%.

##### Network: Problems

None.

##### Network: immich

Updated in `update:immich`: Before is everything until that step, After is from it on.

| Host | Channel | From | Steps | Before | After | In review |
| --- | --- | --- | --- | --- | --- | --- |
| `www.modelscope.cn` | server | immich-machine-learning | app:immich | ✓ |  | no, before the update only |
| `huggingface.co` | server | immich-machine-learning | app:immich | ✓ |  | yes |
| `cas-server.xethub.hf.co` | server | immich-machine-learning | app:immich | ✓ |  | yes |
| `us.aws.cdn.hf.co` | server | immich-machine-learning | app:immich | ✓ |  | yes |

New after the update: none.

#### `@app-dr immich` passed

✓ reset · ✓ owner · ✓ drive · ✓ install:immich · ✓ app:immich · ✓ backup:bucket · ✓ reset · ✓ owner · ✓ restore:bucket · ✓ verify:immich · ✓ routes · ✓ network · ✓ cleanup

- `app:immich`: ✓ register the admin and sign in · ✓ upload photos · ✓ its background jobs make previews · ✓ put them in an album · ✓ copy a photo onto the drive and plug it back in
- `verify:immich`: ✓ sign in · ✓ the photos, their files and the album are still there · ✓ the photo on the drive is still there

##### Network: Problems

None.

##### Network: immich

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `huggingface.co` | server | immich-machine-learning | app:immich | yes |
| `cas-server.xethub.hf.co` | server | immich-machine-learning | app:immich | yes |
| `us.aws.cdn.hf.co` | server | immich-machine-learning | app:immich | yes |

### update: before and after

![update: before and after](update/compare.png)
