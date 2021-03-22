# OhMySh 缓存

## 缓存在哪里

OhMySh 的缓存存储在一个目录中。

当登陆 OhMySh 时会设定 `OMS_CACHE` 变量，你可以通过以下命令进入这个目录:

```bash
cd $OMS_CACHE
```

那么你将进入这个目录！

## `update` 文件

这个文件控制着 OhMySh 的“更新系统”，文件内部存储着最后一次更新的日期，格式如下：

```bash
YYYY/MM/DD
```

It is the last update to date. If you want to update your OhMySh now, you can try this command `oms --update` .

## `runtime-script` Directory

This directory holds the OMS runtime file. The files in this directory are always created by plugins or OhMySh library scripts.

> ### Warning
> 
> The file in this directory will be **cleaned** when OhMySh is running again!!!
> 

## `startup-script` Directory

This directory holds the OMS startup scripts. When OMS start running, the files in this directory will run automatically.

It is diffirence from `runtime-script`, the files in here will **not** delete. You can put your files into this directory and named with `SCRIPT-NAME.sh`.

## `alias.ohmysh.sh` File

This file holds the aliases of your shell. See in [Aliases](https://ohmysh.github.io/docs-v2/#/using/alias).
