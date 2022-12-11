# Directory Recording

This can record your directory changing, to back to last directories.

**Command `bcd`**

- `bcd` to back to the last directory.
- `bcd X` to back to the last X directories.
- `bcd -X` to move forward the last X directories.

**Examples**

```bash
$ cd .ohmysh/
$ cd lib/
$ cd etc/

# Now, let's have a try:
$ bcd             # change to lib/
$ bcd -1          # change to etc/
$ bcd 2           # change to .ohmysh/
```
