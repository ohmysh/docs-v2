# Bash 自动补全

> 本功能正在测试中

你目前可以方便地使用[Bash-Completion](https://github.com/scop/bash-completion)。

## 使用自动补全

使用这个，你需要安装 Bash-Completion。

| 系统平台 | 包管理器 | 命令 |
| :--- | :--- | :--- |
|macOS|	HomeBrew|	`brew install bash-completion`|
|GNU/Linux|	LinuxBrew|	`brew install bash-completion`|
|Debian	|apt|	`sudo apt-get install -y bash-completion`|
|CentOS|	yum	|`sudo yum install -y bash-completion`|
|Fedora / Mageia|	dnf|	`sudo dnf install -y bash-completion`|
|openSUSE|	zypper|	`sudo zypper install -y bash-completion`|
|Alpine Linux|	apk|	`sudo apk add bash-completion`|
|Arch Linux / Manjaro|	pacman|	`sudo pacman -S bash-completion`|

> ### 手动构建
> [https://github.com/scop/bash-completion#installation](https://github.com/scop/bash-completion#installation)

然后检查安装路径。

| 系统平台 | 路径 | 更改配置的内容 |
| :---- | :--- | :--- |
| Linux | `/usr/share/bash-completion/bash_completion` | 无 |
| MacOS | `/sw/etc/bash_completion` | 无 |
| Linux & MacOS | `/etc/profile.d/bash_completion.sh` | 输入 `oms -e` 修改 `bashcompletionPlatform` 的值为 `Custom` 并修改 `bashcompletionPathCustom` 的值为 `/etc/profile.d/bash_completion.sh` 或为其他地址。 |

重启后即可享受了！

## 停用自动补全

停用它，你需要输入 `oms -e` 来更改 `bashcompletionPlatform` 为 `Disable`.

## 关于 Bash-Completion

我们仅仅提供接入使用[scop/bash-completion](https://github.com/scop/bash-completion)应用的方法, 并遵守其i[版权](https://github.com/scop/bash-completion/blob/master/COPYING)规定。
