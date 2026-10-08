<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="480">
</p>

<p align="center">
  <a href="README.md">English</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.zh-CN.md">简体中文</a> · 日本語
</p>

# bimwright

AI アシスタントと BIM・CAD アプリケーションをつなぐオープンソースのツール。

Model Context Protocol（MCP）を通じて Revit、AutoCAD、Navisworks、Inventor を操作できます。C# で実装したゲートウェイがローカルで動作し、MCP 対応の AI クライアントを各アプリケーションのネイティブ API につなぎます。人の指示と確認のもとで、モデルや図面の調査、繰り返し作業の自動化、ネイティブな形状や技術文書の作成・修正を行います。

**bimwright** は **BIM** と **wright** を組み合わせた名前です。wright は、ものを作る人や建てる人を表す古い英語で、*shipwright*（船大工）などに使われます。私たちは、設計や建設に携わる人のためのツールを開発しています。

---

## ツール

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) — Autodesk® Revit® 向けの MCP ゲートウェイ。BIM モデルの調査、要素の作成・修正、ビュー・シート・モデルデータの操作に対応します。型付きツールとトランザクションを保護するバッチ実行で、エージェントによる BIM 作業とアドイン開発を支援します。Apache-2.0。
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) — Autodesk® AutoCAD® 向けの MCP ゲートウェイ。DWG 図面の調査・編集、形状・文字・ブロック・寸法・注釈の操作、ビューの画像取得と移動に対応します。繰り返しの CAD 作業や、文字を元の位置に書き戻す翻訳ワークフローを支援します。Apache-2.0。
- [**nwd-mcp**](https://github.com/bimwright/nwd-mcp) — Autodesk® Navisworks® Manage 向けの MCP ゲートウェイ。統合モデルのプロパティ照会、項目の検索・選択、表示制御、保存済みビューポイントへの移動で、調整作業と干渉レビューを支援します。Apache-2.0。
- [**ipt-mcp**](https://github.com/bimwright/ipt-mcp) — Autodesk® Inventor® 向けの MCP ゲートウェイ。パラメトリックなパーツ・スケッチ・フィーチャの作成、アセンブリの配置・調査、ビュー・寸法・注釈・表を含むネイティブな製図の作成・調整に対応します。Apache-2.0。
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) — ベトナム語を中心とする BIM ナレッジベース。ISO 19650、情報管理、プロジェクトのデリバリー、ベトナムの BIM 法規制を扱います。CC-BY-SA 4.0。

ゲートウェイは一般的な作業に型付きツールを提供し、その範囲外の作業には C# 実行を利用できます。任意の ToolBaker ワークフローで繰り返すパターンを再利用可能な個人ツールにできますが、自動的な自己学習ではなく、明示的な承認が必要です。インストール方法、対応アプリケーションのバージョン、機能と安全上の制限は、各プロジェクトの README を参照してください。

## 命名について

ゲートウェイの名前は、利用者になじみのあるファイル拡張子に由来します。Revit モデルの `.rvt`、AutoCAD 図面の `.dwg`、Navisworks の統合モデルの `.nwd`、Inventor パーツの `.ipt` です。`<ext>-mcp` という形式で名前を統一することで、各ゲートウェイが対象とするアプリケーションやワークフローを見分けやすくしています。これらは識別の手がかりであり、対応するファイル形式やワークフローを限定するものではありません。

この説明は命名の由来を示すものであり、ファイル形式名の所有権や、それらが商標保護の対象外であることを主張するものではありません。関連する商標は、それぞれの権利者に帰属します。

`<ext>-mcp` ファミリーは、予測可能で、監査でき、操作を取り消せる設計を共通の方針としています。似た名前で関連ツールを開発する場合は、まずご連絡ください。プロジェクトを分散させるよりも、協力して開発したいと考えています。

---

<sub>Autodesk、AutoCAD、DWG、Inventor、Navisworks および Revit は Autodesk, Inc. および／またはその子会社・関連会社の商標または登録商標です。bimwright は独立したオープンソースプロジェクトであり、Autodesk, Inc. との提携、同社による資金提供、または同社の推奨を受けているものではありません。</sub>
