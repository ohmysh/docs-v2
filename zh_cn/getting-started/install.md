# 安装说明

本说明将帮助您安装 OhMySH。

如果你有任何问题，可以在 [(ohmysh/ohmysh) 仓库](https://github.com/ohmysh/ohmysh/issues) 提出议题。

## 准备

OhMySh 基于 [SH shell (Bourne shell)](https://en.wikipedia.org/wiki/Bourne_shell) 或 GNU-Bash 工作。

所以确保你已经安装了 `sh (>=4.x.x)` 和 `bash (>=4.x.x)` 。还有些其他依赖: `curl` `git` .

## 安装

在命令行中运行以下命令来快速安装。

```sh
curl https://raw.githubusercontent.com/ohmysh/ohmysh/main/install.sh > OMSInstaller.sh
bash OMSInstaller.sh
```

> ### 中国用户提示
>
> 你可以把上面那段内容的第一行替换为：
>
> `curl https://ghproxy.com/https://raw.githubusercontent.com/ohmysh/ohmysh/main/install.sh > OMSInstaller.sh`

## 检查安装

Run the following script with **any** shell.

```sh
bash --login
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
