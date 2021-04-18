# Plugins

## Getting Plugins

All the plugins of OMS are installed at `$OMS_DIR/usr/plugin` folder. Run the following command to get a list of them.

```sh
oms --pluginlist
```

If you want to check the plugins' introductions or it's usages, you can read "ReadMe" files in [this folder](https://github.com/ohmysh/ohmysh/tree/main/usr/plugin).

You can also make a customized plugin by yourself. Read [This page](https://github.com/ohmysh/ohmysh/blob/main/usr/plugin/readme.md).

## Running Plugins

Run the following command:

```sh
oms -p TYPE PLUGIN-NAME
```

- `TYPE` : There are 3 options, `enable` (Enable a plugin), `disable` (Disable a plugin), `restart` (Restart a **ENABLED** plugin).
- `PLaUGIN-NAME` : The plugin name you want.
