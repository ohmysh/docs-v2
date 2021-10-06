# OhMySh FAQ

## Installation Errors

- **Error code `1`** : OMS cannot found some application for run OMS, you can read "Prepare" to fix
- **Error code `2`** : You had installed OMS
- **Error code `3`** : Cannot reach to GitHub Repo ohmysh/ohmysh, checking internet

## Using Errors

- **ERROR 1** : Run `ohmysh --help`
- **ERROR 2** : Run `ohmysh --help` to check your options
- **ERROR 3** : Run Installer Script and add option `--config` like `sh OMSInstaller.sh --config`
- **ERROR 4** : Run `ohmysh --themelist` to check the name.
- **ERROR 5** : Run `ohmysh --pluginlist` to check the name.
- **ERROR 6** : Check your Internet connection, we cannot connect to GitHub repository.



- **Cannot run OMS** : Run Installer Script and add option `--config` like `sh OMSInstaller.sh --config`
- **Cannot apply your own theme/plugin** : Check if your own theme/plugin name is different to OhMySH official theme/plugin name in `$OMS_DIR/usr/theme/` or `$OMS_DIR/usr/plugin/` .
- **Cannot found CLI** : Run Install Script again to fix it

## Zsh

OhMySh can run on Zsh after **Zsh Features Update (July 2021)**. We fixed these errors in the update.

Run these commands in `bash`:

```bash
oms --chsh zsh
chsh -s /usr/bin/zsh
oms -p enable zsh
```

Then, restart the computer and enjoy zsh!

## Known Problems

> We will solve them quickly.

- Zsh bug, please see in _FAQ -> Zsh_ part.
- Chinese Internet errors, please see in _FAQ -> Chinese Internet_ part.
