# Trash Manager

> This feature is testing now.
> Included in `PRE24`.

Notice: The trash application depends on `realpath`.

## `trash` : Move a file to the trash bin

To delete a file to the bin, use `trash FILE`.

## `lstrash` : Get a list of the trash bin

If you want to get a list of the trash bin, use `lstrash`.

Example:

```bash
$ lstrash
 Date deleted           File name
 2021-12-04 20:05:50    /home/ohmysh/hey
 2021-12-05 10:45:09    /home/ohmysh/hello
 2021-12-25 18:38:37    /home/ohmysh/hey
```

## `rmtrash` : Delete a file permanently from the bin


If you want to delete a file permanently, try `rmtrash PATH/FILENAME`.

To search a file, try `rmtrash /SEARCH_NAME`

## `retrash` : Restore a file from the bin

If you want to restore a file, try `retrash PATH/FILENAME`

To search a file, try `retrash /SEARCH_NAME`


