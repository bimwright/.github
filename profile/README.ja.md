<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="480">
</p>

<p align="center">
  <a href="README.md">English</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.zh-CN.md">简体中文</a> · 日本語
</p>

# bimwright

AI アシスタントと BIM・CAD アプリケーションをつなぐオープンソースのツール。

Model Context Protocol（MCP）を通じて Revit、AutoCAD、Navisworks、Inventor を操作できます。各アプリケーションのネイティブ API を使い、モデルの照会、繰り返し作業の自動化、変更の実行を行います。

**bimwright** は **BIM** と **wright** を組み合わせた名前です。wright は、ものを作る人や建てる人を表す古い英語で、*shipwright*（船大工）などに使われます。私たちは、設計や建設に携わる人のためのツールを開発しています。

---

## ツール

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) — Autodesk® Revit® 2022–2027 向けの MCP ゲートウェイ。Revit API を AI から呼び出せるツールとして公開し、ツールセットによる段階的な公開、トランザクションを保護するバッチ実行、ToolBaker によるツールの再利用に対応します。Apache-2.0。
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) — Autodesk® AutoCAD® 2022–2027 向けの MCP ゲートウェイ。図面の文字を読み取り、位置関係に応じて断片をまとめ、翻訳を元の位置に書き戻します。コード実行の監査と操作の取り消しにも対応します。Apache-2.0。
- [**nwd-mcp**](https://github.com/bimwright/nwd-mcp) — Autodesk® Navisworks® Manage 2022–2027 向けの MCP ゲートウェイ。干渉確認のために統合モデルを照会・確認し、ビューを移動できます。通信はループバック TCP に限定し、セッションごとのトークンで認証します。Apache-2.0。
- [**ipt-mcp**](https://github.com/bimwright/ipt-mcp) — Autodesk® Inventor® 2022–2027 向けの MCP ゲートウェイ。パラメトリックなパーツ・スケッチ・フィーチャのモデリング、パラメータ、iProperty を AI から操作できます。複数バージョンに対応するアドインを C# で実装しています。Apache-2.0。
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) — ベトナム語を中心とする BIM ナレッジベース。ISO 19650 とベトナムの法規制（QĐ 347/348/1057/2500、Luật 60/2024、Nghị định 111/2024/175/2024、Thông tư 09/2024/24/2025）を扱います。CC-BY-SA 4.0。

`<ext>-mcp` ファミリーは、予測可能で、監査でき、操作を取り消せる設計を共通の方針としています。似た名前で関連ツールを開発する場合は、まずご連絡ください。プロジェクトを分散させるよりも、協力して開発したいと考えています。

---

<sub>Revit、AutoCAD、Navisworks、Inventor および Autodesk は Autodesk, Inc. の登録商標です。bimwright は独立したオープンソースプロジェクトであり、Autodesk, Inc. との提携、同社による資金提供、または同社の推奨を受けているものではありません。</sub>
