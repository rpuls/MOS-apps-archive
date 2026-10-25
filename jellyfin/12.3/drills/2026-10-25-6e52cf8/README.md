# jellyfin drill on 6e52cf8b5bdd

Pull request: [#339](https://github.com/rpuls/my-own-suite/pull/339)

On `6e52cf8b5bdd`: `@update jellyfin` failed at `install:jellyfin`, `@app-dr jellyfin` not run.

#### `@update jellyfin` failed at `install:jellyfin`

✓ reset · ✓ owner · ✓ drive · ✗ install:jellyfin

```text
TimeoutError: locator.click: Timeout 45000ms exceeded.
Call log:
  - waiting for getByRole('dialog', { name: 'Jellyfin details' }).getByRole('button', { name: /^Install$/iu })
    - locator resolved to <button disabled type="button" class="mos-btn mos-btn-primary">Install</button>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is not enabled
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is not enabled
    - retrying click action
```

##### Network: Problems

None.

#### `@app-dr jellyfin` not run
