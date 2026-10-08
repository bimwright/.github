<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="480">
</p>

<p align="center">
  English · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a>
</p>

# bimwright

Open-source tools connecting AI assistants to BIM and CAD applications.

Work with Revit, AutoCAD, Navisworks, and Inventor through the Model Context Protocol (MCP). Our C# gateways run locally and connect MCP-capable AI clients to the applications’ native APIs. Inspect models and drawings, automate repetitive tasks, and create or modify native geometry and documentation with human direction and review.

The name combines **BIM** with **wright**, an old word for a maker or builder—as in *shipwright*. We build tools for people who design and build.

---

## Tools

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) — MCP gateway for Autodesk® Revit®. Inspect BIM models, create and modify elements, and work with views, sheets, and model data. Typed tools and transaction-safe batches support agent-driven BIM workflows and add-in development. Apache-2.0.
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) — MCP gateway for Autodesk® AutoCAD®. Inspect and edit DWG drawings, work with geometry, text, blocks, dimensions, and annotations, and capture and navigate drawing views. Supports repetitive CAD work and in-place translation workflows. Apache-2.0.
- [**nwd-mcp**](https://github.com/bimwright/nwd-mcp) — MCP gateway for Autodesk® Navisworks® Manage. Query properties, search and select items, control visibility, and navigate saved viewpoints in federated models to support coordination and clash review. Apache-2.0.
- [**ipt-mcp**](https://github.com/bimwright/ipt-mcp) — MCP gateway for Autodesk® Inventor®. Build parametric parts, sketches, and features; place and inspect assemblies; and create and refine native engineering drawings with views, dimensions, annotations, and tables. Apache-2.0.
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) — Vietnamese-first BIM knowledge base covering ISO 19650, information management, project delivery, and Vietnam’s BIM regulatory landscape. CC-BY-SA 4.0.

The gateways provide typed tools for common tasks and C# execution for work beyond that surface. Optional ToolBaker workflows turn repeated patterns into reusable personal tools, with explicit acceptance rather than automatic self-learning. Each project README covers installation, supported application versions, capabilities, and safety limits.

## Naming

The gateway names take inspiration from familiar file extensions: `.rvt` for Revit models, `.dwg` for AutoCAD drawings, `.nwd` for Navisworks coordination models, and `.ipt` for Inventor parts. The `<ext>-mcp` pattern helps users recognize the application and workflows each gateway serves and keeps the family naming consistent. These are recognition cues, not limits on the file types or workflows a gateway supports.

The naming explains the projects' origins; it does not claim ownership of the file-format names or that those names are outside trademark protection. Related trademarks belong to their respective owners.

A shared architectural pattern runs through the whole `<ext>-mcp` family: predictable, auditable, reversible. If you're thinking of building one of these under a similar name, please reach out first — we'd rather collaborate than fragment.

---

<sub>Autodesk, AutoCAD, DWG, Inventor, Navisworks, and Revit are trademarks or registered trademarks of Autodesk, Inc., and/or its subsidiaries and/or affiliates. bimwright is an independent open-source project and is not affiliated with, sponsored by, or endorsed by Autodesk, Inc.</sub>
