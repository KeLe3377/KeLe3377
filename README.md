<div align="center">

# KeLe3377

**AI Agent 工程 · LLM 应用落地**

关注 Agent 编排架构、混合检索与 LLM 系统的稳定性

把「能跑通的 Demo」做成「敢长期跑的系统」

[![GitHub](https://img.shields.io/badge/GitHub-KeLe3377-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/KeLe3377)

</div>

---

## 在做什么

- 🧭 **Agent 编排**：意图识别 → 领域路由 → 规划/执行 → 工具调用 → 结果合成，研究 ReAct、Plan-and-Execute 与多视角审议的适用边界
- 🔍 **检索质量**：向量 + 关键词混合召回、RRF 融合、二阶段 reranker，以及表格 / 长文档等异构资料的切块与结构化过滤
- 🛡️ **稳定性治理**：熔断、降级、主备模型路由、Trace 全链路追踪，让 Agent 在真实业务里不崩、可定位
- 🧱 **知识资产化**：把领域规则、库结构、查询范式沉淀为可复用的 Skill，而不是散落在提示词里
- 🧪 **评测驱动**：先建立可回归的评测集与 Golden Case，再谈效果提升

---

## 技术栈

| 分类 | 技术 |
| :--- | :--- |
| **大模型应用** | LangGraph · Agent Workflow · Tool Calling · ReAct · Plan-and-Execute · 多智能体审议 · Prompt Engineering · RAG |
| **检索与数据** | Milvus · BM25 · RRF 融合 · Reranker · 结构化切块 · PostgreSQL / MySQL / Oracle / SQLite · Redis |
| **后端工程** | Python · FastAPI · SSE 流式 · Docker · 熔断 / 降级 / 主备路由 · Trace 全链路追踪 |
| **工程化** | 测试驱动开发 (TDD) · Pytest · Agent 评估体系 · Golden Case 回归 · CI 与自动化交付 |
| **其他** | Rust (GPUI 桌面端) · TypeScript / Node · Vue · Git |

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Milvus](https://img.shields.io/badge/Milvus-00A1EA?style=flat-square&logo=milvus&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

</div>

---



### 🖥️ ContextOS — 面向 AI 编程 Agent 的桌面工作台

> 把分散在本机各个 Agent 中的会话、项目改动与可复用上下文集中起来：可搜索历史、查看变更、整理记忆，并通过 MCP 或 CLI 继续组合这些能力。

`Rust` `GPUI` `MCP` `CLI` `桌面应用`

- **统一会话浏览**：内置适配器覆盖 Claude Code、Codex、Cursor、Gemini CLI、OpenCode、Copilot CLI、Kimi Code、CodeBuddy 等十余种 Agent，支持全文搜索、按 Agent / 项目归档、定位到具体消息
- **项目改动追踪**：监控指定工作区，记录文件改动与前后快照，并与会话日志中的文件操作对齐，还原 Agent 的实际工作轨迹
- **长会话压缩**：机械规则 + Jev 评估 + 可配置 LLM 策略，按完整对话轮次处理并管理生成的摘要
- **记忆与 Skill 管理**：浏览维护 Agent 记忆、项目指令与 Skill，查看其在各 Agent 目录下的安装与同步状态
- **能力复用**：桌面端、`contextos-mcp`、`contextos-cli` 共享同一套业务实现，Agent 可按需组合会话、改动、记忆、关系、压缩等操作
- **本机优先**：会话索引保存在本地，外部 LLM / 压缩服务仅在用户配置后按需调用

[![Repo](https://img.shields.io/badge/Repository-ContextOS-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/KeLe3377/ContextOS)

---



