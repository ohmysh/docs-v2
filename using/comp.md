# Bash Completion Supporting

> This feature is still in pre-releases

You now can use [Bash Completion](https://github.com/scop/bash-completion) easily in OhMySh.

## Enabling Auto Completion

To enable this, you need to install the Bash-Completion program.

| System Platform | Package Manager | Command |
| :--- | :--- | :--- |
|macOS|	HomeBrew|	`brew install bash-completion`|
|GNU/Linux|	LinuxBrew|	`brew install bash-completion`|
|Debian	|apt|	`sudo apt-get install -y bash-completion`|
|CentOS|	yum	|`sudo yum install -y bash-completion`|
|Fedora / Mageia|	dnf|	`sudo dnf install -y bash-completion`|
|openSUSE|	zypper|	`sudo zypper install -y bash-completion`|
|Alpine Linux|	apk|	`sudo apk add bash-completion`|
|Arch Linux / Manjaro|	pacman|	`sudo pacman -S bash-completion`|

> ### Build it by yourself
> [https://github.com/scop/bash-completion#installation](https://github.com/scop/bash-completion#installation)

Then, Check your bash-completion path.

| System Platform | Path | Edit configuration file |
| :---- | :--- | :--- |
| Linux | `/usr/share/bash-completion/bash_completion` | No |
| MacOS | `/sw/etc/bash_completion` | No |
| Linux & MacOS | `/etc/profile.d/bash_completion.sh` | Type `oms -e` to change `bashcompletionPlatform` to `Custom` and change `bashcompletionPathCustom` to `/etc/profile.d/bash_completion.sh` or maybe other path. |

Next, reboot your machine. Now you can enjoy it!

## Disabling Auto Completion

To disable this, you need to type `oms -e` to change `bashcompletionPlatform` to `Disable`.

## About Completion

The Bash-Completion is just using from [scop/bash-completion](https://github.com/scop/bash-completion), and we undered its [license](https://github.com/scop/bash-completion/blob/master/COPYING).
