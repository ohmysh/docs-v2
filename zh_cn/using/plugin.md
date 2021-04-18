# 插件

## 获取插件

所有的官方那个插件都安装到 `$OMS_DIR/usr/plugin` 目录了，你可以通过下面的命令获取他们。

```sh
oms --pluginlist
```

如果你希望查看插件的说明或使用方法，可以在[这个目录](https://github.com/ohmysh/ohmysh/tree/main/usr/plugin)里查看子目录的“先读我”文件。

你也可以定制自己的插件，参考[这篇文章](https://github.com/ohmysh/ohmysh/blob/main/usr/plugin/readme.md).

## 使用插件

运行下面的命令

```sh
oms -p <类型> <插件名>
```

- `类型` : There are 3 options, `enable` (Enable a plugin), `disable` (Disable a plugin), `restart` (Restart a **ENABLED** plugin).
- `插件名` : The plugin name you want.
