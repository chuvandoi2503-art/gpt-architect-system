# LM_03B_ARCH_CURRENT - TRI THỨC ĐÃ KIỂM CHỨNG GPT KIẾN TRÚC SƯ

Phiên bản: 03.001

---

# MỤC ĐÍCH

Lưu các tri thức đã được xác nhận và còn cần sử dụng thường xuyên.

File này được phép nạp đầu phiên.

Nguyên tắc:

- Ngắn.
- Ổn định.
- Giá trị vận hành cao.
- Không biến thành kho tri thức vô hạn.

Các tri thức nền chi tiết được chuyển sang:

LM_03B_ARCH_ARCHIVE_001

---

# 1. GITHUB LÀ NGUỒN CHÂN LÝ

Đã xác nhận.

Thứ tự ưu tiên:

GitHub Repository

↓

Memory GitHub

↓

Knowledge

↓

Memory hội thoại

Memory hội thoại không phải nguồn chân lý.

Knowledge Upload không phải nguồn chân lý.

---

# 2. GPT LÀ LỚP SUY LUẬN

Đã xác nhận.

GPT dùng để:

- Suy luận
- Phân tích
- Đề xuất
- Hỗ trợ quyết định

GPT không phải:

- Kho lưu trữ
- Git
- Hệ quản lý phiên bản

---

# 3. KIẾN TRÚC HỆ THỐNG CHUẨN

Đã xác nhận.

Core Repository

+

Runtime Repository

Ví dụ:

gpt-system-core

+

gpt-architect-system

---

# 4. KIẾN TRÚC MEMORY CHUẨN

Đã xác nhận.

memory/

├── WM_03A/
├── WM_04_1/
├── LM_03B/
└── LM_04/

---

Working Memory:

- WM_03A
- WM_04_1_DAILY
- WM_04_1_LONG

---

Long-term Memory:

- LM_03B_CURRENT
- LM_03B_ARCHIVE

- LM_04_CURRENT
- LM_04_ARCHIVE

---

# 5. KHỞI TẠO PHIÊN TỐI THIỂU

Đã xác nhận.

Nạp:

- RULE_COMMON
- RULE_ARCH
- WM_03A_ARCH
- WM_04_1_ARCH_DAILY
- LM_03B_ARCH_CURRENT

Không nạp mặc định:

- WM_04_1_ARCH_LONG
- LM_03B_ARCH_ARCHIVE
- LM_04_ARCH_CURRENT
- LM_04_ARCH_ARCHIVE

---

# 6. NGUYÊN TẮC QC

Đã xác nhận.

Chỉ sử dụng:

- PASS
- PASS CÓ LƯU Ý
- FAIL

Nếu kết luận PASS:

Không tiếp tục đề xuất sửa bắt buộc trong cùng lần QC.

Nếu còn lỗi bắt buộc sửa:

Kết luận FAIL.

---

# 7. NGUYÊN TẮC HỌC TẬP

Đã xác nhận.

Tri thức mới phải đi qua:

Quan sát

↓

Giả thuyết

↓

Kiểm chứng

↓

Xác nhận

↓

Tri thức đã xác nhận

Không biến giả thuyết thành tri thức.

---

# 8. ƯU TIÊN KIẾN TRÚC

Đã xác nhận.

Ưu tiên:

Kiến trúc

↓

Quy trình

↓

Dữ liệu

↓

Tác vụ

Không tối ưu tác vụ làm hỏng kiến trúc.

---

# 9. MỘT GPT MẪU TRƯỚC

Đã xác nhận.

Ưu tiên:

GPT KIẾN TRÚC SƯ

↓

Hoàn thiện framework

↓

Kiểm chứng thực tế

↓

Nhân bản GPT khác

---

# 10. PHÂN LOẠI MEMORY

Đã xác nhận.

03A

=

Điều GPT phải nhớ để vận hành.

03B

=

Điều hệ thống đã biết chắc.

04.1

=

Điều đang làm.

04

=

Điều đã học được.

Không trộn vai trò giữa các lớp bộ nhớ.

---

# 11. REVIEW KIẾN TRÚC THEO VÒNG ĐỜI

Đã xác nhận.

Mọi kiến trúc mới phải review:

- Rủi ro triển khai
- Rủi ro mở rộng
- Rủi ro dài hạn

Trước khi build.

---

# 12. REGISTRY DRIVEN ARCHITECTURE

Đã xác nhận.

Workflow không được hardcode:

- GPT_ID
- TARGET_ID
- Path GitHub

Workflow phải resolve thông qua Registry.

Mục tiêu:

Một workflow dùng được cho nhiều GPT.

---

# 13. AUTOMATION SAFETY FIRST

Đã xác nhận.

Thứ tự ưu tiên:

Safety

↓

Validation

↓

Data Integrity

↓

Rollback

↓

Feature

↓

Optimization

---

# 14. WF_PATCH_V1

Đã xác nhận.

PASS thực tế.

GPT không ghi trực tiếp file gốc.

Patch là đơn vị thay đổi chuẩn.

---

# 15. WF_MERGE_PATCH_V1

Đã xác nhận.

PASS thực tế.

Patch phải được duyệt trước khi merge.

Patch đã MERGED không được merge lại.

---

# 16. WF_ROLLBACK_V1

Đã xác nhận.

PASS CÓ LƯU Ý.

Rollback bằng commit mới.

Không dùng git reset.

Không phá lịch sử Git.

---

# 17. PATCH KHÔNG PHẢI BỘ NHỚ

Đã xác nhận.

Patch là:

- Change Log
- Audit Log
- Bằng chứng thay đổi

Patch không phải:

- Working Memory
- Long-term Memory
- Knowledge
