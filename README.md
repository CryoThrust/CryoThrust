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
> [#4731](https://github.com/modelcontextprotocol/servers/pull/4731) ⏳ 修复 memory server 对 undefined observation 的处理，CI 通过 / Guard undefined observations in memory search; CI green

**[alibaba/spring-ai-alibaba](https://github.com/alibaba/spring-ai-alibaba)**

Spring AI Alibaba Agent 框架。修复 filesystem 工具的输入 schema，使动态工具调用符合 MCP object schema 约定。

Spring AI Alibaba agent framework. Fixed filesystem tool input schemas so dynamically exposed tools follow the MCP object-schema contract.

> [#4942](https://github.com/alibaba/spring-ai-alibaba/pull/4942) ⏳ 修复 ls/glob filesystem tools 的 object schema / Use object input schemas for `ls` and `glob` filesystem tools

**[langgenius/dify](https://github.com/langgenius/dify)**

重点关注 Dify 的 Agent、RAG、MCP 与插件运行时问题。目前已核查近期高优先级 issue：可复现的 Skill CRLF 导入、MCP provider 参数校验、凭据权限等问题均已有对应 PR，因此暂不重复提交。

Tracking Dify's Agent, RAG, MCP, and plugin runtime work. Recent high-priority issues—including Skill CRLF imports, MCP provider validation, and credential permissions—were checked and already have corresponding PRs, so no duplicate changes are proposed.

> #41675 🔎 plugin-daemon restart is surfaced as `400 invalid_param`; source-level exception mapping still under review / dependency failure should be distinguishable from invalid input

**[agentic-spring-ai/agentic-spring-ai](https://github.com/agentic-spring-ai/agentic-spring-ai)**

Spring AI Agent 框架。修复渐进式工具披露与 filesystem tools schema，补充回归测试。

Spring AI Agent framework. Fixed dynamic grouped tools and filesystem tool schemas with regression coverage.

> [#22](https://github.com/agentic-spring-ai/agentic-spring-ai/pull/22) ✅ 修复 grouped tools 动态更新 / Fix dynamic grouped tools update
> [#53](https://github.com/agentic-spring-ai/agentic-spring-ai/pull/53) ✅ 补全 filesystem tools object schema / Expose filesystem tool object schemas

**[langchain4j/langchain4j](https://github.com/langchain4j/langchain4j)**

Java LLM 应用框架。为 Agent 与 MCP 参数补充描述传播，覆盖注解解析、Planner 展示与 MCP schema，并补充参数名与描述并存时的 Planner 集成测试。

Java framework for LLM applications. Preserved Agent and MCP argument descriptions across annotations, planner rendering, and MCP schemas, with integration coverage for planner argument resolution when names and descriptions coexist.

> [#6241](https://github.com/langchain4j/langchain4j/pull/6241) ✅ 已合并 / Merged
> [#6250](https://github.com/langchain4j/langchain4j/pull/6250) ⏳ MCP 工具结果支持 image/resource content；JDK 25 检查为环境性超时 / Support image and resource content in MCP tool results; JDK 25 check has an unrelated environment timeout
> [#6268](https://github.com/langchain4j/langchain4j/pull/6268) ⏳ 按 `@Tool(name = ...)` 解析工具执行器；CI 全通过，等待评审 / Resolve tool executors by custom `@Tool(name = ...)`; all CI checks green, awaiting review

**[agentscope-ai/agentscope-java](https://github.com/agentscope-ai/agentscope-java)**

Java Agent 框架。修复本地 shell 执行在大输出场景下因 stdout/stderr 管道未及时消费而死锁的问题，并补充跨平台回归测试。

Java agent framework. Fixed a pipe-buffer deadlock in local shell execution for large stdout/stderr output and added cross-platform regression coverage.

> [#2936](https://github.com/agentscope-ai/agentscope-java/pull/2936) ⏳ CI 全部通过，等待 CLA 与维护者评审 / All CI checks passed; awaiting CLA verification and maintainer review

**[quarkiverse/quarkus-langchain4j](https://github.com/quarkiverse/quarkus-langchain4j)**

Quarkus 的 LangChain4j 集成。修复 Anthropic 客户端在程序化构造且未设置 timeout 时的空指针问题，补充构造级回归测试。

Quarkus integration for LangChain4j. Fixed the null timeout path when constructing the Anthropic client programmatically and added focused construction coverage.

> [#2800](https://github.com/quarkiverse/quarkus-langchain4j/pull/2800) ⏳ 修复 Anthropic 默认 timeout / Fix Anthropic default timeout

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
