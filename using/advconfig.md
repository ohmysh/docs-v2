# Advanced Configuration

> The feature is started in `August, 2021 Feature Update`

This guide will help to configure some more.

**The Configuration file is in `$OMS_CACHE/config.ohmysh.sh`.**

## Disable Update

OhMySh Updater will install the latest update automaticly. If you don't want to install the update automaticly, you can dis-comment this command in config file.

```bash
configUpdateDisable=1
```

> If you want to install update manually, try `oms -u`.

## Disable Cover

[Cover is a feature in OhMySh.](https://ohmysh.github.io/docs-v2/#/using/cover) If you want to disable it, you can dis-comment this command in config file.

```bash
configCoverDisable=1
```
