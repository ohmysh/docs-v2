# 安装说明

本说明将帮助您安装 OhMySH。

如果你有任何问题，可以在 [(ohmysh/ohmysh) 仓库](https://github.com/ohmysh/ohmysh/issues) 提出议题。

## 准备

请先[系统页面](/zh_cn/getting-started/system)检查系统要求。

OhMySh 基于 [SH shell (Bourne shell)](https://en.wikipedia.org/wiki/Bourne_shell) 或 GNU-Bash 工作。

所以确保你已经安装了 `sh (>=4.x.x)` 和 `bash (>=4.x.x)` 。还有些其他依赖: `curl` `git` .

> ### 对于 MacOS 用户
> 如果你正在使用 macOS，你需要从 homebrew 或 apt 安装最新版的 bash。
> 1. `brew install bash`
> 2. `echo 'alias bash="/opt/homebrew/bin/bash"' >> ~/.zshrc`

现在我们支持 `lolcat` 了，您可以在安装程序中选择自动安装（或手动安装）。

## 安装

在命令行中运行以下命令来快速安装（这条命令可能不使用于中国，中国网络请使用下面的命令）

```bash
curl https://raw.githubusercontent.com/ohmysh/ohmysh/main/install.sh > OMSInstaller.sh
bash OMSInstaller.sh
```


或者如果你在中国，你可以[在FAQ的中国网络部分](https://ohmysh.github.io/docs-v2/#/zh_cn/other/faq?id=%e4%b8%ad%e5%9b%bd%e7%bd%91%e7%bb%9c%e9%97%ae%e9%a2%98)获得解决方案。

<!--
或者如果你在中国，你可以使用这条命令来访问中国区镜像来获取安装程序。

```bash
curl https://gitee.com/ohmysh/ohmysh-mirror/raw/main/install.sh > OMSInstaller.sh
bash OMSInstaller.ah
```
-->

## 检查安装

在终端中运行这个命令来检查是否安装是否成功

```bash
bash
```

## 高级选项

### 获取下载器

在命令行中运行以下命令。

```sh
curl https://raw.githubusercontent.com/ohmysh/ohmysh/main/install.sh > OMSInstaller.sh
```

### 使用高级选项

运行安装程序带着下面的环境变量，例如 `env1_name=env1_value env2_name=env2_value sh OMSInstaller.sh`

- 更改 OhMySh 安装路径
  - ENV_NAME: `OMS`
  - ENV_VALUE: [PATH]
  - 提示: 不要把这个路径设定成无法访问的路径。
- 更改运行时文件存储目录
  - ENV_NAME: `OMS_CACHE`
  - ENV_VALUE: [PATH]
  - 提示: 不要把这个路径设定成无法访问的路径，并且不能与安装路径重复或嵌套。
