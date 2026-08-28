<div align="center">

# Yohanes

**Java 后端工程师 · AI 应用工程师**

把模型能力做成可运行、可观测、可恢复的工程系统。

[精选项目](#精选项目) · [开源贡献](#开源贡献) · [技术栈](#技术栈)

</div>

## 我在做什么

我关注 AI 系统进入真实业务后的工程问题：上下文如何管理，检索结果如何评估，工具调用如何恢复，以及服务行为如何观测。

```text
RAG       检索 / 重排 / 依据链 / 评估
Agent     工具调用 / 状态 / 编排 / 恢复
Backend   Java / Spring / 分布式系统 / 可观测性
```

## 精选项目

| 项目 | 简介 |
| --- | --- |
| [openai-codex-adapter](https://github.com/CryoThrust/openai-codex-adapter) | **协议适配与兼容性**：连接 Chat Completions 与 Codex Responses API，处理重试、流式响应和协议差异。 |
| [agent-skills](https://github.com/CryoThrust/agent-skills) | **Agent 工程工作流**：沉淀可复用 Skill，把复杂研发任务拆成可验证的步骤。 |
| [codex-claude-executor](https://github.com/CryoThrust/codex-claude-executor) | **委托执行边界**：分离实现、验证与审查，保留清晰的执行上下文。 |
| [Sesh](https://github.com/CryoThrust/Sesh) | **开发效率工具**：原生 macOS 会话管理工具，用于浏览和整理 Claude Code 工作记录。 |

## 开源贡献

以下内容均链接到公开 Issue、PR 或 commit；尚未合并的工作明确标注为进行中。

| 项目 | 贡献内容 | 状态 |
| --- | --- | --- |
| [neutrino-proxy](https://github.com/dromara/neutrino-proxy) | 端口映射管理、参数校验、数据库迁移与端口组行为修复。<br>[commit 证据](https://github.com/dromara/neutrino-proxy/commit/e725cdbb2841c5f4cc520e4dca4b869754b09f98) | 已提交 |
| [spring-ai-alibaba](https://github.com/alibaba/spring-ai-alibaba) | 修复 Agent 渐进式工具披露中空 `groupedTools` Map 无法动态更新的问题，并补充回归测试。<br>[PR #4935](https://github.com/alibaba/spring-ai-alibaba/pull/4935) · [Issue #4929](https://github.com/alibaba/spring-ai-alibaba/issues/4929) | Review 中 |
| [OpenViking](https://github.com/volcengine/OpenViking) | 修复 `context_type=skill` 的隐式检索目标解析、记忆合并中的重复行号前缀累积，以及 OpenAI-compatible embedding 的显式多模态配置透传。<br>[PR #4423](https://github.com/volcengine/OpenViking/pull/4423) · [PR #4424](https://github.com/volcengine/OpenViking/pull/4424) · [PR #4432](https://github.com/volcengine/OpenViking/pull/4432) | Review 中 |
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

## 工作方式

- 从公开 Issue 或可复现问题出发，先缩小影响范围，再提交最小修复。
- 用回归测试、CI 和可追溯链接说明改动，而不是只描述概念。
- 优先处理边界条件：编码、路径、状态、上下文和失败恢复。

## 工程原则

> 一个能运行的 Demo 只是起点。真正可依赖的系统，还需要清晰的数据边界、可观测的行为、可度量的质量，以及面对异常时的恢复路径。
