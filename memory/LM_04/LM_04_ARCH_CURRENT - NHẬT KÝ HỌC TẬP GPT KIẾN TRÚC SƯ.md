# LM_04_ARCH_CURRENT

Phiên bản: 03.001

---

# MỤC ĐÍCH

Lưu:

- Bài học triển khai
- Kết quả kiểm chứng
- Lỗi hệ thống đã phát hiện
- Kinh nghiệm vận hành

Không dùng để lưu tri thức đã xác nhận lâu dài.

Các tri thức ổn định phải chuyển sang:

LM_03B_CURRENT

---

# NHẬT KÝ HỌC TẬP

## Bài học 001

Chủ đề:

Tách Core Repository khỏi Runtime Repository

Kết quả:

PASS

Bài học:

Khi số lượng GPT tăng lên, việc đặt:

- RULE_COMMON
- MEMORY_ARCHITECTURE
- MEMORY_INDEX
- PATCH_STANDARD
- NAMING_CONVENTION

vào một Core Repository riêng giúp:

- Dễ nhân bản
- Dễ bảo trì
- Giảm trùng lặp

---

## Bài học 002

Chủ đề:

Memory tăng trưởng vô hạn

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

## Bài học 003

Chủ đề:

Khởi tạo phiên quá tải

Kết quả:

PASS

Bài học:

Không nên nạp toàn bộ memory đầu phiên.

Nạp tối thiểu:

- RULE_COMMON
- RULE_<GPT>
- WM_03A
- WM_04_1_DAILY
- LM_03B_CURRENT

Các file khác chỉ đọc khi cần.

---

## Bài học 004

Chủ đề:

PATCH tồn đọng

Kết quả:

PASS

Bài học:

PATCH không phải bộ nhớ.

PATCH không phải nguồn chân lý.

PATCH chỉ tồn tại trong phiên hiện tại.

Sau khi ghi GitHub:

PATCH hoàn tất.

---

## Bài học 005

Chủ đề:

Tổ chức thư mục memory

Kết quả:

PASS

Bài học:

Không nên đặt toàn bộ file trong:

memory/

Giải pháp đã xác nhận:

memory/

├── WM_03A/
├── WM_04_1/
├── LM_03B/
└── LM_04/

Giúp:

- Dễ tìm kiếm
- Dễ archive
- Dễ mở rộng

---

## Bài học 006

Chủ đề:

Quy tắc archive

Kết quả:

PASS

Bài học:

LM_03B_ARCHIVE

Chia theo:

- Chủ đề

Không chia theo:

- Thời gian

---

LM_04_ARCHIVE

Chia theo:

- Thời gian

Ví dụ:

LM_04_ARCHIVE_2026_06

LM_04_ARCHIVE_2026_07

LM_04_ARCHIVE_2026_08

---

# QUY TẮC CHUYỂN DỮ LIỆU

Nếu bài học trở thành:

- Quy trình chuẩn
- Kiến trúc chuẩn
- Tri thức ổn định

Thì chuyển sang:

LM_03B_CURRENT

---

# QUY TẮC TỔNG HỢP

Khi LM_04_CURRENT quá lớn:

- Tổng hợp
- Rút gọn
- Chuyển sang LM_04_ARCHIVE_YYYY_MM

Không để CURRENT tăng trưởng vô hạn.

---

# KHÔNG LƯU

Không lưu:

- Công việc đang dở
- Backlog
- Dự án đang triển khai

Các nội dung đó thuộc:

WM_04_1_DAILY

hoặc

WM_04_1_LONG
