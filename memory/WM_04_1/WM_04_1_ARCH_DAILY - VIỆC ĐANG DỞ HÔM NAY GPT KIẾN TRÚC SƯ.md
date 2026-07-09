# WM_04_1_ARCH_DAILY

Phiên bản: 03.001

---

# MỤC ĐÍCH

Lưu việc đang dở trong ngày hoặc phiên làm việc gần nhất.

Đây là file Working Memory được nạp mặc định đầu phiên.

File được phép ghi đè.

Không dùng để lưu lịch sử dài hạn.

Không dùng để lưu backlog.

Không dùng để lưu tri thức.

---

# CÔNG VIỆC ĐÃ HOÀN THÀNH

## 1. GPT Research V1

Trạng thái:

PASS

Đã chốt kiến trúc vận hành:

- Research chỉ nhận Research Request.
- Knowledge Gap do GPT Content xác định.
- Research không QC Profile.
- Research chỉ QC chất lượng viên gạch.
- Research trả Research Package.
- Bổ sung Definition of Done.
- Hoàn thiện RULE_RESEARCH V1.

---

## 2. Kiến trúc Content

Trạng thái:

PASS

Đã thống nhất luồng vận hành:

Input thật

↓

QC Input

↓

Xác định Profile

↓

Tra Profile

↓

Knowledge Gap

↓

Research Request

↓

Research

↓

Research Package

↓

Content

↓

Kiến trúc nội dung

↓

Output

↓

QC

↓

Đề xuất cập nhật Profile

---

# PHÁT HIỆN KIẾN TRÚC

## 1.

Knowledge Gap thuộc trách nhiệm của Content.

Không thuộc Research.

---

## 2.

Research chỉ chịu trách nhiệm:

- Search.
- Chuẩn hóa.
- QC chất lượng viên gạch.
- Đóng gói Research Package.

---

## 3.

Profile sẽ là Domain Knowledge.

Không còn được xem là Memory.

---

## 4.

Không tạo Search Layer.

Không tạo Index riêng.

Quyết định giữ kiến trúc tối giản cho đến khi có điểm nghẽn thực tế.

---

# CÔNG VIỆC ĐANG DỞ

## VIỆC ĐANG DỞ CẦN TIẾP TỤC PHIÊN SAU
Trọng tâm phiên sau

Kiến trúc GPT / hệ thống học tiếng Anh thực tế cho:

-Anh
-Con 34 tháng tuổi
-Hai bố con học cùng nhau

## Hướng kiến trúc đã chốt tạm

Không tạo GPT dạy tiếng Anh đơn lẻ.

Tạo hệ:

ENGLISH LEARNING OS

Mục tiêu:

Biến tiếng Anh thành một phần của cuộc sống thật của hai bố con.

## Phiên sau cần làm
1. Xác định mục tiêu học tiếng Anh của bố.
2. Xác định mục tiêu học tiếng Anh của con 34 tháng.
3. Thiết kế roadmap thực tế.
4. Thiết kế bài học hằng ngày.
5. Thiết kế kiểm tra nghe / nói / đọc / viết.
6. Gợi ý app, phần mềm, kênh học ưu tiên miễn phí.
7.Tận dụng Reality Pack / Data Brick từ Đợi Làm Bố.
8.Thiết kế cách ghi tiến độ học.
9.Thiết kế cách Content OS và English OS dùng chung dữ liệu đời sống.

---

# GHI CHÚ

Không phát sinh thay đổi Core.

Không phát sinh thay đổi Project.

Không lưu tri thức dài hạn.

Chỉ lưu trạng thái triển khai để tiếp tục phiên sau.

---

# QUY TẮC

Chỉ lưu:

- Việc đang làm
- Việc đang dở
- Bước tiếp theo

Không lưu:

- Tri thức
- Nhật ký học tập
- Backlog dài hạn
- Quy trình hệ thống

Các nội dung trên phải được lưu vào file đúng chức năng theo MEMORY_ARCHITECTURE.
