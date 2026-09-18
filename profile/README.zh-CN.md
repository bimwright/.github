<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="480">
</p>

<p align="center">
  <a href="README.md">English</a> · <a href="README.vi.md">Tiếng Việt</a> · 简体中文 · <a href="README.ja.md">日本語</a>
</p>

# bimwright

连接 AI 助手与 BIM、CAD 应用的开源工具。

通过 Model Context Protocol（MCP）使用 Revit、AutoCAD、Navisworks 和 Inventor。借助这些应用的原生 API 查询模型、自动化重复任务并执行修改。

**bimwright** 这个名字由 **BIM** 和 **wright** 组成。wright 是英语中表示制作者或建造者的旧词，如 *shipwright*（造船工）。我们为从事设计和建造的人开发工具。

---

## Tools

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) —— 面向 Autodesk® Revit® 2022–2027 的 MCP gateway。把 Revit API 暴露成 AI 可调用的工具，配套 progressive disclosure (toolset gating)、事务安全的 batch execution，以及 ToolBaker 自进化引擎。
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) —— 面向 Autodesk® AutoCAD® 2022–2027 的 MCP gateway。读取图纸文字、按空间关系聚合片段、原位写回翻译，并通过可审计、可撤销的流程执行代码。
- [**nwd-mcp**](https://github.com/bimwright/nwd-mcp) —— 面向 Autodesk® Navisworks® Manage 2022–2027 的 MCP gateway。查询、检视并导航联合 (federated) 协调模型以进行冲突检查，采用仅环回 (loopback-only) TCP 与按会话令牌保障安全。
- [**ipt-mcp**](https://github.com/bimwright/ipt-mcp) —— 面向 Autodesk® Inventor® 2022–2027 的 MCP gateway。把参数化的 part/sketch/feature 建模、参数与 iProperty 暴露成 AI 可调用的工具，运行于纯 C# 的多版本 add-in 技术栈之上。
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) —— 越南语优先的 BIM 知识库：ISO 19650 + 越南本地监管体系 (QĐ 347/348/1057/2500、Luật 60/2024、Nghị định 111/2024/175/2024、Thông tư 09/2024/24/2025)。CC-BY-SA 4.0 许可证。页面内容以越南语为主。

整个 `<ext>-mcp` 家族共享同一套架构原则：predictable, auditable, reversible (可预测、可审计、可回滚)。如果您正在考虑以相近命名自行开发其中之一，请先与我们联系 —— 我们更希望协作，而不是让生态碎片化。

---

<sub>Revit、AutoCAD、Navisworks、Inventor 与 Autodesk 是 Autodesk, Inc. 的注册商标。bimwright 是一个独立的开源项目，与 Autodesk, Inc. 无任何附属、赞助或背书关系。</sub>
