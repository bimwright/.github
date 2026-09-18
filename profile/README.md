<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="480">
</p>

<p align="center">
  English · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a>
</p>

# bimwright

Open-source tools connecting AI assistants to BIM and CAD applications.

Work with Revit, AutoCAD, Navisworks, and Inventor through the Model Context Protocol (MCP). Query models, automate repetitive tasks, and make changes using the applications’ native APIs.

The name combines **BIM** with **wright**, an old word for a maker or builder—as in *shipwright*. We build tools for people who design and build.

---

## Tools

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) — MCP gateway for Autodesk® Revit® 2022–2027. 229 tools across 23 toolsets (232 with adaptive bake), with progressive disclosure (toolset gating), transaction-safe batch execution, and a ToolBaker self-evolution engine. Apache-2.0.
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) — MCP gateway for Autodesk® AutoCAD® 2022–2027. 61 tools (36 default + 25 optional) with a ToolBaker self-evolution engine. Read drawing text, cluster spatial fragments, rewrite translations in place, and run audited code through one reversible workflow. Apache-2.0.
- [**nwd-mcp**](https://github.com/bimwright/nwd-mcp) — MCP gateway for Autodesk® Navisworks® Manage 2022–2027. 30 tools when all toolsets and send_code enabled (default 29) with a ToolBaker self-evolution engine. Query, inspect, and navigate federated coordination models for clash review, secured with loopback-only TCP and per-session tokens. Apache-2.0.
- [**ipt-mcp**](https://github.com/bimwright/ipt-mcp) — MCP gateway for Autodesk® Inventor® 2022–2027. 59 tools with send_code (default 58) across 13 toolsets, with a ToolBaker self-evolution engine. Drive parametric part/sketch/feature modeling, parameters, and iProperties as AI-callable tools across a pure-C# multi-version add-in stack. Apache-2.0.
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) — Vietnamese-first BIM knowledge base: ISO 19650 + the Vietnamese regulatory landscape (QĐ 347/348/1057/2500, Luật 60/2024, Nghị định 111/2024/175/2024, Circulars 09/2024/24/2025). CC-BY-SA 4.0.

A shared architectural pattern runs through the whole `<ext>-mcp` family: predictable, auditable, reversible. If you're thinking of building one of these under a similar name, please reach out first — we'd rather collaborate than fragment.

---

<sub>Revit, AutoCAD, Navisworks, Inventor, and Autodesk are registered trademarks of Autodesk, Inc. bimwright is an independent open-source project and is not affiliated with, sponsored by, or endorsed by Autodesk, Inc.</sub>
