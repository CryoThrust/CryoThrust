<div align="center">

# Yohanes

**Java Backend · AI Systems**

把模型能力落到可靠的后端系统：可观测、可恢复、可演进。

[精选项目](#精选项目) · [开源贡献](#开源贡献) · [技术栈](#技术栈)

</div>

## 关注方向

面向真实业务中的 AI 系统，重点处理上下文、检索、工具调用和长任务执行的工程边界。

| 方向 | 工程关注点 |
| --- | --- |
| **RAG** | 混合检索、重排、知识图谱、依据链与质量评估 |
| **Agent** | 工具协议、状态编排、记忆、任务恢复与可观测性 |
| **Backend** | Java / Spring、分布式系统、消息驱动与服务治理 |

## 精选项目

| 项目 | 说明 |
| --- | --- |
| [openai-codex-adapter](https://github.com/CryoThrust/openai-codex-adapter) | OpenAI Chat Completions 与 Codex Responses API 的协议适配层，覆盖流式事件、重试与兼容性处理。 |
| [agent-skills](https://github.com/CryoThrust/agent-skills) | 面向 Agent 研发的可复用工作流与工程化 Skill。 |
| [codex-claude-executor](https://github.com/CryoThrust/codex-claude-executor) | 将实现委托、验证和审查拆分为清晰边界的 Codex 插件。 |
| [Sesh](https://github.com/CryoThrust/Sesh) | 原生 macOS 开发会话管理工具。 |

## 开源贡献

公开 Issue、PR 和 commit 是这部分内容的唯一依据。

| 项目 | 贡献主题 | 公开记录 |
| --- | --- | --- |
| [agentic-spring-ai](https://github.com/agentic-spring-ai/agentic-spring-ai) | 修复 Agent 渐进式工具披露中的动态 grouped tools 更新问题，并补充回归测试。 | [PR #22（已合并）](https://github.com/agentic-spring-ai/agentic-spring-ai/pull/22) · [commit 8c65205](https://github.com/agentic-spring-ai/agentic-spring-ai/commit/8c65205bd2c75531054e11cf7ee3fce41348432f) |
| [OpenViking](https://github.com/volcengine/OpenViking) | 检索目标解析、记忆文本规范化、多模态 embedding 配置、知识图谱展示、会话恢复重试与 RAGFS 锁错误诊断。 | [#4423](https://github.com/volcengine/OpenViking/pull/4423) · [#4424](https://github.com/volcengine/OpenViking/pull/4424) · [#4432](https://github.com/volcengine/OpenViking/pull/4432) · [#4435](https://github.com/volcengine/OpenViking/pull/4435) · [#4437](https://github.com/volcengine/OpenViking/pull/4437) · [#4507](https://github.com/volcengine/OpenViking/pull/4507) |
| [MCP Servers](https://github.com/modelcontextprotocol/servers) | 修复 filesystem 的 UTF-8 分块边界处理与 POSIX 环境下的 Windows 路径误解析。 | [#4704（已合并）](https://github.com/modelcontextprotocol/servers/pull/4704) · [#4703](https://github.com/modelcontextprotocol/servers/pull/4703) |
| [neutrino-proxy](https://github.com/dromara/neutrino-proxy) | 端口映射、参数校验、数据库迁移与端口组行为修复。 | [commit e725cdb](https://github.com/dromara/neutrino-proxy/commit/e725cdbb2841c5f4cc520e4dca4b869754b09f98) |

## 技术栈

`Java` `Spring Boot` `MyBatis` `Spring Cloud Alibaba` `MySQL` `Redis`

`RocketMQ` `RabbitMQ` `Kafka` `Docker` `Linux` `Nginx`

`RAG` `Embedding` `Hybrid Retrieval` `Neo4j` `GraphRAG` `LightRAG`

`Agent` `Function Calling` `MCP` `Langfuse` `MinerU`

## 开源协作

从可复现的问题出发，提交小而完整的修复，用测试、CI 和公开讨论建立长期信任。当前重点是持续参与 RAG、Agent、工具协议和后端基础设施项目，逐步承担更多 review、维护和发布责任。

> Reliable AI systems are built at the boundaries: state, protocols, data, and failure recovery.
