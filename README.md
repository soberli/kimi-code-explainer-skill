# 🔍 Code Explainer Skill for Kimi Code CLI

一个 [Kimi Code CLI](https://github.com/MoonshotAI/Kimi-Chat) 的 Skill，用于生成**结构化、深度化的源码解析文档**。

当你需要理解一段代码的架构逻辑、设计思想，或者准备技术分享时，这个 Skill 可以帮助你快速产出高质量的代码讲解文档。

---

## ✨ 功能特性

- **结构化输出**：统一的 8 部分文档格式，从宏观架构到微观实现逐层深入
- **设计导向**：不仅解释"代码做了什么"，更深入分析"为什么这样设计"
- **AI 时代架构思维**：每篇解析末尾提炼核心设计哲学、架构模式，以及 AI 时代的可维护性启示
- **多语言支持**：适用于 Python、JavaScript、Java、Go、Rust 等任何编程语言
- **故障隔离与防御性编程**：特别标注异常处理、边界条件、降级策略等工程实践

---

## 📦 安装

将本仓库克隆到 Kimi Code CLI 的 skills 目录：

```bash
# macOS / Linux
git clone https://github.com/soberli/kimi-code-explainer-skill.git ~/.kimi/skills/code-explainer

# Windows
# 克隆到 Kimi skills 目录，通常为：
# C:\Users\<你的用户名>\.kimi\skills\code-explainer
```

或者直接在 Kimi Code CLI 中使用 `--skills-dir` 参数指定。

---

## 🚀 使用方法

安装后，在 Kimi Code CLI 中直接提出代码讲解请求即可自动触发：

> "请讲解这段代码"
> 
> "分析一下这个文件的源码"
> 
> "解读一下 monitor.py 的实现逻辑"
> 
> "帮我 review 这段代码的架构设计"

---

## 📝 输出格式

Skill 生成的文档包含以下 8 个部分：

| 章节 | 内容 |
|------|------|
| 1. 文件概述 | 定位、核心能力 |
| 2. 整体架构 | 组成部分与职责表格 |
| 3~N. 逐部分详细讲解 | 代码块 + 核心逻辑说明表格 |
| 4. 流程/设计对照表 | 步骤与关键设计对照 |
| 5. 协作关系图 | ASCII 调用关系与数据流向 |
| 6. 核心设计亮点 | 优秀设计总结表格 |
| 7. 设计理念与架构思维 | ⭐ 核心哲学、架构模式、AI 时代启示、可迁移经验 |

---

## 🎯 示例场景

### 场景 1：理解新项目代码

刚接手一个项目，需要快速理解某个核心模块的实现：

> "请讲解 `app/services/monitor.py` 的源码"

Skill 将输出完整的架构分析，帮助你 5 分钟抓住核心设计。

### 场景 2：技术分享准备

准备团队内部的技术分享，需要结构化的讲解材料：

> "分析 `async_task_scheduler.py` 的设计，侧重并发模型和故障隔离"

Skill 会自动梳理出适合分享的表格、流程图和亮点总结。

### 场景 3：代码 Review

Review 同事提交的代码，需要系统性地评估架构质量：

> "解读这个 PR 中 `notification_manager.py` 的设计思想"

Skill 会标注防御性编程、异常处理、事务边界等工程实践。

---

## 🏗️ 架构模式识别

Skill 会在解析中识别以下常见架构模式：

- 管道-过滤器（Pipeline-Filter）
- 发布-订阅（Pub-Sub）
- 分层架构（Layered Architecture）
- 事件驱动（Event-Driven）
- CQRS（命令查询职责分离）
- 策略模式（Strategy Pattern）
- ...以及更多

---

## 🤝 贡献

如果你有改进建议，或者希望添加更多架构模式的识别规则，欢迎提交 Issue 或 Pull Request。

---

## 📄 License

MIT License © 2025 soberli
