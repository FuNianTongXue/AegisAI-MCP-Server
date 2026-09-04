# AegisAI-MCP Server

> 面向聊天通讯、信息安全、报告生成、代码检测、移动端模拟器、威胁情报、逆向工程、合规检测、Android 安全与 iOS 安全场景的 MCP 服务精选目录。

本项目整理与多类工作流高度相关的 MCP 服务，保存服务名称、版本或版本要求、连接类型、用途摘要、上游仓库链接以及安全审查提示，便于技术选型、部署评估和二次核验。项目不复制第三方代码。

## 目录范围

本目录覆盖十一类场景。服务按照场景相关性与功能覆盖范围组织，不代表任何服务质量认证、商业推荐或安全保证。

| 主题 | 代表性服务 | 适用重点 |
|---|---|---|
| 聊天通讯 | Teams MCP Server、Messages.app MCP Server、Google Chat MCP、whatsapp-mcp-server | 企业协作、消息检索、会话管理和消息发送 |
| 信息安全 | AutoPentest、Vulnerable MCP Server、Penetration Testing MCP Server | 授权安全测试、实验环境和漏洞评估 |
| 报告生成 | Report Builder MCP Server、MCP Vulnerability Reporting | 执行摘要、HTML 报告和安全评估报告 |
| 代码检测 | Code Auditor、Actionlint MCP、Code Review MCP | 代码质量、CI 工作流、PR 审查和安全检测 |
| iOS 模拟器 | iOS Simulator MCP Server、Mobile MCP | UI 自动化、截图、录屏、应用安装和调试 |
| Android 模拟器 | Mobile MCP、Android-MCP、Android MCP Server | ADB 自动化、应用操作、截图、录屏和崩溃信息 |
| 威胁情报 | Google Threat Intelligence MCP、OpenCTI MCP Server、FastMCP Threat Intelligence | IOC、恶意软件、域名、IP、威胁组织和报告查询 |
| 逆向工程 | Ghidra MCP Server、ReVa、APKTool MCP Server | 二进制分析、反编译、静态分析、数据流和固件分析 |
| 合规检测 | MCP Server Audit、MCP Security Scanner | MCP 服务审计、依赖检查、IaC 检查和合规违规识别 |
| Android 安全 | MobSF-MCP、APKTool MCP Server | APK/Android 安全扫描、权限、Manifest、代码和组件分析 |
| iOS 安全 | MobSF-MCP、Mobile Security MCP | IPA/iOS 安全扫描、隐私、代码、证书和配置分析 |

## 服务索引

