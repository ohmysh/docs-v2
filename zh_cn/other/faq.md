# OhMySh FAQ

这是常见的一些报错，您可以通过下表自行解决错误，如果仍未解决，您可以在 [GitHub ohmysh/ohmysh 仓库](https://github.com/ohmysh/ohmysh/issues)向我们提出 Issue。

## 安装错误

- **Error code `1`** : OhMySh 安装器找不到某些需要的软件，请阅读[安装说明->准备](https://ohmysh.github.io/docs-v2/#/zh_cn/getting-started/install?id=%e5%87%86%e5%a4%87)部分
- **Error code `2`** : 你已经安装了 OhMySh，或你选择的安装路径已存在
- **Error code `3`** : 无法连接到 GitHub 官方仓库 (ohmysh/ohmysh) 请检查网络连接

## 使用错误

- **ERROR 1** : 运行 `ohmysh --help` 。
- **ERROR 2** : 运行 `ohmysh --help` 检查你的参数是否正确。
- **ERROR 3** : 添加 `--config` 参数运行安装程序，例如 `sh OMSInstaller.sh --config` 。
- **ERROR 4** : 运行 `ohmysh --themelist` 检查你所输入的名称是否存在。
- **ERROR 5** : 运行 `ohmysh --pluginlist` 检查你所输入的名称是否存在。
- **ERROR 6** : 请检查您的网络连接，我们无法连接到 GitHub 的仓库。
- **ERROR 7** : 参数丢失，请检查你的命令是否正确。
- **ERROR 8** : 请检查您的终端是否支持 `declare` （可能是由于你的终端版本过老导致的）
- **ERROR 9** : 请检查你的设备是否支持 `realpath` 指令
- **ERROR 10** : 参数丢失，请检查你的命令是否正确。
- **ERROR 11** : Bash-Completion 自动补全安装路径配置错误，查看[这里](/zh_cn/using/comp)来更改配置。
- **ERROR 12** : 你的配置文件可能已经过期了，运行 `bash $OMS_DIR/lib/opt/profile-update.sh` 以解决问题。
- **ERROR 13** : 未定义的调试名称，通过 `oms --debug list` 来检查
- **ERROR 14** : 存在一个更新进程正在后台运行。如果确实没有更新进程在运行，您可以通过 `oms -r` 来解决这个问题。





- **无法运行 OMS** : 添加 `--config` 参数运行安装程序，例如 `sh OMSInstaller.sh --config`
- **无法应用自己的主题/插件** : 检查你自己的主题/插件名称是否与官方仓库 `$OMS_DIR/usr/theme/` 或 `$OMS_DIR/usr/plugin/` 目录下名称重复
- **Cannot found CLI** : 重新安装 OhMySh 以解决问题


## 中国网络问题

在中国大陆特定网络环境下是无法（快速）连接到 GitHub 官方仓库，这个问题我们并不确定是否完全解决，目前我们可以帮助受限制用户通过中国区镜像站快速访问，操作办法见下面部分。

### 获取安装程序错误

你可以把获取安装程序方法改为：

```bash
curl https://gitee.com/ohmysh/ohmysh-mirror/raw/main/install.sh > OMSInstaller.sh
bash OMSInstaller.ah
```

### 获取仓库

你可以把安装程序执行方法改成:

```bash
REPO=https://gitee.com/ohmysh/ohmysh-mirror.git bash OMSInstaller.sh
```

### 仓库任意文件访问

在官方仓库里所有文件均可以通过 Gitee Web 网页端进行访问（不能修改），可以通过[此链接](https://gitee.com/ohmysh/ohmysh-mirror)来访问。

也可以通过 API 进行访问，具体方式见下：

```bash
curl https://gitee.com/ohmysh/ohmysh-mirror/raw/main/PATH/TO/FILE.TYPE
```

### 修改文件

在 Gitee 镜像仓库提交拉取请求是不会被通过的，你需要登录 GitHub 官方仓库进行提交。

## Zsh

OhMySh 自从 **Zsh Features Update (July 2021) (Zsh 功能性更新 2021.07)** 完成后，我们解决了 Zsh 的若干问题，现在可以正常运行了。

在 `bash` 中运行以下命令:

```bash
oms --chsh zsh
chsh -s /usr/bin/zsh
oms -p enable zsh
```

重启计算机后即可享用！

## `date -d` 问题

在 macOS 系统上 `date -d` 命令无法正常工作，我们目前使用由 GNU 开发的包含于[`coreutils`](https://www.gnu.org/software/coreutils/)
的 `gdate` 软件。

**解决方法:** (`build >= 75`)

1. 安装 `coreutils` (macOS 示例 `brew install coreutils`)
2. 测试 `gdate`: 输入 `gdate -d 2022.01.01 +%x` ，检查是否能正常工作。

## 已知问题

> 我们将尽快修复

- 01 Zsh 问题, 请查看 _FAQ -> zsh_ 部分。
- 02 中国网络问题请查看 _FAQ -> 中国网络问题_ 部分。
- 03 ~~`0.0.5-build_21` 可能无法使用 CLI 操控插件~~，目前已经修复，请安装**十二月更新**。
- 04 ~~`< 36` 版本之前的回收站可能无法仅删除或恢复**一个**文件，~~目前已经修复，请安装**二月更新**。
- 05 ~~你可能无法使用 CLI 更换更新频道~~，已经在2022年7月解决
- 06 ~~`tree` 命令可能无法正常使用，详见 https://github.com/ohmysh/ohmysh/issues/21~~，已经在2022年7月解决。
- 07 `date -d` 命令无法在 macOS 中使用，将不会修复了
- 08 ~~“在终端内打开”可能无法使用~~，已经在2023年1月修复。


