# Getting ready to use

If you didn't change default shell to SH and bash while installing the OMS, you can run this comand and reboot your machine after that:

## Running with bash [Recommended]

```bash
chsh -s /bin/bash
```

## Running with Zsh

```bash
chsh -s /bin/bash
oms --chsh zsh
chsh -s /usr/bin/zsh
oms -p enable zsh
```

Then, reboot your device.

## Running with SH

If you don't know what it is, do NOT try it.

Go to check your system in installation guide.

```bash
chsh -s /bin/sh
```

**Or** run command `sh --login` or `bash` if you want to use it.
