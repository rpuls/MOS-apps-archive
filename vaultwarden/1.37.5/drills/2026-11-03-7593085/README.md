# vaultwarden drill on 7593085303b4

Pull request: [#348](https://github.com/rpuls/my-own-suite/pull/348)

On `7593085303b4`: `@update vaultwarden` passed, `@app-dr vaultwarden` passed.

#### `@update vaultwarden` passed

✓ reset · ✓ owner · ✓ dns01 · ✓ install:vaultwarden · ✓ app:vaultwarden · ✓ platform-update:wait · ✓ update:vaultwarden · ✓ verify:vaultwarden · ✓ routes · ✓ compare · ✓ network

- `app:vaultwarden`: ✓ create the vault account · ✓ save a login item
- `verify:vaultwarden`: ✓ sign in from a new device · ✓ the item still decrypts to what was saved

Screens that changed: vaultwarden/vault 5.8%.

##### Network: Problems

None.

##### Network: vaultwarden

Updated in `update:vaultwarden`: Before is everything until that step, After is from it on.

| Host | Channel | From | Steps | Before | After | In review |
| --- | --- | --- | --- | --- | --- | --- |
| `api.pwnedpasswords.com` | browser | vaultwarden.r41639891338.lab.my-demo-domain.site | app:vaultwarden, verify:vaultwarden | ✓ | ✓ | yes |

New after the update: none.

#### `@app-dr vaultwarden` passed

✓ reset · ✓ owner · ✓ dns01 · ✓ install:vaultwarden · ✓ app:vaultwarden · ✓ backup:bucket · ✓ reset · ✓ owner · ✓ restore:bucket · ✓ dns01 · ✓ verify:vaultwarden · ✓ routes · ✓ network · ✓ cleanup

- `app:vaultwarden`: ✓ create the vault account · ✓ save a login item
- `verify:vaultwarden`: ✓ sign in from a new device · ✓ the item still decrypts to what was saved

##### Network: Problems

None.

##### Network: vaultwarden

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `api.pwnedpasswords.com` | browser | vaultwarden.r41639891338.lab.my-demo-domain.site | app:vaultwarden, verify:vaultwarden | yes |

### update: before and after

![update: before and after](update/compare.png)
