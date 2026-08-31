<div align="center">

# Yohanes

尽我所能，尽我所不能

Do what I can, attempt what I cannot

</div>

---

## 开源贡献 / Open Source

**[volcengine/OpenViking](https://github.com/volcengine/OpenViking)**

字节跳动 AI Agent 上下文数据库。持续贡献 6 个 PR，覆盖检索、记忆、知识图谱、会话恢复等核心模块。

ByteDance's AI Agent context database. 6 PRs across retrieval, memory, knowledge graph, and session recovery modules.

> [#4423](https://github.com/volcengine/OpenViking/pull/4423) 检索目标解析修复 / Retrieval target parsing fix
> [#4424](https://github.com/volcengine/OpenViking/pull/4424) 记忆文本规范化 / Memory text normalization
> [#4432](https://github.com/volcengine/OpenViking/pull/4432) 多模态 embedding 配置 / Multimodal embedding configuration
> [#4435](https://github.com/volcengine/OpenViking/pull/4435) 知识图谱展示修复 / Knowledge graph display fix
> [#4437](https://github.com/volcengine/OpenViking/pull/4437) 会话恢复重试机制 / Session recovery retry mechanism
> [#4507](https://github.com/volcengine/OpenViking/pull/4507) RAGFS 锁错误诊断 / RAGFS lock error diagnosis

**[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers)**

Anthropic 官方 MCP 协议实现。修复 filesystem server 和 POSIX 环境下的路径解析问题。

Anthropic's official MCP implementation. Fixed filesystem server UTF-8 chunk boundary and POSIX path parsing issues.

> [#4704](https://github.com/modelcontextprotocol/servers/pull/4704) ✅ 修复 UTF-8 分块边界 / Fix UTF-8 chunk boundary in filesystem server
> [#4703](https://github.com/modelcontextprotocol/servers/pull/4703) 修复 POSIX 下 Windows 路径误解析 / Fix Windows path parsing on POSIX systems

**[agentic-spring-ai/agentic-spring-ai](https://github.com/agentic-spring-ai/agentic-spring-ai)**

Spring AI Agent 框架。修复渐进式工具披露中 grouped tools 动态更新，补充回归测试。

Spring AI Agent framework. Fixed dynamic grouped tools update in progressive tool disclosure, added regression tests.

> [#22](https://github.com/agentic-spring-ai/agentic-spring-ai/pull/22) ✅ 修复 grouped tools 动态更新 / Fix dynamic grouped tools update

**[dromara/neutrino-proxy](https://github.com/dromara/neutrino-proxy)**

内网穿透代理。端口映射、参数校验、数据库迁移与端口组行为修复。

NAT traversal proxy. Port mapping, parameter validation, DB migration and port group behavior fixes.

> [e725cdb](https://github.com/dromara/neutrino-proxy/commit/e725cdbb2841c5f4cc520e4dca4b869754b09f98)

---

## 原创项目 / Projects

**[openai-codex-adapter](https://github.com/CryoThrust/openai-codex-adapter)**

OpenAI Chat Completions ↔ Codex Responses API 协议适配层，覆盖流式事件、重试与兼容性处理。

Protocol adapter between OpenAI Chat Completions and Codex Responses API. Streaming events, retry logic, and compatibility handling.

**[codex-claude-executor](https://github.com/CryoThrust/codex-claude-executor)**

Codex 插件：将实现委托给 Claude Code，Codex 独立验证。实现、验证、审查边界清晰。

Codex plugin that delegates implementation to Claude Code with independent verification. Clean boundaries between implementation, verification, and review.

**[Sesh](https://github.com/CryoThrust/Sesh)**

原生 macOS Claude Code 会话管理工具，浏览、搜索、管理开发会话。

Native macOS app for browsing, searching, and managing Claude Code sessions.

**[agent-skills](https://github.com/CryoThrust/agent-skills)**

面向 Agent 研发的可复用工作流与工程化 Skill。

Reusable workflows and engineering skills for AI agent development.

---

> *Reliable AI systems are built at the boundaries: state, protocols, data, and failure recovery.*
