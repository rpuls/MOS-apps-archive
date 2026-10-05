# MOS apps archive

Every app package [My Own Suite](https://myownsuite.org) has published, as it shipped, and the evidence from the drills behind each app update.

The suite repository keeps only the current version of each package under [`apps/`](https://github.com/rpuls/my-own-suite/tree/main/apps). This archive keeps every earlier one, so any of them can be read without digging through git history.

## Layout

```text
<app>/
  README.md                every archived version and drill, newest first
  <app version>/           the version of the app itself, as owners see it
    <package version>/     a MOS package of that app version, once the signed catalog published it
      package/             the files the package digest covers: manifest, Dockerfiles, privacy review, README, icon, screenshots
      published.json       the catalog entry, the package digest and the suite commit it was published from
    drills/
      <date>-<commit>/     one update drill: what it ran, the network report and before/after screenshots
```

## What it is not

The archive is a record. MOS never installs from it and its files carry no signature: the signed catalog in the suite repository decides what installs. To check a snapshot, recompute its package digest and compare it with `published.json`, or open the suite commit it names.

Drills are run by Norn, MOS's update bot, on the change behind each app update before it is reviewed. A drill of a version that was never published has a `drills/` folder and no package folder.

## Apps

| App | Latest app version | Package | Published |
| --- | --- | --- | --- |
| [actual-budget](actual-budget/) | 26.8.1 | 0.2.0 | 2026-10-02 |
| [immich](immich/) | 3.1.0 | 0.8.1 | 2026-09-16 |
| [onlyoffice](onlyoffice/) | 9.3.1 | 0.2.5 | 2026-09-16 |
| [paperless-ngx](paperless-ngx/) | 3.1.3 | 0.3.2 | 2026-10-02 |
| [radicale](radicale/) | 3.7.6 | 0.5.1 | 2026-09-16 |
| [seafile](seafile/) | 13.0.21 | 0.3.1 | 2026-09-16 |
| [stirling-pdf](stirling-pdf/) | 2.10.0 | 0.2.6 | 2026-09-16 |
| [vaultwarden](vaultwarden/) | 1.37.0 | 0.4.0 | 2026-10-02 |