| 服务 | 主题 | 版本或要求 | 连接类型 | 上游仓库 |
|---|---|---|---|---|
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
| iOS Simulator MCP Server | iOS 模拟器 | >=1.3.3 | local | [GitHub](https://github.com/joshuayoes/ios-simulator-mcp) |
| Mobile MCP | iOS / Android 模拟器 | latest | local | [GitHub](https://github.com/mobile-next/mobile-mcp) |
| Android-MCP | Android 模拟器 | latest | local | [GitHub](https://github.com/CursorTouch/Android-MCP) |
| Android MCP Server | Android 模拟器 | latest | local | [GitHub](https://github.com/martingeidobler/android-mcp-server) |
| Google Threat Intelligence MCP | 威胁情报 | latest | local | [GitHub](https://github.com/google/mcp-security) |
| OpenCTI MCP Server | 威胁情报 | latest | local | [GitHub](https://github.com/zxzinn/opencti-mcp) |
| FastMCP Threat Intelligence | 威胁情报 | latest | local | [GitHub](https://github.com/4R9UN/fastmcp-threatintel) |
| Ghidra MCP Server | 逆向工程 | latest | local | [GitHub](https://github.com/bethington/ghidra-mcp) |
| ReVa — Reverse Engineering Assistant | 逆向工程 | 7.3.1 | local | [GitHub](https://github.com/cyberkaida/reverse-engineering-assistant) |
| APKTool MCP Server | 逆向工程 / Android 安全 | 3.0.0 | local | [GitHub](https://github.com/zinja-coder/apktool-mcp-server) |
| MCP Server Audit | 合规检测 / MCP 安全 | latest | local | [GitHub](https://github.com/ModelContextProtocol-Security/mcpserver-audit) |
| MCP Security Scanner | 合规检测 / 代码安全 | latest | local | [GitHub](https://github.com/aws-samples/sample-mcp-security-scanner) |
| MobSF-MCP | Android 安全 / iOS 安全 | latest | local | [GitHub](https://github.com/nkcc-apk/MobSF-MCP) |
| Mobile Security MCP | Android 安全 / iOS 安全 | latest | local | [GitHub](https://github.com/Serhatcck/mobile-security-mcp) |

## 选型建议

如果重点是 TypeScript/JavaScript 代码质量、安全模式和架构问题，Code Auditor 更加聚焦；如果重点是 GitHub Actions 工作流语法以及 Shell 或 Python 检查，Actionlint MCP 更合适；如果需要将 PR 差异、静态检查、测试和 Markdown 报告串联起来，可进一步评估 Code Review MCP。

移动端自动化方面，iOS Simulator MCP Server 适合直接控制 iOS Simulator 的可访问性树、点击、输入、截图、录屏、应用安装和深链接；Mobile MCP 通过统一接口覆盖 iOS Simulator、Android Emulator 以及真实设备；Android-MCP 和 Android MCP Server 更适合基于 ADB 的 Android 操作。移动自动化服务应使用专用模拟器或测试设备，不要把生产账户、支付信息或个人消息导入测试环境。

逆向工程方面，Ghidra MCP Server 适合较完整的二进制分析、反编译、P-code、调试和批处理工作流；ReVa 适合以 Ghidra 为基础的长流程辅助分析；APKTool MCP Server 更适合 Android APK 的 Manifest、资源、smali 和权限分析。逆向分析必须针对自有、获授权或明确允许研究的样本，并在隔离环境中执行脚本和样本。

合规检测方面，MCP Server Audit 面向 MCP 服务源代码、配置和依赖的安全审计，可辅助识别危险模式、依赖风险和配置问题；MCP Security Scanner 将 Checkov、Semgrep、Bandit 和 ASH 等扫描能力统一到 MCP 工作流中，适合代码、IaC 和安全基线检查。扫描结果需要由具备经验的人员复核，不能直接等同于合规认证或法律结论。

Android 安全和 iOS 安全方面，MobSF-MCP 将 MobSF 的 APK、IPA 和 APPX 分析能力通过 MCP 暴露，可查询权限、组件、证书、网络安全、代码、隐私和报告信息；Mobile Security MCP 可作为移动应用静态分析和安全评估候选。应使用测试样本和隔离的 MobSF 实例，保护上传文件、API 密钥、源码和生成的报告。

威胁情报方面，Google Threat Intelligence MCP 连接 VirusTotal API，可查询威胁集合、恶意软件、文件、域名、IP、URL 和 IOC；OpenCTI MCP Server 面向 OpenCTI 平台，可查询报告、恶意软件、指标、威胁组织以及 STIX 对象。所有服务都应通过环境变量或密钥管理器保存 API 凭据，不得将令牌写入仓库；对外部 IOC、报告和样本应进行数据分级与访问控制。

## 安全与合规提示

信息安全、威胁情报、逆向分析、移动安全和通讯类 MCP 服务可能读取私密消息、凭据、源代码、漏洞数据、恶意样本、应用包或本地文件。部署前应审查源码、依赖、许可证、网络访问、日志和数据留存策略；生产环境建议使用专用账号、短期令牌、只读权限、容器隔离和出口控制。

移动模拟器和移动安全 MCP 可能执行点击、输入、应用安装、深链接打开、录屏、设备控制、APK/IPA 上传和报告导出。应限制设备范围和可访问数据，关闭不必要的外网访问，并避免把真实个人设备、生产证书或敏感凭据暴露给自动化代理。

逆向工程、渗透测试和样本分析类服务只能用于获得明确授权的目标或样本；故意包含漏洞的服务只能在隔离实验环境中运行。合规检测工具的输出不构成认证、审计意见或法律意见。

第三方服务的安装命令、运行参数和权限要求应以其上游仓库当前文档为准。本项目不代替安全测试、代码审计、威胁情报研判、移动应用安全评估、隐私影响评估或法律合规审查。

## 数据文件

`mcp-catalog.csv` 保存可筛选的结构化目录；`mcp-catalog.json` 保存相同记录及审查字段；`methodology.md` 说明收录范围、核验方法、风险审查原则和更新建议。

---

项目名称：**AegisAI-MCP Server**
