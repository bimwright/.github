<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="480">
</p>

<p align="center">
  <a href="README.md">English</a> · <a href="README.vi.md">Tiếng Việt</a> · 简体中文 · <a href="README.ja.md">日本語</a>
</p>

# bimwright

连接 AI 助手与 BIM、CAD 应用的开源工具。

通过 Model Context Protocol（MCP）使用 Revit、AutoCAD、Navisworks 和 Inventor。我们的 C# 网关在本地运行，将支持 MCP 的 AI 客户端连接到应用的原生 API。在人的指导和审核下，检查模型与图纸、自动化重复任务，并创建或修改原生几何与技术文档。

**bimwright** 这个名字由 **BIM** 和 **wright** 组成。wright 是英语中表示制作者或建造者的旧词，如 *shipwright*（造船工）。我们为从事设计和建造的人开发工具。

---

## 工具

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) —— 面向 Autodesk® Revit® 的 MCP 网关。检查 BIM 模型，创建和修改构件，并处理视图、图纸与模型数据。类型明确的工具和事务安全的批量执行支持智能体驱动的 BIM 工作流程与插件开发。Apache-2.0。
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) —— 面向 Autodesk® AutoCAD® 的 MCP 网关。检查和编辑 DWG 图纸，处理几何、文字、块、尺寸和注释，并捕获与导航图纸视图。支持重复性 CAD 工作和原位文字翻译流程。Apache-2.0。
- [**nwd-mcp**](https://github.com/bimwright/nwd-mcp) —— 面向 Autodesk® Navisworks® Manage 的 MCP 网关。在联合模型中查询属性、搜索和选择对象、控制可见性并导航已保存的视点，辅助协调与冲突审查。Apache-2.0。
- [**ipt-mcp**](https://github.com/bimwright/ipt-mcp) —— 面向 Autodesk® Inventor® 的 MCP 网关。构建参数化零件、草图与特征，放置和检查装配，并创建和完善包含视图、尺寸、注释和表格的原生工程图。Apache-2.0。
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) —— 越南语优先的 BIM 知识库，涵盖 ISO 19650、信息管理、项目交付和越南的 BIM 法规体系。CC-BY-SA 4.0。

网关为常见任务提供类型明确的工具，并通过 C# 执行处理工具范围之外的工作。可选的 ToolBaker 流程将重复模式转为可复用的个人工具，需要明确接受，而非自动自学习。各项目的 README 提供安装方法、支持的应用版本、功能和安全限制。

## 命名方式

这些网关的名称源自用户熟悉的文件扩展名：Revit 模型的 `.rvt`、AutoCAD 图纸的 `.dwg`、Navisworks 协调模型的 `.nwd`，以及 Inventor 零件的 `.ipt`。统一的 `<ext>-mcp` 命名方式便于用户识别各网关面向的应用和工作流程。这些名称是识别线索，并不限定网关支持的文件类型或工作流程。

这段说明解释名称的由来，并不主张我们拥有文件格式名称，也不表示这些名称不受商标保护。相关商标归各自权利人所有。

整个 `<ext>-mcp` 家族共享同一套架构原则：predictable, auditable, reversible (可预测、可审计、可回滚)。如果您正在考虑以相近命名自行开发其中之一，请先与我们联系 —— 我们更希望协作，而不是让生态碎片化。

---

<sub>Autodesk、AutoCAD、DWG、Inventor、Navisworks 和 Revit 是 Autodesk, Inc. 及／或其子公司、关联公司的商标或注册商标。bimwright 是一个独立的开源项目，与 Autodesk, Inc. 无任何附属、赞助或背书关系。</sub>
