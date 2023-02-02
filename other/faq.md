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
- **ERROR 7** : Some parameters are missing. Please check if the command is correct.
- **ERROR 8** : Please check if your shell supports `declare` (Maybe you can try to update the shell)
- **ERROR 9** : Cannot find `realpath` tool on your computer, please check if your shell supports it.
- **ERROR 10** : Some parameters are missing. Please check if the command is correct.
- **ERROR 11** : Your bash-completion application installed path setting went wrong. Check the path in [here](/using/comp)
- **ERROR 12** : Your configuration file may be out of date, `bash $OMS_DIR/lib/opt/profile-update.sh` to fix.
- **ERROR 13** : Debug option not found, check in `oms --debug list`.
- **ERROR 14** : An update is running beside. If you are sure that there is not any update running, please try with `oms -r`.
- **ERROR 15** : `gdate` cannot be found. If you are using macOS, please install `gdate` to replace `date`.



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

## `date -d` bugs.

On macOS, `date -d` command cannot work properly. We found `gdate` from GNU based on [`coreutils`](https://www.gnu.org/software/coreutils/).

**Way to fix:** (`build >= 75`)

1. Install `coreutils` (`brew install coreutils` on macOS)
2. Test `gdate`: typing `gdate -d 2022.01.01 +%x`. Check if it working properly.

## Known Issues

> We will solve them quickly.

- 01 Zsh bug, please see in _FAQ -> Zsh_ part.
- 02 Chinese Internet errors, please see in _FAQ -> Chinese Internet_ part.
- 03 ~~You may not run plugins by CLI in `0.0.5-build_21`.~~ We fixed it, and to solve it, you can download December Updates.
- 04 ~~You may not delete or restore **just one** file by `trash` in oms build version `< 36`~~, you can download February Updates.
- 05 ~~You may not switch channel by CLI.~~ Fixed it in July 2022.
- 06 ~~`tree` command cannot be used properly, see in https://github.com/ohmysh/ohmysh/issues/21~~, fixed in July 2022
- 07 Command `date -d` cannot be used in macOS, see in _FAQ -> `date -d` bugs_.
- 08 ~~"Open in terminal" may not function properly~~, fixed in Jan 2023.
