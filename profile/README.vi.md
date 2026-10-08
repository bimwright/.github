<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="480">
</p>

<p align="center">
  <a href="README.md">English</a> · Tiếng Việt · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a>
</p>

# bimwright

Các công cụ mã nguồn mở kết nối trợ lý AI với ứng dụng BIM và CAD.

Làm việc với Revit, AutoCAD, Navisworks và Inventor qua Model Context Protocol (MCP). Các gateway viết bằng C# chạy local, kết nối client AI hỗ trợ MCP với API gốc của ứng dụng. Khảo sát mô hình và bản vẽ, tự động hóa công việc lặp lại, tạo hoặc chỉnh sửa hình học và tài liệu kỹ thuật native dưới sự chỉ dẫn và kiểm tra của con người.

Tên **bimwright** ghép **BIM** với **wright**, một từ tiếng Anh cổ chỉ người thợ chế tạo hoặc xây dựng — như trong *shipwright* (thợ đóng tàu). Chúng tôi làm công cụ cho những người làm thiết kế và xây dựng.

---

## Công cụ

- [**rvt-mcp**](https://github.com/bimwright/rvt-mcp) — MCP gateway cho Autodesk® Revit®. Khảo sát mô hình BIM, tạo và chỉnh sửa element, làm việc với view, sheet và dữ liệu mô hình. Các tool có kiểu dữ liệu rõ ràng và batch an toàn về transaction hỗ trợ quy trình BIM qua agent và phát triển add-in. Apache-2.0.
- [**dwg-mcp**](https://github.com/bimwright/dwg-mcp) — MCP gateway cho Autodesk® AutoCAD®. Khảo sát và chỉnh sửa bản vẽ DWG; làm việc với hình học, text, block, kích thước và chú thích; chụp và điều hướng view bản vẽ. Hỗ trợ công việc CAD lặp lại và quy trình dịch text tại chỗ. Apache-2.0.
- [**nwd-mcp**](https://github.com/bimwright/nwd-mcp) — MCP gateway cho Autodesk® Navisworks® Manage. Truy vấn thuộc tính, tìm và chọn đối tượng, điều khiển hiển thị và điều hướng viewpoint đã lưu trong mô hình tổng hợp để hỗ trợ phối hợp và rà soát xung đột. Apache-2.0.
- [**ipt-mcp**](https://github.com/bimwright/ipt-mcp) — MCP gateway cho Autodesk® Inventor®. Dựng part, sketch và feature tham số; bố trí và khảo sát assembly; tạo và hoàn thiện bản vẽ kỹ thuật native với view, kích thước, chú thích và bảng. Apache-2.0.
- [**bim-wiki**](https://github.com/bimwright/bim-wiki) — Kho kiến thức BIM ưu tiên tiếng Việt, bao gồm ISO 19650, quản lý thông tin, triển khai dự án và khung pháp lý BIM tại Việt Nam. CC-BY-SA 4.0.

Các gateway cung cấp tool có kiểu dữ liệu rõ ràng cho tác vụ phổ biến và khả năng chạy C# cho công việc ngoài phạm vi đó. Quy trình ToolBaker tùy chọn biến pattern lặp lại thành tool cá nhân tái sử dụng, cần chấp thuận rõ ràng thay vì tự động tự học. README của từng dự án trình bày cách cài đặt, phiên bản ứng dụng hỗ trợ, khả năng và giới hạn an toàn.

## Cách đặt tên

Tên các gateway lấy cảm hứng từ phần mở rộng tệp quen thuộc: `.rvt` cho mô hình Revit, `.dwg` cho bản vẽ AutoCAD, `.nwd` cho mô hình phối hợp Navisworks và `.ipt` cho chi tiết Inventor. Quy ước `<ext>-mcp` giúp người dùng nhận ra ứng dụng và quy trình mà mỗi gateway phục vụ, đồng thời giữ cách gọi nhất quán trong cả nhóm dự án. Đây là dấu hiệu nhận diện, không phải giới hạn về loại tệp hoặc quy trình mà gateway hỗ trợ.

Cách đặt tên giải thích nguồn gốc dự án, không hàm ý chúng tôi sở hữu tên định dạng tệp hoặc các tên đó nằm ngoài phạm vi bảo hộ nhãn hiệu. Các nhãn hiệu liên quan thuộc chủ sở hữu tương ứng.

Cả họ `<ext>-mcp` dùng chung một pattern kiến trúc: predictable, auditable, reversible. Nếu bạn đang nghĩ đến việc tự build một cái tương tự dưới tên gần giống, vui lòng liên hệ trước — chúng tôi muốn hợp tác hơn là làm fragment thị trường.

---

<sub>Autodesk, AutoCAD, DWG, Inventor, Navisworks và Revit là nhãn hiệu hoặc nhãn hiệu đã đăng ký của Autodesk, Inc. và/hoặc các công ty con, công ty liên kết. bimwright là một dự án open-source độc lập, không liên kết, không được tài trợ, và không được bảo chứng bởi Autodesk, Inc.</sub>
