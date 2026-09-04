# 新增方向核验记录（2026-09-04）

## 逆向工程

- Ghidra MCP Server: https://github.com/bethington/ghidra-mcp 。公开仓库说明其提供 Ghidra 二进制分析、反编译、P-code、调试、批处理和项目管理能力；仓库页面显示 Apache-2.0 许可证。
- ReVa: https://github.com/cyberkaida/reverse-engineering-assistant 。公开仓库说明其为 Ghidra MCP server，可用于长流程二进制和固件逆向分析；仓库页面显示版本 7.3.1 发布信息。
- APKTool MCP Server: https://github.com/zinja-coder/apktool-mcp-server 。公开仓库说明其基于 apktool 分析 Android APK，支持 Manifest、权限、导出组件、smali 和硬编码 URL/IP 检查；仓库页面显示 Apache-2.0 许可证。

## 合规检测

- MCP Server Audit: https://github.com/ModelContextProtocol-Security/mcpserver-audit 。公开仓库说明其审计 MCP server 源码，检查漏洞、依赖、配置和危险模式，并提供 CWE/AIVSS 相关分析。
- MCP Security Scanner: https://github.com/aws-samples/sample-mcp-security-scanner 。公开仓库说明其通过 MCP 统一调用 Checkov、Semgrep、Bandit 和 ASH，覆盖代码、IaC、安全漏洞和合规规则检查。

## Android 安全与 iOS 安全

- MobSF-MCP: https://github.com/nkcc-apk/MobSF-MCP 。公开仓库说明其将 MobSF API 通过 MCP 暴露，支持 APK、IPA、APPX 上传、扫描日志、JSON/PDF 报告、权限、组件、证书、网络安全、代码、隐私、SBOM 和 VirusTotal 结果查询。
- Mobile Security MCP: https://github.com/Serhatcck/mobile-security-mcp 。公开检索结果将其描述为可分析 Android APK 和 iOS 应用包的移动应用安全 MCP 服务；部署前需复核仓库当前文档。

## 记录口径

项目只保留上游仓库链接，不保留任何第三方市场名称、市场安装量或市场来源字段。版本为上游公开说明中的版本、最低安全版本或 latest 占位；功能摘要为公开说明的归纳，不等同于完整安全验证。逆向、移动安全和合规扫描均需在授权和隔离环境中运行。
