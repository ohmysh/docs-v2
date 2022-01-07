# 垃圾管理

> This feature is testing now.
> Included in `PRE24`. to try a stable version, please install `PRE26.220103`.

Notice: The trash application depends on `realpath`.

```bash
              trash help:
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

You can enable `mapTrash` in [Advanced Configuration](/using/advconfig).

## `trash` : Move a file to the trash bin

To delete a file to the bin, use `trash FILE`.

## `lstrash` : Get a list of the trash bin

If you want to get a list of the trash bin, use `lstrash`.

If you want to search some files in the bin, use `lstrash KEY` or `lstrash PATH`.

Example:

```bash
$ lstrash h
 Date deleted           File name
 2021-12-04 20:05:50    /home/ohmysh/hey
 2021-12-05 10:45:09    /home/ohmysh/hello
 2021-12-25 18:38:37    /home/ohmysh/hey
```

## `rmtrash` : Delete a file permanently from the bin


If you want to delete a file permanently, try `rmtrash PATH/FILENAME`.

To search a file, try `rmtrash SEARCH_NAME`

To delete all the files in the bin, try `rmtrash -a`.

## `retrash` : Restore a file from the bin

If you want to restore a file, try `retrash PATH/FILENAME`

To search a file, try `retrash SEARCH_NAME`


