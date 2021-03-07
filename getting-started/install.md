# Installation Guide

This guide will help you to install the OhMySH.

If you have any question, open a new issue in [(ohmysh/ohmysh) repository](https://github.com/ohmysh/ohmysh/issues) to tell us.

## Preparation

OhMySh works with [SH shell (Bourne shell)](https://en.wikipedia.org/wiki/Bourne_shell) or GNU-Bash.

So make sure `sh (>=4.x.x)` was installed. There are some other dependences: `curl` `git` .

## Installation

Run the following commands with SH.

```sh
curl https://raw.githubusercontent.com/ohmysh/ohmysh/main/install.sh > OMSInstaller.sh
sh OMSInstaller.sh
```

> ### For Chinese users
>
> Get the installer from this: 
>
> `curl https://ghproxy.com/https://raw.githubusercontent.com/ohmysh/ohmysh/main/install.sh > OMSInstaller.sh`

## Checking the Installation

Run the following script with **any** shell.

```sh
sh --login
```

> ### Running SH with `--login` option
>
> If you run SH with the `--login` option, SH will run OMS automatically.
>

## Advanced Options

### Getting Installer

Run the following commands with SH.

```sh
curl https://raw.githubusercontent.com/ohmysh/ohmysh/main/install.sh > OMSInstaller.sh
```

### Run with Advanced Options

Run installer script with some enviroment, such as `env1_name=env1_value env2_name=env2_value sh OMSInstaller.sh`

- Change OhMySH installation path
  - ENV_NAME: `OMS`
  - ENV_VALUE: [PATH]
  - More info: Do not set it to a path without access rights.
- Change OhMySH cache path
  - ENV_NAME: `OMS_CACHE`
  - ENV_VALUE: [PATH]
  - More info: Do not set it to a path that does not have access rights and cannot be the same as the installation path or inside the installation path.
