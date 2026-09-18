<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="480">
</p>

<p align="center">
  <a href="README.md">English</a> · Tiếng Việt · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a>
</p>

# bimwright

Các công cụ mã nguồn mở kết nối trợ lý AI với ứng dụng BIM và CAD.

Làm việc với Revit, AutoCAD, Navisworks và Inventor qua Model Context Protocol (MCP). Truy vấn mô hình, tự động hóa công việc lặp lại và thực hiện thay đổi bằng API gốc của các ứng dụng.

Tên **bimwright** ghép **BIM** với **wright**, một từ tiếng Anh cổ chỉ người thợ chế tạo hoặc xây dựng — như trong *shipwright* (thợ đóng tàu). Chúng tôi làm công cụ cho những người làm thiết kế và xây dựng.

---

## Tools

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) — MCP gateway cho Autodesk® Revit® 2022–2027. Expose Revit API thành các tool AI gọi được, có progressive disclosure (toolset gating), batch execution an toàn về transaction, và ToolBaker self-evolution engine.
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) — MCP gateway cho Autodesk® AutoCAD® 2022–2027. Đọc text trong bản vẽ, nhóm fragment theo không gian, ghi lại bản dịch tại chỗ, và chạy code có audit trong một workflow có thể undo.
- [**nwd-mcp**](https://github.com/bimwright/nwd-mcp) — MCP gateway cho Autodesk® Navisworks® Manage 2022–2027. Query, inspect và điều hướng mô hình phối hợp (federated) để clash review, bảo mật bằng TCP chỉ-loopback và token theo từng session.
- [**ipt-mcp**](https://github.com/bimwright/ipt-mcp) — MCP gateway cho Autodesk® Inventor® 2022–2027. Điều khiển dựng hình parametric part/sketch/feature, parameter và iProperty dưới dạng tool AI gọi được, trên stack add-in đa phiên bản viết thuần C#.
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) — Kho kiến thức BIM ưu tiên tiếng Việt: ISO 19650 + khung pháp lý Việt Nam (QĐ 347/348/1057/2500, Luật 60/2024, Nghị định 111/2024/175/2024, Thông tư 09/2024/24/2025). Giấy phép CC-BY-SA 4.0.

Cả họ `<ext>-mcp` dùng chung một pattern kiến trúc: predictable, auditable, reversible. Nếu bạn đang nghĩ đến việc tự build một cái tương tự dưới tên gần giống, vui lòng liên hệ trước — chúng tôi muốn hợp tác hơn là làm fragment thị trường.

---

<sub>Revit, AutoCAD, Navisworks, Inventor và Autodesk là thương hiệu đã đăng ký của Autodesk, Inc. bimwright là một dự án open-source độc lập, không liên kết, không được tài trợ, và không được bảo chứng bởi Autodesk, Inc.</sub>
