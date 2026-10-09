# Git 实战速查表 · Git Cheatsheet

> 🌍 [Español](README.es.md) · [Português](README.pt.md)

一份**一页纸**的 Git 实战救命速查表：30 条偏"救命向"的真实命令，按场景分类——**配置、日常、撤销、分支、rebase、储藏、远程、救命命令、高级**。每条只讲三件事：**它是干什么的、一条可复制的命令、适用场景标签**。不灌水，不凑数，全部命令均为真实 git 语法。

## 面向谁

每天都在 `git add/commit/push` 里打转的开发者，以及被 `rebase` 冲突、误删分支、丢提交吓出过冷汗的你。如果你只会三板斧，这张表能让你在关键时刻自救。

## 怎么用

1. 直接看 **[CHEATSHEET.md](CHEATSHEET.md)** ——速查表正文，英文命令全球通用。
2. 先跑"配置"三条：身份、默认分支 `main`、常用别名，一次设置终身受益：
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   git config --global init.defaultBranch main
   ```
3. 出事时直奔"救命命令"区：`reflog` 能找回几乎所有"丢失"的提交。

## 收录了什么

| 分类 | 内容 |
|---|---|
| ⚙️ 配置 | 身份、默认分支、命令别名 |
| 📅 日常 | 状态、暂存、提交、看日志 |
| ↩️ 撤销 | 取消暂存、丢弃改动、reset 三档、revert |
| 🌿 分支 | 建分支、合并 `--no-ff`、删本地/远端分支 |
| 🔁 Rebase | 变基、交互式整理、`--continue/--abort`、黄金法则 |
| 📦 储藏 | stash 存取、列表、按名取回 |
| 🌐 远程 | remote、fetch 修剪、pull --rebase、发布分支 |
| 🆘 救命 | reflog 找回提交、cherry-pick、bisect 定位 bug |
| 🚀 高级 | worktree、submodule、浅克隆 |

所有命令均为真实 git 语法（参考 https://git-scm.com/doc），危险操作（`reset --hard`、`push --force`）均有明确警告。

## 为什么是这 30 条

- **救命优先**：reflog、reset 三档、rebase 黄金法则是真实生产事故里最常用的。
- **实战不理论**：不讲 git 内部原理，只给"出事了敲什么"。
- **危险标红线**：会丢数据的命令都标了 ⚠️，先看说明再敲。

## 欢迎 PR

命令写错了、漏了常用场景、翻译不到位——欢迎提 Pull Request。新增条目请保持统一格式（标题 / 一句话 / 代码块 / 标签），**提交前请核实命令真实可用**。

## License

MIT © 2026 Guangyi Zhao，详见 [LICENSE](LICENSE)。
