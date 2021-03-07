# OhMySh FAQ

## Installation Errors

- **Error code `1`** : OMS cannot found some application for run OMS, you can read "Prepare" to fix
- **Error code `2`** : You had installed OMS
- **Error code `3`** : Cannot reach to GitHub Repo ohmysh/ohmysh, checking internet

## Using Errors

- **Error 1** : Run `ohmysh --themelist` to check the name.

- **Error 2** : Run `ohmysh --pluginlist` to check the name.




- **Cannot run OMS** : Run Installer Script and add option `--config` like `sh OMSInstaller.sh --config`

- **Cannot apply your own theme/plugin** : Check if your own theme/plugin name is different to OhMySH official theme/plugin name in `$OMS_DIR/usr/theme/` or `$OMS_DIR/usr/plugin/` .

## OhMySh Command Line Interface

- **ERROR 1** : Run `ohmysh --help`
- **ERROR 2** : Run `ohmysh --help` to check your options



- **Cannot found CLI** : Run Install Script again to fix it

## Known Problems

> We will solve them quickly.

- Zsh bug, please see in _Known Problems -> For Zsh_ part.

> ### For Zsh
> 
> Ohmysh cannot run on zsh because of the color or prompt format of sh/bash is different to zsh.
