# 更新日志

> 自从 OhMySh 0.0.4 版本起，我们把更新日志放到这里。

当前最新版本: **OhMySh 0.1 长期支持 (Dec 2022)** `Dec2022@0.1.0-build_82.20221225`

## 十二月更新

> 更新于 2022 年 12 月 25 日

- 新增了编辑器选项功能
- 新增了目录切换记录
- 解决了垃圾箱的问题
- **解决了提示符输出异常**
- 移除了查错器

## 十月体验&积累更新

> 更新于 2022 年 10 月 30 日

- 更新了对于 lolcat 的支持
- 更新了 `title` 功能
- 提升了 CLI 的用户体验.
- 修复 ohmysh/ohmysh#29 的错误
- 更新了 `OhMySh Updater`

## 八月功能性&体验性更新

> 更新于 2022 年 8 月 31 日

- 新增了 lolcat 输出
- 新增了 `debug` 功能
- 更新了 CLI 格式
- 更新了安装程序

合并了 ohmysh/ohmysh#27

特别感谢 @0x07CB 的贡献。

## 七月功能性&积累更新

> 更新于 2022 年 7 月 31 日

- 解决了上个稳定版本的大量错误
- 更新了 `安装程序`
- 新增了 `终端标题` 功能
- 新增了对于 macOS 的贴士

## 三月体验更新

> 更新于 2022 年 3 月 31 日

- 添加了开发板更换器。
- 更新了 `更新器`.
- 更新了 `安装程序`.
- 更新了配置文件路径格式.
- 包含了 CLI 更新:
  - 更新了 `-v` 显示.
  - 更新了 `-r|--reload` 格式.

## 二月功能性&累积更新 `0.0.6-build_40.220222`

> 更新于 2022 年 2 月 22 日

- 添加了 `completion` 新功能
- 添加了 `time/date format` 新功能
- 添加了 `OhMySh Reload` 新功能
- 修复了 `Installer`
- 修复了 `Updater`
- 修复了 `theme` 功能
- 修复了 `trash` 功能
- 包含了 CLI 更新:
  - 添加了新的链接 `-r|--reload`
  - 修复了积累的错误

## 一月功能性更新 `0.0.5-build_30.220129`

> 更新于 2022 年 1 月 29 日

- 更新了 `trash` 新功能
- 添加了一些垃圾服务
- 更新了 `安装引导程序` 添加了色彩输出
- 添加了 环境变量设置
- 包含了 CLI 更新 `0.0.5-build_17`
  - 更新了 帮助菜单
  - 添加了 `高级设置` 设置链接

## 十二月累积更新 `0.0.5-build_23`

> 更新于 2021 年 12 月 29 日

- 解决了 `主题` 功能的错误: `usr/theme/*`
- 包含了 CLI 的 `0.0.5-build_16` 更新:
  - 解决了插件选项的一些错误
- [*测试版本*] 新增了 `垃圾桶` 功能

## 十一月累积更新 `0.0.5-build_21`

> 更新于 2021 年 11 月 27 日

- 解决了 shell-check 发现的一大堆问题 (32 个文件).
- 解决了自动化的错误: `.github/workflows/`
- 停用了旧 git 模块: `lib/git.sh`
- 停用了旧 `_OMS_PWD` 命名规则 : `lib/dir.sh`
- 修正了 `logo` 出现的问题 : `lib/logo.sh`

> 包含了 `build_PRE19`, `build_PRE20`, `build_21`.

## 十月体验更新 `0.0.5-build_16`, `0.0.5-build_PRE17`, `0.0.5-build_18`

> 更新于 2021 年 10 月 24 日

- `0.0.5-build_16`
  - 更新了 `高级配置` 功能: `lib/config.sh`, `lib/etc/config.etc.sh`, cover, map, updater.
- `0.0.5-build_PRE17`
  - 更新了 `logo`: `lib/logo.sh`.
  - 更新了 `CLI::version` 显示功能: `lib/ohmysh-cli.sh`.
- `0.0.5-build_18`
  - 更新了 `主题` 功能的输出显示: `lib/theme.sh`.
  - 更新了 `更新器` 功能的输出显示: `lib/update.sh`.
  - 解决了主程序中的一些问题: `main.sh`.
  - 更新了 `pacman` 插件: `usr/plugin/pacman/pacman.plugin.sh`.

## 九月体验更新 `0.0.5-build_14`, `0.0.5-build_15`

> 更新于 2021 年 9 月 25 日

- `0.0.5-build_14`
  - 更新了 `高级配置` 功能: `lib/config.sh`, `lib/etc/config.etc.sh`.
  - 解决了 CLI 的一些错误.
  - 更新了 `主题` 功能的 `git prompt` 功能 : `lib/git-prompt.sh`.
  - 更新了一些主题
- `0.0.5-build_15`
  - 更新了 `Command Redirect` 功能 : `lib/opt/map.sh` .

## 八月更新 `0.0.5-build_13`

> 更新于 2021 年 8 月 25 日

- 更新了 `高级配置` 功能: `lib/config.sh`, `lib/etc/config.etc.sh`.
- 解决了 `封面` 的一些错误: `lib/cover.sh`.
- 解决了更新程序的一些错误: `lib/update.sh`.
- 更新了安装程序: `install.sh`.
- 包含了 CLI 的更新: `lib/cli.sh`
  - 更新了 CLI 的版本输出.

## Zsh 功能更新 `0.0.5-build_12.1`

> 更新于 2021 年 7 月 28 日

- 更新了 Zsh 功能。

## 六月更新 `0.0.5-build_12`

> 更新于 2021 年 6 月 13 日

- 更新了安装程序: `install.sh` :
  - 添加了图标输出.
- 更新了快捷方式模板命名规则: `lib/alias.sh`.
- 新增了 `Cover` 功能: `lib/cover.sh`:
  - 新增了模板.
  - 添加了 `默认 Default` 封面.
- 新增了图形图标输出:
  - 新增了 `logo` 功能: `lib/logo.sh`.
  - 新增了图标.
- 包含了 CLI 的更新:
  - 更新了 CLI 插件管理:
    - 新增了 `start plugin` 模式.
  - 更新了版本查询.
  - 新增了封面控制.
- 更新了 `updater`: `lib/update.sh`.
- 在主程序里更新了一些注释.

## 五月更新 `0.0.4-build_11`

> 更新于 2021 年 5 月 11 日.

- 更新了描述文件
- 包含了安装程序更新: `install.sh` :
  - 新增功能 `更换仓库源`.
- 更新了错误代号 `3,4,5` : `main.sh`.

## 中国区镜像同步脚本更新

> 更新于 2021年4月18日

- 更新了同步脚本
  - 包含新增的“构建 Pages”

## `0.0.3-pre_10`

> 更新于 2021/03/27

- 添加了 `特殊日期提示` 功能: `lib/opt/special-date.sh`
- 添加了 `命令重定向` 功能: `lib/opt/map.sh`
- 更新了 `查看命令是否存在` 模块: `lib/check-command.sh` :: function `checkcmd`
- 包含了 CLI 的 `0.0.3-build_7` 更新：
  - 更新了帮助页面

## OhMySh 中国镜像 (Gitee)

> 更新于 2021/03/25.

中国区镜像包含官方仓库和官方文档 (v2)。

- OhMySH 主仓库镜像地址: [gitee.com/ohmysh/ohmysh-mirror](https://gitee.com/ohmysh/ohmysh-mirror)
- OhMySH 开放文档镜像地址: [ohmysh.gitee.io/docs-v2](https://ohmysh.gitee.io/docs-v2)
