# Installation Guide

This guide will help you to install the OhMySH.

If you have any question, open a new issue in [(ohmysh/ohmysh) repository](https://github.com/ohmysh/ohmysh/issues) to tell us.

## Preparation

Check your system required first in [System Page](/getting-started/system).

OhMySh works with [SH shell (Bourne shell)](https://en.wikipedia.org/wiki/Bourne_shell) , GNU-Bash and Zsh.

So make sure `sh (>=4.x.x)` and `bash (>=4.x.x)` or `zsh (>=5.x.x)` was installed. There are some other dependences: `curl` `git` .

> ### For MacOS Users
> If you are using macOS, you may need to install latest version of `bash` and [`coreutils`](https://ohmysh.github.io/docs-v2/#/other/faq?id=date-d-bugs) from [homebrew](https://brew.sh), apt, etc. [**No homebrew?**](https://brew.sh)
> 1. `brew install bash` and `brew install coreutils` (for brew users)
> 2. `echo 'alias bash="/opt/homebrew/bin/bash"' >> ~/.zshrc`

`lolcat` can be used in our program. If you want to use it, select `install` in installation script (or you can install by yourself).

## Installation

Run the following commands with shell. (Not support Chinese internet)

```bash
curl https://raw.githubusercontent.com/ohmysh/ohmysh/main/install.sh > OMSInstaller.sh
bash OMSInstaller.sh
```

Or if you are in China, you may need get installer from Chinese mirror with this commands:

```bash
curl https://gitee.com/ohmysh/ohmysh-mirror/raw/main/install.sh > OMSInstaller.sh
bash OMSInstaller.ah
```

## Checking the Installation

Run the following script with **any** shell.

```sh
bash
```

## Ready to use

Please read [Ready to use](/getting-started/ready) page in docs. **It will be very useful!**

## Advanced Options

### Getting Installer

Run the following commands with shell.

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
