<div align="center">

# Yohanes · CryoThrust

**Java 后端工程师 · AI 应用构建者**

专注于构建面向生产环境的后端系统与实用型 AI 应用。

<a href="https://github.com/CryoThrust?tab=repositories">项目</a> ·
<a href="https://github.com/CryoThrust/openai-codex-adapter">AI 基础设施</a> ·
<a href="https://github.com/CryoThrust/agent-skills">Agent 工具链</a>

</div>

## 我在做什么

- **后端系统** — Java、Spring Boot、MyBatis、微服务、Redis、消息中间件与分布式系统。
- **AI 应用** — RAG 流程、知识工程、混合检索、知识图谱与工具调用 Agent。
- **工程质量** — 可观测性、效果评估、性能调优与清晰可维护的系统边界。

## 自主构建与维护

| 项目 | 技术与工程实践 |
| --- | --- |
| [openai-codex-adapter](https://github.com/CryoThrust/openai-codex-adapter) | OpenAI Chat Completions 与 Codex Responses API 的兼容适配层，包含重试处理。 |
| [agent-skills](https://github.com/CryoThrust/agent-skills) | 面向 AI Agent 的可复用 Skill 集合，包含架构图生成能力。 |
| [codex-claude-executor](https://github.com/CryoThrust/codex-claude-executor) | Codex 插件实践：委托实现任务，同时保留独立验证流程。 |
| [Sesh](https://github.com/CryoThrust/Sesh) | 用于浏览和管理 Claude Code 会话的原生 macOS 工具。 |
| [ClaudeSessionManager](https://github.com/CryoThrust/ClaudeSessionManager) | 用于浏览和管理 Claude Code 会话的 macOS 工具。 |

## 开源贡献

### [neutrino-proxy](https://github.com/dromara/neutrino-proxy) · 贡献者 · ⭐ 700+

参与一个高星开源内网代理项目的生产修复与功能开发：

- 改进端口映射管理，包括端口分组、搜索与排序。
- 完善管理流程中的参数校验与数据库迁移。
- 修复端口组选择和映射行为相关问题。

贡献证据：[端口映射](https://github.com/dromara/neutrino-proxy/commit/e725cdbb2841c5f4cc520e4dca4b869754b09f98) · [问题修复](https://github.com/dromara/neutrino-proxy/commit/559c6bd5f548a109cbaeaeefee6ee4e2a0b1f964) · [参数校验](https://github.com/dromara/neutrino-proxy/commit/a5c568392b05d204ac66c408705ffe6ecd7b19cd)

### [spring-ai-alibaba](https://github.com/alibaba/spring-ai-alibaba) · 贡献者 · ⭐ 10k+

针对渐进式工具披露提出修复：保留外部维护的初始空 `groupedTools`，使 Agent 创建后新增的工具无需重建拦截器即可生效。

贡献证据：[PR #4935](https://github.com/alibaba/spring-ai-alibaba/pull/4935) · [Issue #4929](https://github.com/alibaba/spring-ai-alibaba/issues/4929)

### [OpenViking](https://github.com/volcengine/OpenViking) · 贡献者 · ⭐ 30k+

修复搜索接口在 `context_type=skill` 且未指定目标 URI 时遗漏共享 Agent Skill 目录的问题，将上下文类型贯通到隐式检索目标解析，并补充 `find/search` 回归测试。

贡献证据：[PR #4423](https://github.com/volcengine/OpenViking/pull/4423) · [Issue #3739](https://github.com/volcengine/OpenViking/issues/3739)

### [MCP Servers](https://github.com/modelcontextprotocol/servers) · 贡献者 · ⭐ 80k+

修复 filesystem server 在 1024 字节分块边界切分多字节 UTF-8 字符时产生乱码的问题，分别为 `head` 与 `tail` 路径增加跨块安全解码处理。

贡献证据：[PR #4703](https://github.com/modelcontextprotocol/servers/pull/4703) · [Issue #4666](https://github.com/modelcontextprotocol/servers/issues/4666)

补充修复：[PR #4704](https://github.com/modelcontextprotocol/servers/pull/4704) · [Issue #4686](https://github.com/modelcontextprotocol/servers/issues/4686)：在 POSIX 环境拒绝 Windows 盘符路径，避免跨平台路径被静默当作相对路径写入错误位置。

## 技术关注

持续研究并借鉴这些项目中的 AI 工程实践。它们是我关注的上游项目，不代表我的原创项目。

| 方向 | 参考项目 | 关注点 |
| --- | --- | --- |
| Agent 上下文与记忆 | [OpenViking](https://github.com/volcengine/OpenViking) · [Mem0](https://github.com/mem0ai/mem0) <br> ![stars](https://img.shields.io/github/stars/volcengine/OpenViking?style=flat-square) ![stars](https://img.shields.io/github/stars/mem0ai/mem0?style=flat-square) | 持久化上下文、Agent 记忆与可复用知识。 |
| Agent 编排 | [LangGraph](https://github.com/langchain-ai/langgraph) <br> ![stars](https://img.shields.io/github/stars/langchain-ai/langgraph?style=flat-square) | 面向高可靠 Agent 的有状态、可控工作流。 |
| 工具互操作 | [MCP servers](https://github.com/modelcontextprotocol/servers) <br> ![stars](https://img.shields.io/github/stars/modelcontextprotocol/servers?style=flat-square) | 连接 Agent、工具与数据的通用协议。 |
| RAG 基础设施 | [RAGFlow](https://github.com/infiniflow/ragflow) <br> ![stars](https://img.shields.io/github/stars/infiniflow/ragflow?style=flat-square) | 面向生产环境的检索与 Agent 上下文流程。 |

我最关注 **有依据的生成**、**有状态工具调用**、**可观测评估** 与 **可靠恢复**：这决定了一个系统只是演示效果惊艳，还是能够真正被依赖。

## 当前重点

```text
RAG 质量         → 检索、重排、可溯源生成、效果评估
Agent 系统       → 工具调用、状态、编排、故障恢复
后端设计         → 清晰边界、可靠流程、可观测服务
```

## 技术栈

`Java` `Spring Boot` `MyBatis` `Spring Cloud Alibaba` `MySQL` `Redis`

`RocketMQ` `RabbitMQ` `Kafka` `Docker` `Linux` `Nginx`

`RAG` `Embedding` `Hybrid Retrieval` `Neo4j` `GraphRAG` `LightRAG`

`Agent` `Function Calling` `Langfuse` `MinerU`

## 我的工程理念

> 一个有价值的系统不只是能跑通的 Demo：它应该具备清晰的数据边界、可观测的行为、可度量的质量，以及面对真实复杂情况时的恢复路径。

<div align="center">

![Profile views](https://komarev.com/ghpvc/?username=CryoThrust&style=flat-square&color=4f46e5)

</div>
