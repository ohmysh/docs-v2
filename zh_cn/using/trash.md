# 垃圾管理

注意: 本程序依赖于 `realpath`.

```bash
              trash 帮助:
trash:
  trash FILE       :  move a file/folder to the bin
lstrash:
  lstrash          :  get a list of the bin
  lstrash KEY      :  search KEY
  lstrash PATH     :  search file on PATH
rmtrash:
  rmtrash FILE     :  remove FILE
  rmtrash KEY      :  search KEY to remove
  rmtrash -a       :  remove all files
retrash:
  retrash FILE     :  restore FILE
  retrash KEY      :  search KEY to restore
```

你可以在[高级配置](/zh_cn/using/advconfig).启用 `mapTrash`

## `trash` : 将文件丢进垃圾站

删除文件使用 `trash FILE`.

## `lstrash` : 获得垃圾站的文件列表

如果你希望获得文件列表，使用 `lstrash`.

搜索请使用 `lstrash KEY` or `lstrash PATH`.

举个例子:

```bash
$ lstrash h
 Date deleted           File name
 2021-12-04 20:05:50    /home/ohmysh/hey
 2021-12-05 10:45:09    /home/ohmysh/hello
 2021-12-25 18:38:37    /home/ohmysh/hey
```

## `rmtrash` : 完全地删除文件

如果你希望强制删除文件，使用 `rmtrash PATH/FILENAME`.

搜索文件删除请使用 `rmtrash SEARCH_NAME`

清空垃圾站，使用 `rmtrash -a`.

## `retrash` : 恢复垃圾站文件

恢复文件， `retrash PATH/FILENAME`

搜索一个文件来恢复， `retrash SEARCH_NAME`

# 垃圾服务

我们提供以下服务：

## 垃圾自动删除

你是否需要定时自动删除文件？OhMySh 能帮到你！

启用它，运行 `oms -e` (vi) 或 `oms -e EDITOR` 打开配置文件，并键入以下内容：

```bash
export trashService='Enable'
export trashAutoDeleteService='Enable'
export trashAutoDeleteConfigDate='30'
```

- `trashAutoDeleteService` : 启用或禁用自动删除服务
- `trashAutoDeleteConfigDate` : 自动删除日期，建议 30 天。
