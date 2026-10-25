# jellyfin drill on 71b81fc954c5

Pull request: [#339](https://github.com/rpuls/my-own-suite/pull/339)

On `71b81fc954c5`: `@update jellyfin` failed at `update:jellyfin`, `@app-dr jellyfin` passed.

#### `@update jellyfin` failed at `update:jellyfin`

✓ reset · ✓ owner · ✓ drive · ✓ install:jellyfin · ✓ app:jellyfin · ✓ platform-update:wait · ✗ update:jellyfin

- `app:jellyfin`: ✓ sign in as the administrator chosen at install · ✓ the Movies and Series libraries are already there · ✓ copy a film onto the drive and plug it back in · ✓ Jellyfin finds the film on its own · ✓ the film plays

```text
TimeoutError: locator.click: Timeout 45000ms exceeded.
Call log:
  - waiting for getByRole('dialog', { name: 'Review Jellyfin update' }).getByRole('button', { name: 'Update', exact: true })
    - locator resolved to <button disabled type="button" class="mos-btn mos-btn-primary">Update</button>
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

##### Network: jellyfin

Updated in `update:jellyfin`: Before is everything until that step, After is from it on.

| Host | Channel | From | Steps | Before | After | In review |
| --- | --- | --- | --- | --- | --- | --- |
| `www.gstatic.com` | browser | jellyfin.mos.lab | app:jellyfin | ✓ |  | yes |
| `repo.jellyfin.org` | server | app | app:jellyfin | ✓ |  | yes |
| `sfo1.mirror.jellyfin.org` | server | app | app:jellyfin | ✓ |  | yes |
| `api.themoviedb.org` | server | app | app:jellyfin | ✓ |  | yes |
| `www.omdbapi.com` | server | app | app:jellyfin | ✓ |  | yes |

New after the update: none.

#### `@app-dr jellyfin` passed

✓ reset · ✓ owner · ✓ drive · ✓ install:jellyfin · ✓ app:jellyfin · ✓ backup:bucket · ✓ reset · ✓ owner · ✓ restore:bucket · ✓ verify:jellyfin · ✓ routes · ✓ network · ✓ cleanup

- `app:jellyfin`: ✓ sign in as the administrator chosen at install · ✓ the Movies and Series libraries are already there · ✓ copy a film onto the drive and plug it back in · ✓ Jellyfin finds the film on its own · ✓ the film plays
- `verify:jellyfin`: ✓ sign in · ✓ the film on the drive is still in the library · ✓ and still plays

##### Network: Problems

None.

##### Network: jellyfin

| Host | Channel | From | Steps | In review |
| --- | --- | --- | --- | --- |
| `repo.jellyfin.org` | server | app | app:jellyfin, restore:bucket | yes |
| `www.gstatic.com` | browser | jellyfin.mos.lab | app:jellyfin, verify:jellyfin | yes |
| `sfo1.mirror.jellyfin.org` | server | app | app:jellyfin, restore:bucket | yes |
| `api.themoviedb.org` | server | app | app:jellyfin | yes |
| `www.omdbapi.com` | server | app | app:jellyfin | yes |
