# AegisAI-MCP Server

> 面向聊天通讯、信息安全、报告生成与代码检测场景的 LobeHub MCP 服务精选目录。

本项目整理 LobeHub MCP Plugins Marketplace 中与四类工作流高度相关、且在检索时点显示较高 **Installs** 数值的 MCP 服务。项目不复制第三方代码，仅保存服务元数据、用途摘要、配置提示、来源链接及风险审查意见，便于安全评估、选型和二次核验。

## 目录范围与口径

本次快照日期为 **2026-09-03（用户时区）**。下载量采用 LobeHub 详情页的 `Installs` 字段；该字段是市场安装计数，不等同于 GitHub Releases 下载量、活跃用户数或服务质量评分。候选服务通过 LobeHub 公开详情页和搜索结果交叉检索，按主题相关性与 Installs 排序，保留高相关服务；由于市场内容会持续变化，本目录不宣称是永久穷尽的全站排行榜。

| 主题 | 代表性高 Installs 候选 | 最高已核验 Installs |
|---|---|---:|
| 聊天通讯 | Teams MCP Server | 76 |
| 信息安全 | MCP Vulnerability Reporting | 8 |
| 报告生成 | Report Builder MCP Server | 6 |
| 代码检测 | Code Auditor | 157 |

## 快速索引

