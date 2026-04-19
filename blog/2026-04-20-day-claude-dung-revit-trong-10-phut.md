---
title: "Dạy Claude dùng Revit trong 10 phút"
date: 2026-04-20
author: bimwright
tags: [revit, bim, mcp, claude, ai, vietnam]
canonical_url: https://github.com/bimwright/.github/blob/master/blog/2026-04-20-day-claude-dung-revit-trong-10-phut.md
summary: rvt-mcp — cây cầu mã nguồn mở cho phép AI agent chỉnh sửa trực tiếp mô hình Revit của bạn, an toàn, không upload lên cloud.
---

# Dạy Claude dùng Revit trong 10 phút

11 giờ đêm. Deadline 9 giờ sáng. PM vừa ghé ngang bàn: *"Em đổi lại quy ước đặt tên Level theo chuẩn mới nhé — L01 - Hầm, L02 - Thương mại, L03 - Văn phòng..."*

Dự án của bạn có 47 level.

Bạn biết chính xác sắp diễn ra gì: click Level 1 → Properties → Name → gõ → Apply. Click Level 2 → Properties → Name → gõ → Apply. Lặp lại 45 lần nữa. Bạn biết có thể viết Dynamo hay pyRevit, nhưng viết xong script thì cũng mất bằng thời gian click tay.

Đây chính là chỗ ngứa mà `rvt-mcp` gãi.

---

## rvt-mcp là gì?

Một process nhỏ chạy song song với Revit. Bạn nói với AI agent (Claude chẳng hạn): *"đổi tên tất cả level theo pattern này"*. Agent gọi 1 trong 28 tool mà `rvt-mcp` expose, tool chạy trong Revit trong **1 transaction duy nhất**. Bạn thấy kết quả ngay trên model. Không vừa ý? **Ctrl+Z — quay ngược cả 47 đổi tên cùng lúc.**

Không cloud. Model của bạn không rời khỏi máy. Apache-2.0. Revit 2022-2027.

---

## Cài trong 10 phút

Cần: Revit 2022-2027, .NET 8 SDK, và 1 AI host (Claude Code, Claude Desktop, Cursor, Cline, Codex, Copilot, Gemini CLI — đều được).

Cách nhanh nhất — **để AI tự cài**:

1. Clone repo: `git clone https://github.com/bimwright/rvt-mcp`
2. Mở `AGENTS.md` cho AI agent của bạn đọc
3. Gõ: *"install this for me"*

Agent đề xuất từng bước, xin phép trước khi chạm vào máy bạn. Bạn approve hoặc reject. Không có gì bị làm lén.

---

## Ví dụ thực tế

Mở Revit. Mở AI host. Gõ:

> *Rename tất cả level: "Level 1" → "L01 - Hầm", "Level 2" → "L02 - Thương mại", "Level 3" → "L03 - Văn phòng". Từ level 4 trở lên: "L04 - Văn phòng L2", "L05 - Văn phòng L3"...*

Agent đề xuất mapping (47 tên cũ ↔ 47 tên mới). Bạn review. Approve. Một transaction — xong.

Không thích? Ctrl+Z. Tất cả về y cũ.

Pattern y hệt cho: tạo sheet hàng loạt, filter elements, set parameters, tạo schedule, tạo level + grid, bóc tách khối lượng vật liệu.

---

## Thay đổi gì cho bạn

1. **Click nhàm chán biến mất.** 1 giờ đổi tên level → 2 phút đối thoại.
2. **Bạn vẫn nắm dây cương.** Mọi thay đổi là Revit transaction — 1 Ctrl+Z rollback hoàn toàn. Không có gì chạy ngầm.
3. **Chuyên môn của bạn được scale.** AI gõ phím hộ, còn *quyết định đặt tên gì* vẫn là của bạn.

Triết lý thiết kế gói gọn 3 từ: **predictable, auditable, reversible** (dự đoán được, kiểm tra được, hoàn nguyên được).

---

## Không phải...

- Không thay thế kiến trúc sư / kỹ sư.
- Không upload model lên cloud.
- Không phải hộp đen — 28 tool, mã nguồn mở, đọc được từng dòng.
- Không phải phép màu — đề xuất của AI cần bạn review trước khi approve.

Nó là **một công cụ**, giống Dynamo là công cụ — chỉ khác ở chỗ hiểu được tiếng người.

---

## Thử xem

Mã nguồn mở, Apache-2.0, Revit 2022-2027:

👉 **https://github.com/bimwright/rvt-mcp**

Star nếu thấy hữu ích. Dùng cho task thật. Gãy thì mở issue — tụi mình đọc hết.

Nếu bạn đang muốn AI thật sự *làm việc* BIM cùng bạn thay vì chỉ nói chuyện — đây là thứ đó.

---

*`rvt-mcp` thuộc [bimwright](https://github.com/bimwright) — bộ MCP server mã nguồn mở cho ngành AEC. Kho kiến thức BIM của tụi mình là [`bim-wiki`](https://github.com/bimwright/bim-wiki) (ISO 19650 + khung pháp lý BIM Việt Nam, CC-BY-SA 4.0) cũng mới ra tuần này.*

***bimwright. Built right.***
