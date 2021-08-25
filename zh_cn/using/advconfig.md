# 高级配置

> 这个功能是从 `Augest, 2021 Feature Update` 更新开始的

本教程会帮助你学会更多的配置方案。

**所有的配置内容均在 `$OMS_CACHE/config.ohmysh.sh` 文件内。**

## 暂停更新

OhMySh 更新器将会帮助你自动安装的更新，如果你不希望自动安装，你取消注释以下内容。

```bash
configUpdateDisable=1
```

> 如果你希望手动更新，请使用 `oms -u`.

## 停用封面

[封面是 OhMySh 的一个功能，点击了解](https://ohmysh.github.io/docs-v2/#/zh_cn/using/cover) 如果你希望停用他，取消注释掉下面的内容。

```bash
configCoverDisable=1
```
