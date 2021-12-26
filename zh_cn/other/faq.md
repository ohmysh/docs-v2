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

## 已知问题

> 我们将尽快修复

- Zsh 问题, 请查看 _FAQ -> zsh_ 部分。
- 中国网络问题请查看 _FAQ -> 中国网络问题_ 部分。
- `0.0.5-build_21` 可能无法使用 CLI 操控插件，目前已经修复，请安装**十二月更新**。


