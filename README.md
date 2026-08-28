<div align="center">

# Yohanes · CryoThrust

**Java 后端工程师 / AI 应用工程师**

面向真实业务构建可靠的后端系统、RAG 流程与工具调用 Agent。

[项目](https://github.com/CryoThrust?tab=repositories) · [开源贡献](#开源贡献) · [技术方向](#技术方向)

</div>

## 我关注的问题

我更关心 AI 系统落地后的工程问题：上下文如何管理、检索结果如何评估、工具调用如何恢复、服务行为如何观测。

```text
RAG       检索 / 重排 / 依据链 / 评估
Agent     工具调用 / 状态 / 编排 / 恢复
Backend   Java / Spring / 分布式系统 / 可观测性
```

## 自主构建

| 项目 | 简介 |
| --- | --- |
| [openai-codex-adapter](https://github.com/CryoThrust/openai-codex-adapter) | OpenAI Chat Completions 与 Codex Responses API 的协议适配层，包含重试与兼容处理。 |
| [agent-skills](https://github.com/CryoThrust/agent-skills) | 面向 Agent 的可复用 Skill 与工程工作流，覆盖架构图等常见研发任务。 |
| [codex-claude-executor](https://github.com/CryoThrust/codex-claude-executor) | Agent 委托执行插件：拆分实现与验证，保留可审查的执行边界。 |
| [Sesh](https://github.com/CryoThrust/Sesh) | 原生 macOS 会话管理工具，用于浏览和整理 Claude Code 工作记录。 |

## 开源贡献

以下内容均链接到公开 Issue、PR 或 commit；尚未合并的工作明确标注为进行中。

| 项目 | 贡献内容 | 状态 |
| --- | --- | --- |
| [neutrino-proxy](https://github.com/dromara/neutrino-proxy) | 端口映射管理、参数校验、数据库迁移与端口组行为修复。<br>[commit 证据](https://github.com/dromara/neutrino-proxy/commit/e725cdbb2841c5f4cc520e4dca4b869754b09f98) | 已提交 |
| [spring-ai-alibaba](https://github.com/alibaba/spring-ai-alibaba) | 修复 Agent 渐进式工具披露中空 `groupedTools` Map 无法动态更新的问题，并补充回归测试。<br>[PR #4935](https://github.com/alibaba/spring-ai-alibaba/pull/4935) · [Issue #4929](https://github.com/alibaba/spring-ai-alibaba/issues/4929) | Review 中 |
| [OpenViking](https://github.com/volcengine/OpenViking) | 修复 `context_type=skill` 的隐式检索目标解析，以及记忆合并中重复行号前缀累积。<br>[PR #4423](https://github.com/volcengine/OpenViking/pull/4423) · [PR #4424](https://github.com/volcengine/OpenViking/pull/4424) | Review 中 |
| [MCP Servers](https://github.com/modelcontextprotocol/servers) | 修复 filesystem 的 UTF-8 分块边界乱码与 POSIX 环境 Windows 路径误解析。<br>[PR #4703](https://github.com/modelcontextprotocol/servers/pull/4703) · [PR #4704](https://github.com/modelcontextprotocol/servers/pull/4704) | CI 通过，Review 中 |

## 技术方向

我持续阅读和实践这些项目中的工程模式，它们是参考项目，不代表我的原创工作：

- **Agent 上下文与记忆**： [OpenViking](https://github.com/volcengine/OpenViking) · [Mem0](https://github.com/mem0ai/mem0)
- **有状态 Agent 编排**： [LangGraph](https://github.com/langchain-ai/langgraph)
- **工具互操作协议**： [MCP Servers](https://github.com/modelcontextprotocol/servers)
- **生产级 RAG**： [RAGFlow](https://github.com/infiniflow/ragflow)

## 技术栈

`Java` `Spring Boot` `MyBatis` `Spring Cloud Alibaba` `MySQL` `Redis`

`RocketMQ` `RabbitMQ` `Kafka` `Docker` `Linux` `Nginx`

`RAG` `Embedding` `Hybrid Retrieval` `Neo4j` `GraphRAG` `LightRAG`

`Agent` `Function Calling` `MCP` `Langfuse` `MinerU`

## 工程原则

> 一个能运行的 Demo 只是起点。真正可依赖的系统，还需要清晰的数据边界、可观测的行为、可度量的质量，以及面对异常时的恢复路径。
