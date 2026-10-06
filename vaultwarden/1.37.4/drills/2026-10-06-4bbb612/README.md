# vaultwarden drill on 4bbb6124f203

Pull request: [#317](https://github.com/rpuls/my-own-suite/pull/317)

On `4bbb6124f203`: `@update vaultwarden` failed at `update:vaultwarden`, `@app-dr vaultwarden` passed.

#### `@update vaultwarden` failed at `update:vaultwarden`

✓ reset · ✓ owner · ✓ dns01 · ✓ install:vaultwarden · ✓ app:vaultwarden · ✓ platform-update:wait · ✗ update:vaultwarden

```text
Error: vaultwarden is offered no update (catalog status not-in-catalog, installed 0.4.1).
```

##### Network: Problems

None.

##### Network: vaultwarden

Updated in `update:vaultwarden`: Before is everything until that step, After is from it on.

| Host | Channel | From | Steps | Before | After | In review |
| --- | --- | --- | --- | --- | --- | --- |
| `api.pwnedpasswords.com` | browser | vaultwarden.r37506725076.lab.my-demo-domain.site | app:vaultwarden | ✓ |  | yes |

New after the update: none.

#### `@app-dr vaultwarden` passed

✓ reset · ✓ owner · ✓ dns01 · ✓ install:vaultwarden · ✓ app:vaultwarden · ✓ backup:bucket · ✓ reset · ✓ owner · ✓ restore:bucket · ✓ dns01 · ✓ verify:vaultwarden · ✓ routes · ✓ network · ✓ cleanup

##### Network: Problems

None.

##### Network: vaultwarden

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `api.pwnedpasswords.com` | browser | vaultwarden.r37506725076.lab.my-demo-domain.site | app:vaultwarden, verify:vaultwarden | yes |