| 服务 | 主题 | Installs | 连接类型 | LobeHub | 上游仓库 |
|---|---|---:|---|---|---|
| Teams MCP Server | 聊天通讯 | 76 | local | [详情](https://lobehub.com/mcp/m0nkmaster-msteams-mcp) | [GitHub](https://github.com/m0nkmaster/msteams-mcp) |
| Code Auditor | 代码检测 / 安全模式 | 157 | local | [详情](https://lobehub.com/mcp/code-auditor-code-auditor) | [GitHub](https://github.com/BenAHammond/code-auditor-mcp) |
| Actionlint MCP 服务器 | 代码检测 | 47 | local | [详情](https://lobehub.com/mcp/hongkongkiwi-actionlint-mcp) | [GitHub](https://github.com/hongkongkiwi/actionlint-mcp) |
| Code Review MCP — Cursor-first PR reviewer | 代码检测 / 报告 | 46 | local | [详情](https://lobehub.com/mcp/shadabbi-code-review-mcp) | [GitHub](https://github.com/shadabbi/code-review-mcp) |
| Messages.app MCP Server | 聊天通讯 | 25 | local | [详情](https://lobehub.com/mcp/baphomet480-messages-app-mcp) | [GitHub](https://github.com/Baphomet480/messages-app-mcp) |
| Google Chat MCP | 聊天通讯 | 7 | hybrid | [详情](https://lobehub.com/mcp/nguyenvanduocit-google-chat-mcp) | [GitHub](https://github.com/nguyenvanduocit/google-chat-mcp) |
| MCP Vulnerability Reporting | 信息安全 / 报告 | 8 | local | [详情](https://lobehub.com/mcp/badchars-mcp-vulnerability-reporting) | [GitHub](https://github.com/badchars/mcp-vulnerability-reporting) |
| AutoPentest | 信息安全 | 7 | local | [详情](https://lobehub.com/mcp/bhavsec-autopentest-ai) | [GitHub](https://github.com/bhavsec/autopentest-ai) |
| Vulnerable MCP Server | 信息安全教育 | 6 | hybrid | [详情](https://lobehub.com/mcp/integsec-vulnerable-mcp-server) | [GitHub](https://github.com/integsec/VulnerableMCP) |
| Penetration Testing MCP Server | 信息安全 | 5 | local | [详情](https://lobehub.com/mcp/dr-yato-pentest-mcp-server) | [GitHub](https://github.com/Dr-yato/pentest-mcp-server) |
| Report Builder MCP Server | 报告生成 | 6 | remote | [详情](https://lobehub.com/mcp/nathanwolfe2208-mcp) | [GitHub](https://github.com/nathanwolfe2208/mcp) |
| whatsapp-mcp-server | 聊天通讯 | 2 | hybrid | [详情](https://lobehub.com/mcp/jochem-van-appeldoorn-whatsapp-mcp-server) | [GitHub](https://github.com/Jochem-van-Appeldoorn/whatsapp-mcp-server) |

## 选型结论

如果首要目标是代码质量与安全模式发现，**Code Auditor** 是本次核验候选中 Installs 最高的服务，适用于 TypeScript/JavaScript 代码库的 SOLID、DRY 和安全模式审查。若重点是 CI 工作流语法，Actionlint MCP 更聚焦；若重点是 GitHub PR 端到端审查、静态检查、测试和 Markdown 报告，Code Review MCP 的覆盖面更完整。

聊天通讯场景中，Teams MCP Server 的 LobeHub Installs 明显高于其他本次核验的通信类候选，但它需要 Microsoft Teams 账号和浏览器认证。Messages.app MCP Server 需要 macOS Messages 数据库的 Full Disk Access；Google Chat MCP 需要外部 OAuth 2.0 凭据；WhatsApp 服务涉及会话数据和消息内容，应优先采用隔离账户与最小权限策略。

报告生成方面，Report Builder MCP Server 提供邮件模板、HTML 报告、执行摘要、质量校验和品牌化能力。MCP Vulnerability Reporting 专注安全评估报告，但详情页提示其依赖本地绝对路径模板，因此部署前应检查模板路径并替换为项目内受控路径。

## 安全与合规提示

信息安全和通讯类 MCP 服务可能读取私密消息、凭据、源代码、漏洞数据或本地文件。部署前应审查源码、依赖、许可证、网络访问、日志和数据留存策略；生产环境建议使用专用账号、短期令牌、只读权限、容器隔离和出口控制。渗透测试类服务只能用于获得明确授权的资产，不能将本目录视为授权或安全保证。

第三方服务的安装命令、运行参数和权限要求应以其上游仓库当前文档为准。本项目不代替安全测试、代码审计、隐私影响评估或法律合规审查。

## 数据文件

`mcp-catalog.csv` 保存可筛选的结构化目录；`mcp-catalog.json` 保存相同记录及审查字段，便于后续自动更新；`methodology.md` 说明采集口径、限制与更新建议。

## References

[1]: https://lobehub.com/mcp/m0nkmaster-msteams-mcp "Teams MCP Server — LobeHub"
[2]: https://lobehub.com/mcp/code-auditor-code-auditor "Code Auditor — LobeHub"
[3]: https://lobehub.com/mcp/hongkongkiwi-actionlint-mcp "Actionlint MCP — LobeHub"
[4]: https://lobehub.com/mcp/shadabbi-code-review-mcp "Code Review MCP — LobeHub"
[5]: https://lobehub.com/mcp/baphomet480-messages-app-mcp "Messages.app MCP Server — LobeHub"
[6]: https://lobehub.com/mcp/nguyenvanduocit-google-chat-mcp "Google Chat MCP — LobeHub"
[7]: https://lobehub.com/mcp/badchars-mcp-vulnerability-reporting "MCP Vulnerability Reporting — LobeHub"
[8]: https://lobehub.com/mcp/bhavsec-autopentest-ai "AutoPentest — LobeHub"
[9]: https://lobehub.com/mcp/integsec-vulnerable-mcp-server "Vulnerable MCP Server — LobeHub"
[10]: https://lobehub.com/mcp/dr-yato-pentest-mcp-server "Penetration Testing MCP Server — LobeHub"
[11]: https://lobehub.com/mcp/nathanwolfe2208-mcp "Report Builder MCP Server — LobeHub"
[12]: https://lobehub.com/mcp/jochem-van-appeldoorn-whatsapp-mcp-server "whatsapp-mcp-server — LobeHub"

---

作者：**Manus AI**  
项目名称：**AegisAI-MCP Server**
