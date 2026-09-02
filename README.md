<div align="center">

# Yohanes

尽我所能，尽我所不能

Do what I can, attempt what I cannot

</div>

---

## 开源贡献 / Open Source

**[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers)**

MCP 官方服务器实现。修复 filesystem server 在 POSIX 环境下错误接受 Windows 路径的问题。

Official MCP server implementations. Fixed Windows-path validation in the filesystem server on POSIX systems.

> [#4704](https://github.com/modelcontextprotocol/servers/pull/4704) ✅ 修复 POSIX 下 Windows 路径校验 / Reject Windows paths on POSIX systems

**[agentic-spring-ai/agentic-spring-ai](https://github.com/agentic-spring-ai/agentic-spring-ai)**

Spring AI Agent 框架。修复渐进式工具披露与 filesystem tools schema，补充回归测试。

Spring AI Agent framework. Fixed dynamic grouped tools and filesystem tool schemas with regression coverage.

> [#22](https://github.com/agentic-spring-ai/agentic-spring-ai/pull/22) ✅ 修复 grouped tools 动态更新 / Fix dynamic grouped tools update
> [#53](https://github.com/agentic-spring-ai/agentic-spring-ai/pull/53) ✅ 补全 filesystem tools object schema / Expose filesystem tool object schemas

**[langchain4j/langchain4j](https://github.com/langchain4j/langchain4j)**

Java LLM 应用框架。为 Agent 与 MCP 参数补充描述传播，覆盖注解解析、Planner 展示与 MCP schema；当前全部 CI 已通过，等待维护者评审。

Java framework for LLM applications. Preserved Agent and MCP argument descriptions across annotations, planner rendering, and MCP schemas; all CI checks pass and maintainer review is pending.

> [#6241](https://github.com/langchain4j/langchain4j/pull/6241) ⏳ Agent/MCP 参数描述传播 / Preserve Agent and MCP argument descriptions

**[agentscope-ai/agentscope-java](https://github.com/agentscope-ai/agentscope-java)**

Java Agent 框架。修复本地 shell 执行在大输出场景下因 stdout/stderr 管道未及时消费而死锁的问题，并补充跨平台回归测试。

Java agent framework. Fixed a pipe-buffer deadlock in local shell execution for large stdout/stderr output and added cross-platform regression coverage.

> [#2936](https://github.com/agentscope-ai/agentscope-java/pull/2936) ⏳ CI 全部通过，等待 CLA 与维护者评审 / All CI checks passed; awaiting CLA verification and maintainer review

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
