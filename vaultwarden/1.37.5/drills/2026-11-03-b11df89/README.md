# vaultwarden drill on b11df8938371

Pull request: [#348](https://github.com/rpuls/my-own-suite/pull/348)

On `b11df8938371`: `@update vaultwarden` failed at `verify:vaultwarden`, `@app-dr vaultwarden` failed at `app:vaultwarden`.

#### `@update vaultwarden` failed at `verify:vaultwarden`

✓ reset · ✓ owner · ✓ dns01 · ✓ install:vaultwarden · ✓ app:vaultwarden · ✓ platform-update:wait · ✓ update:vaultwarden · ✗ verify:vaultwarden

- `app:vaultwarden`: ✓ create the vault account · ✓ save a login item
- `verify:vaultwarden`: ✓ sign in from a new device · ✗ the item still decrypts to what was saved

```text
Error: expect(locator).toHaveValue(expected) failed
Locator:  getByRole('dialog', { name: 'View Login' }).getByRole('textbox', { name: 'Password' })
Expected: "E2E-mw0oktzt-item-secret!"
Received: "••••••••"
Timeout:  30000ms
Call log:
  - Expect "toHaveValue" getByRole('dialog', { name: 'View Login' }).getByRole('textbox', { name: 'Password' }) with timeout 30000ms
  - waiting for getByRole('dialog', { name: 'View Login' }).getByRole('textbox', { name: 'Password' })
    64 × locator resolved to <input readonly bitinput="" id="password" type="password" aria-readonly="true" data-testid="login-password" class="[&:is(input,select)]:tw-h-full [&:is(input,textarea):disabled]:!tw-placeholder-fg-inactive [&:is(input,textarea):disabled]:!tw-text-fg-inactive [&:is(input,textarea):disabled]:tw-bg-bg-secondary [&:is(textarea)]:tw-h-auto [&:is(textarea)]:tw-min-h-[30px] [&:is(textarea)]:tw-resize-none [&_option]:tw-bg-background [&_option]:tw-text-main focus:tw-outline-none tw-bg-transparent tw-block tw…/>
       - unexpected value "••••••••"
App page 1: https://vaultwarden.r41637410367.lab.my-demo-domain.site/#/lock
  snapshot: test/e2e/results/20261103-124431-update-vaultwarden/failures/08-vaultwarden-page-1.yaml
```

##### Network: Problems

None.

##### Network: vaultwarden

Updated in `update:vaultwarden`: Before is everything until that step, After is from it on.

| Host | Channel | From | Steps | Before | After | In review |
| --- | --- | --- | --- | --- | --- | --- |
| `api.pwnedpasswords.com` | browser | vaultwarden.r41637410367.lab.my-demo-domain.site | app:vaultwarden, verify:vaultwarden | ✓ | ✓ | yes |

New after the update: none.

#### `@app-dr vaultwarden` failed at `app:vaultwarden`

✓ reset · ✓ owner · ✓ dns01 · ✓ install:vaultwarden · ✗ app:vaultwarden

- `app:vaultwarden`: ✓ create the vault account · ✗ save a login item

```text
TimeoutError: locator.click: Timeout 45000ms exceeded.
Call log:
  - waiting for getByRole('button', { name: /^New/iu }).first()
App page 1: https://vaultwarden.r41637410367.lab.my-demo-domain.site/#/vault
  snapshot: test/e2e/results/20261103-124756-app-dr-vaultwarden/failures/05-vaultwarden-page-1.yaml
```

##### Network: Problems

None.
