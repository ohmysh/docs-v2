# Advanced Configuration

> The feature is started in `August, 2021 Feature Update`

This guide will help to configure some more.

**The Configuration file is in `$OMS_CACHE/config.ohmysh.sh`.**

## Disable Update

OhMySh Updater will install the latest update automaticly. If you don't want to install the update automaticly, you can dis-comment this command in config file.

```bash
configUpdateDisable='Disable'
```

> If you want to install update manually, try `oms -u`.

## Disable Cover

[Cover is a feature in OhMySh.](https://ohmysh.github.io/docs-v2/#/using/cover) If you want to disable it, you can dis-comment this command in config file.

```bash
configCoverDisable='Disable'
```

## Edit Start Path

If you want to change it, you can dis-comment this command in config file and edit it.

```bash
configStartPath='/path/path/'
```

## Disable/Enable some aliases command

You can dis-comment this command in config file.

```bash
mapLs='Disable'  # Or Enable
mapCd='Disable'
mapHelp='Enable'
mapMSDos='Enable'
mapCSP2021='Disable'
mapTrash='Enable'
```

## Trash Services

See in [here](/using/trash).

## System Environment Path (`$PATH`)

To add environment path, dis-comment this and add something in it.

```bash
configPathEnv='Path1:Path2:Path3:...'
```

## Bash-completion

See in [Bash-Completion](/using/comp).

## Date & Time Format

If you want to set date or time format, edit `dateFormat` and `timeFormat` in the config file.

About rules see in `date --help`.

## Editor Selection

Uncomment and replace `XXX` to the editor you want to set `editorSelect="XXX"`.

```bash
editorSelect='XXX'
```
