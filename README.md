# 某牙保活（跃度）

某牙保活（跃度）是面向 Linux/WSL x86_64 的个人自动化工具。

> **仅供个人学习、研究与功能测试，严禁任何形式的商业使用。**
> 本项目为非官方工具，使用前请阅读 [免责声明](DISCLAIMER.txt) 和
> [许可证](LICENSE.txt)。

## 一条命令安装

```bash
curl -fsSL https://github.com/1076184145/mouya-keepalive/releases/latest/download/install.sh | bash -s -- 1076184145/mouya-keepalive

## 首次使用

```bash
mouya init
# 编辑 ~/.local/share/mouya/config.json
mouya install-browser
mouya login
mouya run
```

私有运行数据默认保存在 `~/.local/share/mouya/`。

## 支持范围

- Linux / WSL
- x86_64 / amd64

程序按现状提供；页面更新、风控策略或账号状态变化都可能导致功能失效。
