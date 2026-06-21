# LM_03B_ARCH_ARCHIVE_001 - TRI THỨC LƯU TRỮ GPT KIẾN TRÚC SƯ

Phiên bản: 03.001

---

# MỤC ĐÍCH

Lưu các tri thức đã được xác nhận nhưng không cần nạp mặc định đầu phiên.

File này là archive dài hạn.

Chỉ đọc khi:

- Thiếu dữ liệu
- Cần tra cứu lịch sử quyết định
- Cần review kiến trúc cũ
- Cần phục hồi bối cảnh

---

# 1. GPT KHÔNG PHẢI KHO LƯU TRỮ

Đã xác nhận.

GPT không phù hợp để:

- Lưu trữ tri thức gốc
- Quản lý tài liệu gốc
- Là nguồn chân lý duy nhất

Lý do:

GPT có thể diễn giải lại nội dung.

GPT không đảm bảo tính toàn vẹn dữ liệu.

---

# 2. GPT KHÔNG PHẢI HỆ QUẢN LÝ PHIÊN BẢN

Đã xác nhận.

GPT không thay thế:

- Git
- Version Control
- Hệ quản lý thay đổi

Version phải được quản lý bởi hệ thống chuyên trách.

---

# 3. TÁCH BỘ NHỚ KHỎI GPT

Đã xác nhận.

Tri thức dài hạn phải nằm ngoài GPT.

GPT chỉ nạp phần cần thiết để vận hành.

---

# 4. KIẾN TRÚC HỆ THỐNG GỐC

Đã xác nhận.

Kiến trúc hình thành framework:

Git

↓

n8n

↓

GPT

Git:

- Version
- Diff
- Rollback
- Nguồn chân lý

n8n:

- Điều phối
- Automation
- Validation

GPT:

- Suy luận
- Phân tích
- Hỗ trợ quyết định

---

# 5. NGUYÊN TẮC QUẢN TRỊ TRI THỨC

Đã xác nhận.

Không sử dụng GPT làm nguồn chân lý.

Không nạp toàn bộ bộ nhớ đầu phiên.

Truy xuất theo nhu cầu.

---

# 6. QUAN ĐIỂM VỀ DIFF VÀ ROLLBACK

Đã xác nhận.

Không ưu tiên loại bỏ hoàn toàn lỗi.

Ưu tiên:

Phát hiện lỗi nhanh

↓

Xác định phiên bản sai

↓

Diff

↓

Rollback

Git là lớp bảo vệ chính.

---

# 7. QUAN ĐIỂM VỀ GPT → N8N → GIT

Đã xác nhận.

Đây là phần khó nhất của hệ thống.

Vì quyết định:

- Ai được cập nhật tri thức
- Tri thức nào được lưu
- Tri thức nào bị từ chối
- Khả năng rollback

Trọng tâm:

Ghi đúng

↓

Phát hiện sai

↓

Rollback được

↓

Khôi phục được

---

# 8. QUY ƯỚC ĐỊNH DANH HỆ THỐNG

Đã xác nhận.

Nguyên tắc:

Con người nhớ tên.

Hệ thống nhớ ID.

Mỗi thành phần phải có:

- ID ổn định
- Tên hiển thị

Định dạng:

ID - TÊN HIỂN THỊ

Ví dụ:

WM_03A_ARCH - BỘ NHỚ LÕI GPT KIẾN TRÚC SƯ

LM_03B_ARCH - BỘ NHỚ DÀI HẠN GPT KIẾN TRÚC SƯ

LM_04_ARCH - NHẬT KÝ HỌC TẬP GPT KIẾN TRÚC SƯ

---

# 9. QUY ƯỚC ID

Đã xác nhận.

KN = Knowledge

WM = Working Memory

LM = Long-term Memory

RULE = Rule

WF = Workflow

PATCH = Patch

ARCH = GPT KIẾN TRÚC SƯ

CONTENT = GPT CONTENT OS

CRM = GPT CRM

SALES = GPT SALES

---

# 10. QUY ƯỚC PATCH

Đã xác nhận.

Định dạng:

PATCH_[GPT_ID]_[YYYYMMDD]_[STT]

Ví dụ:

PATCH_ARCH_20260616_001

Nguyên tắc:

- PATCH viết hoa
- GPT_ID viết hoa
- STT 3 chữ số
- Patch mới chỉ CREATE
- Không ghi đè patch cũ

---

# 11. QUY ƯỚC WORKFLOW

Đã xác nhận.

Định dạng:

WF_[TÊN_WORKFLOW]_[VERSION]

Ví dụ:

WF_PATCH_V1

WF_MERGE_PATCH_V1

WF_ROLLBACK_V1

---

# 12. QUAN ĐIỂM VỀ AI QC ĐỘC LẬP

Đã xác nhận.

Mặc định không sử dụng AI QC độc lập.

Ưu tiên:

- Version
- Diff
- Rollback
- Git History

AI QC là thành phần mở rộng tương lai.

Không phải thành phần bắt buộc.

---

# 13. BACKUP AWARE MERGE

Đã xác nhận.

WF_MERGE_PATCH_V1 lưu:

- PATCH_STATUS
- TARGET_PATH
- BACKUP_CREATED_AT
- PRE_MERGE_CONTENT

Mục tiêu:

- Hỗ trợ rollback
- Không phụ thuộc trí nhớ GPT
- Không phụ thuộc hội thoại

---

# 14. KHÔNG MỞ RỘNG KHI NỀN CHƯA ỔN

Đã xác nhận.

Ưu tiên:

Ổn định nền

↓

Kiểm chứng

↓

Nhân bản

Không mở rộng GPT mới khi framework chưa ổn định.

---

# 15. LỊCH SỬ HÌNH THÀNH FRAMEWORK

Các quyết định nền tảng hình thành từ:

- GPT không phải kho lưu trữ
- GPT không phải Git
- Tách bộ nhớ khỏi GPT
- Diff quan trọng hơn AI QC
- Registry Driven Architecture
- Automation Safety First
- Patch Based Architecture

Các quyết định này đã được lưu archive để phục vụ tra cứu về sau.

---

# TRẠNG THÁI

Archive này chứa tri thức nền ổn định.

Không nạp mặc định đầu phiên.

Chỉ đọc khi cần tra cứu hoặc phục hồi bối cảnh kiến trúc.
