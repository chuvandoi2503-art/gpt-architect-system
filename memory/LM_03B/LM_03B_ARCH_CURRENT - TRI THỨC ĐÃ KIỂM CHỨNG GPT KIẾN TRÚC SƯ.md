# LM_03B_ARCH_CURRENT

Phiên bản: 03.001

---

# MỤC ĐÍCH

Lưu:

- Tri thức đã kiểm chứng
- Kiến trúc đã xác nhận
- Quy trình đã xác nhận
- Workflow đã xác nhận

Có thể nạp đầu phiên.

---

# TRI THỨC ĐÃ KIỂM CHỨNG

## Core Repository + Runtime Repository

Trạng thái:

Đã xác nhận.

Kiến trúc chuẩn:

Core Repository

+

Runtime Repository

Ví dụ:

gpt-system-core

+

gpt-architect-system

hoặc

gpt-system-core

+

gpt-content-director-system

---

## GitHub Là Nguồn Chân Lý

Trạng thái:

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

## Cấu Trúc Memory Chuẩn

Trạng thái:

Đã xác nhận.

Runtime Repository sử dụng:

memory/

├── WM_03A/
├── WM_04_1/
├── LM_03B/
└── LM_04/

---

## Working Memory Tách DAILY Và LONG

Trạng thái:

Đã xác nhận.

WM_04_1_DAILY

Dùng cho:

- Việc đang làm
- Việc đang dở gần nhất

Nạp đầu phiên.

---

WM_04_1_LONG

Dùng cho:

- Dự án
- Backlog
- Công việc tuần
- Công việc tháng
- Công việc quý

Không nạp mặc định đầu phiên.

---

## LM_03B Chia CURRENT Và ARCHIVE

Trạng thái:

Đã xác nhận.

CURRENT

Dùng cho:

- Tri thức mới xác nhận
- Quy trình mới xác nhận

Có thể nạp đầu phiên.

---

ARCHIVE

Dùng cho:

- Tri thức ổn định
- Tri thức ít thay đổi

Không nạp đầu phiên.

---

## LM_04 Chia CURRENT Và ARCHIVE

Trạng thái:

Đã xác nhận.

CURRENT

Dùng cho:

- Nhật ký gần đây
- Kết quả kiểm chứng gần đây

---

ARCHIVE

Dùng cho:

- Lịch sử cũ
- Nhật ký cũ

Không nạp đầu phiên.

---

## Không Lưu Patch Tồn Đọng

Trạng thái:

Đã xác nhận.

PATCH chỉ là cơ chế trung gian.

Sau khi ghi GitHub:

PATCH hoàn tất.

Không tạo:

- Patch backlog
- Patch archive
- Patch repository

---

## Một Nguồn Chân Lý

Trạng thái:

Đã xác nhận.

Không tạo nhiều file cùng mô tả một kiến trúc.

Ưu tiên:

Một kiến trúc

↓

Một file

↓

Một nguồn chân lý

---

# QUY TẮC TỔNG HỢP

Khi LM_03B_CURRENT quá lớn:

- Tổng hợp
- Rút gọn
- Chuyển tri thức ổn định sang LM_03B_ARCHIVE

Không để CURRENT tăng trưởng vô hạn.

---

# KHÔNG LƯU

Không lưu:

- Ý tưởng
- Giả thuyết
- Suy đoán
- Nội dung chưa kiểm chứng

Chỉ lưu nội dung đã được xác nhận trong thực tế vận hành.
