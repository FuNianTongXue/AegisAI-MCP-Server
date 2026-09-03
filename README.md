# AegisAI-MCP Server

> 面向聊天通讯、信息安全、报告生成与代码检测场景的 MCP 服务精选目录。

本项目整理与四类工作流高度相关的 MCP 服务，保存服务名称、版本、连接类型、用途摘要、上游仓库链接以及安全审查提示，便于技术选型、部署评估和二次核验。项目不复制第三方代码。

## 目录范围

本目录覆盖聊天通讯、信息安全、报告生成和代码检测四类场景。服务按照场景相关性与功能覆盖范围组织，不代表任何服务质量认证、商业推荐或安全保证。

| 主题 | 代表性服务 | 适用重点 |
|---|---|---|
| 聊天通讯 | Teams MCP Server、Messages.app MCP Server、Google Chat MCP、whatsapp-mcp-server | 企业协作、消息检索、会话管理和消息发送 |
| 信息安全 | AutoPentest、Vulnerable MCP Server、Penetration Testing MCP Server | 授权安全测试、实验环境和漏洞评估 |
| 报告生成 | Report Builder MCP Server、MCP Vulnerability Reporting | 执行摘要、HTML 报告和安全评估报告 |
| 代码检测 | Code Auditor、Actionlint MCP、Code Review MCP | 代码质量、CI 工作流、PR 审查和安全检测 |

## 服务索引

| 服务 | 主题 | 版本 | 连接类型 | 上游仓库 |
|---|---|---:|---|---|
| Teams MCP Server | 聊天通讯 | 0.23.1 | local | [GitHub](https://github.com/m0nkmaster/msteams-mcp) |
| Messages.app MCP Server | 聊天通讯 | 2.0.1 | local | [GitHub](https://github.com/Baphomet480/messages-app-mcp) |
| Google Chat MCP | 聊天通讯 | 1.0.0 | hybrid | [GitHub](https://github.com/nguyenvanduocit/google-chat-mcp) |
| whatsapp-mcp-server | 聊天通讯 | 1.0.0 | hybrid | [GitHub](https://github.com/Jochem-van-Appeldoorn/whatsapp-mcp-server) |
| AutoPentest | 信息安全 | 1.0.0 | local | [GitHub](https://github.com/bhavsec/autopentest-ai) |
| Vulnerable MCP Server | 信息安全教育 | 1.0.0 | hybrid | [GitHub](https://github.com/integsec/VulnerableMCP) |
| Penetration Testing MCP Server | 信息安全 | 2.0.0 | local | [GitHub](https://github.com/Dr-yato/pentest-mcp-server) |
| Report Builder MCP Server | 报告生成 | 1.0.0 | remote | [GitHub](https://github.com/nathanwolfe2208/mcp) |
| MCP Vulnerability Reporting | 信息安全 / 报告生成 | 0.1.0 | local | [GitHub](https://github.com/badchars/mcp-vulnerability-reporting) |
| Code Auditor | 代码检测 | 1.0.0 | local | [GitHub](https://github.com/BenAHammond/code-auditor-mcp) |
| Actionlint MCP 服务器 | 代码检测 | 1.0.0 | local | [GitHub](https://github.com/hongkongkiwi/actionlint-mcp) |
| Code Review MCP — Cursor-first PR reviewer | 代码检测 / 报告生成 | 1.0.0 | local | [GitHub](https://github.com/shadabbi/code-review-mcp) |

## 选型建议

如果重点是 TypeScript/JavaScript 代码质量、安全模式和架构问题，Code Auditor 更加聚焦；如果重点是 GitHub Actions 工作流语法以及 Shell 或 Python 检查，Actionlint MCP 更合适；如果需要将 PR 差异、静态检查、测试和 Markdown 报告串联起来，可进一步评估 Code Review MCP。

聊天通讯场景应根据平台约束选择服务。Teams MCP Server 面向 Teams 会话、频道和会议内容；Messages.app MCP Server 面向 macOS Messages；Google Chat MCP 需要 Google OAuth 认证；WhatsApp 服务涉及会话数据和消息内容。部署这些服务时，应优先使用专用账号、最小权限和隔离存储。

报告生成场景中，Report Builder MCP Server 支持邮件模板、HTML 报告、执行摘要、质量校验和品牌化能力。MCP Vulnerability Reporting 专注安全评估报告，但部署前需要检查模板路径、模板内容和报告留存策略。

## 安全与合规提示

信息安全和通讯类 MCP 服务可能读取私密消息、凭据、源代码、漏洞数据或本地文件。部署前应审查源码、依赖、许可证、网络访问、日志和数据留存策略；生产环境建议使用专用账号、短期令牌、只读权限、容器隔离和出口控制。渗透测试类服务只能用于获得明确授权的资产；故意包含漏洞的服务只能在隔离实验环境中运行。

第三方服务的安装命令、运行参数和权限要求应以其上游仓库当前文档为准。本项目不代替安全测试、代码审计、隐私影响评估或法律合规审查。

## 数据文件

`mcp-catalog.csv` 保存可筛选的结构化目录；`mcp-catalog.json` 保存相同记录及审查字段；`methodology.md` 说明收录范围、核验方法、风险审查原则和更新建议。

---

作者：**Manus AI**  
项目名称：**AegisAI-MCP Server**
