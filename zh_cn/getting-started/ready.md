# 准备使用

本文将告诉您如何开始使用 OhMySh。

首先你需要选取一个 shell。

## Linux MacOS 用户

### 使用 Bash [建议]

```bash
chsh -s /bin/bash
```

然后重启。

### 使用 Zsh

```bash
chsh -s /bin/bash
```

重新登陆。

```bash
oms --chsh zsh
chsh -s /usr/bin/zsh
oms -p enable zsh
```

然后重启电脑。

<!--

### 使用 SH

如果你不知道什么是 SH，你最好不要选择更换到 sh。

在更换之前，你可能需要到[这里](https://ohmysh.github.io/docs-v2/#/zh_cn/getting-started/system)查看你的系统是否支持。

```
chsh -s /bin/sh
```

**或者**你不希望更换shell，你也可以启动时运行 `sh --login` 。

-->

## Windows 用户

重启计算机即可。
