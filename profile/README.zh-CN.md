<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright — The Digital Craft of the Built Environment" width="480">
</p>

<p align="center">
  <a href="README.md">📖 English</a> · <a href="README.vi.md">Tiếng Việt</a> · 简体中文
</p>

# bimwright — 建成环境的数字匠艺

几个世纪以前，"wright" 指的是一位技艺精湛的匠人 —— 与自己所用的材料有着深入、亲手经验的艺人。今天，建筑行业的"材料"是数据和代码。然而，现代 AEC (建筑/工程/施工) 从业者却常常被困在"围墙花园"之中 —— 被迫使用臃肿、黑箱式的软件，遮蔽了这一学科真正的技艺。

bimwright 的使命是找回匠人的精神。我们不只是软件供应商 —— 我们是逻辑的匠人。通过亲手打造开放、精确的 MCP (Model Context Protocol) 服务器，我们构建起关键的桥梁，让重型 AEC 应用能够与现代 AI 一起进行推理与操作。

我们相信"对"的 BIM 应该是这样做的 —— 透明、专注、为真正的从业者而刻意设计。把控制权交还到实际设计这个世界的建筑师与工程师手中。

**bimwright. Built right.**

---

## Tools

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) —— 面向 Autodesk® Revit® 2022–2027 的 MCP gateway。把 Revit API 暴露成 AI 可调用的工具，配套 progressive disclosure (toolset gating)、事务安全的 batch execution，以及 ToolBaker 自进化引擎。
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) —— 面向 Autodesk® AutoCAD® 2024 的 MCP gateway。读取图纸文字、按空间关系聚合片段、原位写回翻译，并通过可审计、可撤销的流程执行代码。
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) —— 越南语优先的 BIM 知识库：ISO 19650 + 越南本地监管体系 (QĐ 347/348/1057/2500、Luật 60/2024、Nghị định 111/2024/175/2024)。CC-BY-SA 4.0 许可证。页面内容以越南语为主。

### On the forge (锻造中)

`<ext>-mcp` 家族的后续规划：

- **`nwd-mcp`** —— 面向 Navisworks® 的 MCP gateway (NWD 协调 / 冲突检查)。

与 `rvt-mcp` 和 `dwg-mcp` 共享同一套架构原则：predictable, auditable, reversible (可预测、可审计、可回滚)。如果您正在考虑以相近命名自行开发其中之一，请先与我们联系 —— 我们更希望协作，而不是让生态碎片化。

---

<sub>Revit、AutoCAD、Navisworks 与 Autodesk 是 Autodesk, Inc. 的注册商标。bimwright 是一个独立的开源项目，与 Autodesk, Inc. 无任何附属、赞助或背书关系。</sub>
