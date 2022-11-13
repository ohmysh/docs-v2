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

这个日期是最后一次更新的日期。如果你希望立即更新 OhMySh，你可以运行这个命令 `oms --update` .

## `update-lastdate` 文件

存放着上次更新的日期，格式同 update 文件。

## `update-lastver` 文件

上次更新的版本。

格式如: `x.x.x-build_x` .

## `runtime-script` 目录

这个目录保存着 OhMySh 一次性的脚本，这些脚本只会被运行一次，它们通常是由“插件”或“OhMySh 库函数”创建的。

> ### 注意
> 
> 这个目录里的文件将会在运行之后被**删除**，请谨慎使用！！！
> 

## `startup-script` 目录

这个目录保存着 OhMySh 启动时自动运行脚本，它们在每次运行 OhMySh 时被运行。

它和 `runtime-script` 不同，这里的文件**不会**被删除，你可以把你希望运行的脚本程序命名为 `脚本名.sh` 并放入这个目录。

## `alias.ohmysh.sh` 文件

这个文件保存着所有的快捷方式，详见[快捷方式 (Aliases)](https://ohmysh.github.io/docs-v2/#/using/alias).

## `cover.ohmysh.sh` 文件

详见[封面 (Covers)](/zh_cn/using/cover).

## `config.ohmysh.sh` 文件

详见[高级配置 (Advanced Configuration)](/zh_cn/using/advconfig).

## `title.ohmysh.sh` 文件

保存个人标题栏内容。

## `update.o` 文件

标记您更新程序的运行，更新程序运行时此文件将会生成，并在完成之后自动删除。

若此文件在更新程序完成之后仍存在，运行 `oms -r` 进行重置。
