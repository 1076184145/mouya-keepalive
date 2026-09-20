# 某牙保活（跃度）

某牙保活（跃度）是面向 Linux/WSL x86_64 的个人自动化工具。本仓库仅
发布编译后的二进制文件、校验文件和安装器，不包含私有源码、账号凭证或
个人配置。

> **仅供个人学习、研究与功能测试，严禁任何形式的商业使用。**
> 本项目为非官方工具，使用前请阅读 [免责声明](DISCLAIMER.txt) 和
> [许可证](LICENSE.txt)。

## 一条命令安装

```bash
curl -fsSL https://github.com/1076184145/mouya-keepalive/releases/latest/download/install.sh | bash -s -- 1076184145/mouya-keepalive
```

安装器会从最新 Release 下载 `mouya` 与 `mouya.sha256`，完成 SHA-256
校验后安装到 `~/.local/bin/mouya`。

再次执行上述命令即可更新程序，不会覆盖已有配置或登录态。

## 首次使用

```bash
mouya init
# 编辑 ~/.local/share/mouya/config.json
mouya install-browser
mouya login
mouya run
```

私有运行数据默认保存在 `~/.local/share/mouya/`。请勿上传或分享该目录中的
配置、登录态、状态、日志和截图。

## 签到与缓存

从 v1.0.3 起，每日状态固定按北京时间（UTC+8）分日，不受系统时区影响。
房间签到每次核验网页每日任务，不会仅凭本地缓存报告成功；网页确认已完成时
不重复点击，无法确认时报告失败。送礼仍保留当日防重复记录。

## 支持范围

- Linux / WSL
- x86_64 / amd64

程序按现状提供；页面更新、风控策略或账号状态变化都可能导致功能失效。
