# 书写约束插件

`writing-constraints` 包含三个 Codex skill。你可通过 skills 目录加载，也可使用插件命令安装。

| Skill | 用途 | 调用方式 |
| --- | --- | --- |
| `asd-ste100` | 提高技术文档的清晰度，保留技术含义和要求强度 | 自动选择或显式调用 |
| `stop-slop` | 去除散文和文档中的 AI 写作套路 | 自动选择或显式调用 |
| `basic-qa-notes` | 回答项目问题，维护可复用的项目笔记 | 显式调用 |

Codex 按各 skill 的适用范围选择规则，沿用原有内容和调用策略。Codex 仅在当前用户消息中收到 `basic-qa-notes` 的显式调用时使用该 skill，回答项目问题并维护笔记。

## 安装

### 通过 skills 目录加载

将整个 `writing-constraints` 目录放到 `~/.codex/skills/` 下，然后开启新会话。Codex CLI 0.162.0 支持从 `~/.codex/skills/writing-constraints/skills/` 发现三个 skill；使用这种方式时，无需注册 marketplace 或执行 `codex plugin add`。

### 使用插件命令安装

解压 ZIP，进入 `writing-constraints` 目录，执行：

```bash
codex plugin marketplace add .
codex plugin add writing-constraints@writing-tools
```

安装后开启新会话。此包包含本地 marketplace 清单，无需发布到远程市场。

## 使用

- 技术文档：使用 `$asd-ste100` 审查这份操作指南，保留命令、数值和要求强度。
- 文风修改：使用 `$stop-slop` 编辑这篇文章，去掉空话和套路句式。
- 项目笔记：使用 `$basic-qa-notes` 回答这个项目问题，并记录有复用价值的结论。

你可结合 `asd-ste100` 和 `stop-slop` 编辑技术文档。修改文风时，需保留原意、术语和要求强度。编辑中文文档时，可参考清晰度原则，但不能据此声称文档符合 ASD-STE100 英文标准。

## 内容

- `LICENSE`：项目的 MIT 许可证。
- `.codex-plugin/plugin.json`：插件名称、版本和描述。
- `.agents/plugins/marketplace.json`：本地安装入口。
- `skills/`：三个完整 skill，包含原有引用资料和许可证。

已使用 Codex CLI 0.162.0 在临时配置目录中验证 marketplace 注册和插件安装，并通过三个 skill 的结构校验。

## 许可证

本项目采用 MIT License，详见 [LICENSE](LICENSE)。项目原创内容的版权声明为 `Copyright (c) 2026 ligeng`。

- `asd-ste100` 和 `basic-qa-notes` 使用 `skill-creator` 创建，适用根目录的 MIT 许可证。
- `stop-slop` 集成自 Hardik Pandya 的作品，同样采用 MIT License。其原有版权声明 `Copyright (c) 2025 Hardik Pandya` 和许可证保留在 [skills/stop-slop/LICENSE](skills/stop-slop/LICENSE)。

复制或分发本项目时，须保留适用的版权声明和许可证文本，包括 `stop-slop` 的原有声明。
