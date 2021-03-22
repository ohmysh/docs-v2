# Cache of OhMySh

## Where is it

Cache of OhMySh is a directory.

When you login to your shell with OhMySh, we will set a variable named `OMS_CACHE`. You can get into this directory with the following command:

```bash
cd $OMS_CACHE
```

Then you will get into the cache directory!

## `update` File

This file controls OhMySh 'Update System'. It looks like this format to date:

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

