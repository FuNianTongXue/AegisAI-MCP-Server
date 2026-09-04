# AegisAI-MCP Server

> 面向聊天通讯、信息安全、报告生成、代码检测、移动端模拟器、威胁情报、逆向工程、合规检测、Android 安全与 iOS 安全场景的 MCP 服务精选目录。

本项目整理与多类工作流高度相关的 MCP 服务，保存服务名称、版本或版本要求、连接类型、用途摘要、上游仓库链接以及安全审查提示，便于技术选型、部署评估和二次核验。项目不复制第三方代码。

> **重要安全提示：本目录中的 MCP 服务可能由境外个人、组织或云平台维护，服务代码、依赖、镜像、API 端点和数据存储位置可能不在中国境内，实际所在地和数据处理范围必须由使用方自行核验。任何服务都不应因出现在本目录中而被直接安装、下载或接入生产环境。请先完成来源审查、许可证核验、恶意代码与依赖扫描、数据出境评估、权限审查和隔离验证，再决定是否使用。**

建议将 MCP 服务视为需要纳管的软件供应链组件，而不是普通插件。安装包、容器镜像、npm/PyPI 依赖、启动脚本、配置文件和远程 API 均应纳入物料清单（SBOM）和变更管理；服务接入应经过门闸审批、签名或哈希校验、漏洞扫描、权限校验、网络策略校验和运行时监控。

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

## 安全治理建议

### 1. MCP 物料清单（SBOM）管理

每个拟安装的 MCP 服务都应建立唯一资产记录，至少记录服务名称、上游仓库、版本或提交哈希、包管理器、依赖版本、容器镜像摘要、许可证、维护者、下载时间、来源区域、数据处理区域、所需凭据、网络端点、工具权限、风险等级、审批人和最近复核时间。生产环境应固定版本和哈希，禁止直接使用未经审查的 `latest`、浮动分支或未锁定依赖。

建议将 `data/mcp-sbom-template.csv` 作为登记模板，将源码、依赖锁文件、容器镜像、配置和扫描报告关联到同一资产编号。SBOM 不是一次性文件，应在版本升级、依赖变化、镜像变化、API 端点变化或权限变化时重新生成并复核。

### 2. 服务接入门闸

MCP 服务接入前应经过分层门闸。第一层核验来源、维护状态、许可证、版本签名或哈希、依赖和已知漏洞；第二层核验工具清单、命令执行能力、文件读写范围、网络访问、OAuth/API 权限和数据留存；第三层在隔离环境中进行功能、越权、提示注入、敏感数据外传和异常行为测试；第四层由业务、安全和数据合规责任人审批后，才允许进入受控生产网络。

接入网关或代理应默认拒绝未知服务和未知工具，采用服务白名单、工具级白名单、最小权限、短期凭据、出站域名白名单、请求大小限制、超时、速率限制、审计日志和人工确认。对具有发送消息、发布评论、执行命令、安装应用、上传文件、导出报告或访问敏感数据能力的工具，应默认关闭自动批准。

### 3. 高风险服务使用临时安全沙箱

对于逆向工程、APK/IPA 分析、恶意样本处理、渗透测试、命令执行、不可信代码扫描、依赖构建和可能执行第三方脚本的 MCP 服务，建议优先使用 E2B 等临时安全沙箱或组织批准的等效隔离环境。E2B 官方文档将 Sandbox 描述为按需创建的隔离 Linux 虚拟机，并支持设置超时和主动销毁；但沙箱不等于自动安全，使用方仍需自行配置网络、凭据、数据和权限边界。[1] [2]

沙箱应采用短生命周期、一次性或可复现模板、最小权限、无生产凭据、出站网络白名单、只读输入挂载、受控输出目录、CPU/内存/进程/磁盘配额和完整执行审计。任务完成后应主动销毁沙箱，不应默认暂停并长期保留含有源码、样本、密钥或报告的文件状态。对需要访问真实设备、iOS/Android 模拟器或内网系统的服务，应将设备控制面与样本执行面分离，禁止让不可信样本直接接触生产网络。

### 4. 境外服务和数据处理审查

对于代码、源代码仓库、聊天消息、漏洞报告、APK/IPA、恶意样本、威胁情报和个人信息，使用方应确认数据是否会传输到境外或第三方云平台，核验服务商的隐私政策、数据留存、训练使用、分包商、跨境传输机制和删除能力。无法确认数据处理位置、权限边界或删除机制时，不应上传敏感数据；可优先选择自托管、内网部署、脱敏数据和隔离测试账号。

更完整的登记字段、门闸流程、沙箱要求和拒绝条件见 [`docs/security-governance.md`](docs/security-governance.md) 与 [`data/mcp-sbom-template.csv`](data/mcp-sbom-template.csv)。

## 安全与合规提示

信息安全、威胁情报、逆向分析、移动安全和通讯类 MCP 服务可能读取私密消息、凭据、源代码、漏洞数据、恶意样本、应用包或本地文件。部署前应审查源码、依赖、许可证、网络访问、日志和数据留存策略；生产环境建议使用专用账号、短期令牌、只读权限、容器隔离和出口控制。

移动模拟器和移动安全 MCP 可能执行点击、输入、应用安装、深链接打开、录屏、设备控制、APK/IPA 上传和报告导出。应限制设备范围和可访问数据，关闭不必要的外网访问，并避免把真实个人设备、生产证书或敏感凭据暴露给自动化代理。

逆向工程、渗透测试和样本分析类服务只能用于获得明确授权的目标或样本；故意包含漏洞的服务只能在隔离实验环境中运行。合规检测工具的输出不构成认证、审计意见或法律意见。

第三方服务的安装命令、运行参数和权限要求应以其上游仓库当前文档为准。本项目不代替安全测试、代码审计、威胁情报研判、移动应用安全评估、隐私影响评估或法律合规审查。

## 数据文件

`mcp-catalog.csv` 保存可筛选的结构化目录；`mcp-catalog.json` 保存相同记录及审查字段；`methodology.md` 说明收录范围、核验方法、风险审查原则和更新建议；`data/mcp-sbom-template.csv` 提供 MCP 软件物料清单登记模板；`docs/security-governance.md` 提供服务接入门闸、风险分级和校验建议。

---

项目名称：**AegisAI-MCP Server**

## References

[1]: https://e2b.dev/docs "E2B Documentation"
[2]: https://e2b.dev/docs/sandbox "E2B Sandbox Lifecycle"
