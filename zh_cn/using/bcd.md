# 目录记录

此功能可以帮助您记录您到访过的目录，并支持快速跳转。

**命令 `bcd`**

- `bcd` 返回上层目录
- `bcd X` 返回 X 层目录
- `bcd -X` 快进到上 X 个目录

**举个“栗子”**

```bash
$ cd .ohmysh/
$ cd lib/
$ cd etc/

# Now, let's have a try:
$ bcd             # change to lib/
$ bcd -1          # change to etc/
$ bcd 2           # change to .ohmysh/
```
