# 高级配置

> 这个功能是从 `Augest, 2021 Feature Update` 更新开始的

本教程会帮助你学会更多的配置方案。

**所有的配置内容均在 `$OMS_CACHE/config.ohmysh.sh` 文件内。**

## 暂停更新

OhMySh 更新器将会帮助你自动安装的更新，如果你不希望自动安装，你取消注释以下内容。

```bash
configUpdateDisable='Disable'
```

> 如果你希望手动更新，请使用 `oms -u`.

## 停用封面

[封面是 OhMySh 的一个功能，点击了解](https://ohmysh.github.io/docs-v2/#/zh_cn/using/cover) 如果你希望停用他，取消注释掉下面的内容。

```bash
configCoverDisable='Disable'
```

## 更改启动路径

如果你希望更改它，你可以取消以下注释。

```bash
configStartPath='/path/path/'
```

## 禁用/启用一些命令

你可以在配置文件中取消注释下面的内容。

```bash
mapLs='Disable'  # Or Enable
mapCd='Disable'
mapHelp='Enable'
mapMSDos='Enable'
mapCSP2021='Disable'
mapTrash='Enable'
```

## 垃圾服务

在[本文查看](/zh_cn/using/trash)。

## 系统环境变量设置 (`$PATH`)

通过添加下列内容，可以追加环境变量。

```bash
configPathEnv='Path1:Path2:Path3:...'
```

## Bash-Completion

详见[Bash-Completion](/zh_cn/using/comp)

## 日期、时间格式

如果你希望设置时间和日期的格式，修改配置文件的 `dateFormat` `timeFormat` 来实现。

格式规则：见 `date --help`

## 编辑器选择

取消注释并替换 `XXX` 为你想要的编辑器， `editorSelect="XXX"` 。

```bash
editorSelect='XXX'
```
