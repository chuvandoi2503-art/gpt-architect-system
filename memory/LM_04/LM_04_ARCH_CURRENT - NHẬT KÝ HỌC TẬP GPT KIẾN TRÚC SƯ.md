# LM_04_ARCH_CURRENT - NHẬT KÝ HỌC TẬP GPT KIẾN TRÚC SƯ

Phiên bản: 03.001

---

# MỤC ĐÍCH

Lưu:

- Bài học gần đây
- Kết quả kiểm chứng gần đây
- Phát hiện kiến trúc mới
- Kinh nghiệm vận hành mới

File này được phép đọc khi cần hiểu bối cảnh phát triển gần đây.

Không dùng để lưu tri thức nền ổn định.

Các tri thức đã xác nhận phải chuyển sang:

LM_03B_ARCH_CURRENT

hoặc

LM_03B_ARCH_ARCHIVE

---

# BÀI HỌC 001

Chủ đề:

Tách Core Repository khỏi Runtime Repository.

Kết quả:

PASS

Bài học:

Core Repository giúp:

- Dùng chung quy tắc
- Dùng chung kiến trúc
- Dùng chung schema
- Dễ nhân bản GPT mới

Runtime Repository chỉ chứa dữ liệu riêng của từng GPT.

---

# BÀI HỌC 002

Chủ đề:

Memory tăng trưởng vô hạn.

Kết quả:

PASS

Bài học:

Không nên sử dụng:

- Một file WM_04_1 duy nhất
- Một file LM_03B duy nhất
- Một file LM_04 duy nhất

Giải pháp đã xác nhận:

WM_04_1

↓

DAILY + LONG

LM_03B

↓

CURRENT + ARCHIVE

LM_04

↓

CURRENT + ARCHIVE

---

# BÀI HỌC 003

Chủ đề:

Khởi tạo phiên quá tải.

Kết quả:

PASS

Bài học:

Không nạp toàn bộ memory đầu phiên.

Nạp tối thiểu:

- RULE_COMMON
- RULE_ARCH
- WM_03A_ARCH
- WM_04_1_ARCH_DAILY
- LM_03B_ARCH_CURRENT

Các file khác chỉ đọc khi cần.

---

# BÀI HỌC 004

Chủ đề:

PATCH không phải bộ nhớ.

Kết quả:

PASS

Bài học:

PATCH chỉ là cơ chế thay đổi.

PATCH không phải:

- Knowledge
- Working Memory
- Long-term Memory

Sau khi ghi GitHub:

PATCH hoàn tất.

---

# BÀI HỌC 005

Chủ đề:

Workflow nên được review trước khi build.

Kết quả:

PASS

Bài học:

Thứ tự đúng:

Thiết kế

↓

QC kiến trúc

↓

Review Failure Cases

↓

Review Rollback Cases

↓

Review Dependency

↓

Người dùng duyệt

↓

Build

Không nên:

Build

↓

Lỗi

↓

Sửa

↓

Lỗi tiếp

---

# BÀI HỌC 006

Chủ đề:

Workflow lỗi thường nằm ở dữ liệu hơn là code.

Kết quả:

PASS

Bài học:

Khi workflow lỗi:

Ưu tiên kiểm tra:

Kiến trúc dữ liệu

↓

Luồng dữ liệu

↓

Mapping

↓

Sau đó mới tới code

---

# BÀI HỌC 007

Chủ đề:

WF_PATCH_V1.

Kết quả:

PASS THỰC TẾ

Đã kiểm chứng:

- Webhook
- Validate Input
- Generate Patch
- GitHub Create File
- Auto Increment Patch Number
- Build Response
- Respond To Webhook

Bài học:

GPT không nên ghi trực tiếp file gốc.

Patch là lớp trung gian phù hợp.

---

# BÀI HỌC 008

Chủ đề:

WF_MERGE_PATCH_V1.

Kết quả:

PASS THỰC TẾ

Bài học:

Patch phải được duyệt trước khi merge.

Patch đã MERGED không được merge lại.

GitHub giữ lịch sử thay đổi.

Người dùng là người duyệt cuối cùng.

---

# BÀI HỌC 009

Chủ đề:

WF_ROLLBACK_V1.

Kết quả:

PASS CÓ LƯU Ý

Bài học:

Rollback bằng commit mới.

Không dùng git reset.

Không phá lịch sử Git.

---

# BÀI HỌC 010

Chủ đề:

Kiến trúc PATCH → MERGE → ROLLBACK.

Kết quả:

PASS

Bài học:

Một kiến trúc quản lý thay đổi hoàn chỉnh cần:

PATCH

↓

APPROVE

↓

MERGE

↓

ROLLBACK

Trong đó:

- PATCH tạo thay đổi
- APPROVE xác nhận thay đổi
- MERGE áp dụng thay đổi
- ROLLBACK khôi phục thay đổi

---

# BÀI HỌC 011

Chủ đề:

Registry Driven Architecture.

Kết quả:

PASS

Bài học:

Workflow không nên hardcode:

- GPT_ID
- TARGET_ID
- GitHub Path

Workflow nên resolve thông qua Registry.

Điều này giúp:

- Dễ mở rộng
- Dễ nhân bản
- Không sửa workflow khi thêm GPT mới

---

# TRẠNG THÁI

File này chỉ giữ các bài học còn giá trị vận hành gần đây.

Khi quá lớn:

Tổng hợp

↓

Rút gọn

↓

Chuyển sang:

LM_04_ARCH_ARCHIVE_YYYY_MM
