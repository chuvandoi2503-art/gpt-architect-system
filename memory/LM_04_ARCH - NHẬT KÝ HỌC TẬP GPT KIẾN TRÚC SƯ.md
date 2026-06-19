# LM_04_ARCH - NHẬT KÝ HỌC TẬP GPT KIẾN TRÚC SƯ

Phiên bản: 02.000  
Trạng thái: ARCHIVE  
Vai trò: History / Nhật ký học tập, không dùng vận hành hằng ngày

---

## 1. VAI TRÒ CỦA 04

04 là nơi lưu lịch sử học tập nếu cần truy vết.

04 không phải:

- Working Memory.
- Bộ nhớ lõi.
- Bộ nhớ dài hạn đã xác nhận.
- Danh sách công việc.
- File bắt buộc nạp đầu phiên.

04 không cần cập nhật thường xuyên.

---

## 2. NGUYÊN TẮC SỬ DỤNG 04

Chỉ dùng 04 khi cần hiểu:

- Vì sao một quyết định kiến trúc được hình thành.
- Bài học nào dẫn tới thay đổi hệ thống.
- Lỗi nào từng xảy ra trong quá trình phát triển.
- Điều gì đã được kiểm chứng trong quá khứ.

Không dùng 04 để vận hành hằng ngày.

Không dùng 04 làm nguồn chân lý chính.

---

## 3. QUY TẮC CHẮT LỌC BÀI HỌC

Khi có bài học mới:

Nếu GPT phải luôn nhớ:

```text
Đưa vào 03A
```

Nếu là quyết định dài hạn đã xác nhận:

```text
Đưa vào 03B
```

Nếu là trạng thái đang làm:

```text
Đưa vào 04.1
```

Nếu chỉ là lịch sử tham khảo:

```text
Có thể đưa vào 04
```

Nếu không còn giá trị vận hành:

```text
DISCARD
```

---

## 4. CÁC BÀI HỌC ĐÃ ARCHIVE

### Bài học 001 - GPT không phải kho lưu trữ

GPT không phù hợp làm kho lưu trữ tri thức gốc vì có thể rút gọn, mất nội dung hoặc diễn giải lại tài liệu dài.

### Bài học 002 - GPT không thay thế Git

GPT không đảm bảo version, lịch sử thay đổi và khả năng khôi phục.

### Bài học 003 - Knowledge chưa đủ để vận hành

Cần lớp ÁP DỤNG BẮT BUỘC để giữ GPT đi đúng quy tắc trong phiên.

### Bài học 004 - Không nạp toàn bộ bộ nhớ đầu phiên

Nạp quá nhiều tri thức làm tăng nhiễu, tăng chi phí và tăng gánh nặng vận hành.

### Bài học 005 - Cần phân tầng bộ nhớ

Không đồng nhất mọi loại tri thức thành một bộ nhớ duy nhất.

### Bài học 006 - PASS phải có ý nghĩa rõ ràng

Nếu PASS thì không đề xuất sửa tiếp trong cùng lần QC.

### Bài học 007 - GPT Kiến Trúc Sư nên tập trung vào kiến trúc

Vai trò chính là framework, workflow, bộ nhớ, automation và khả năng nhân bản.

### Bài học 008 - Hoàn thiện một GPT mẫu trước

Không xây nhiều GPT chuyên ngành khi framework chưa ổn định.

### Bài học 009 - GitHub Connector và Codex có thể giảm nhu cầu n8n cho repo memory

Nếu cùng hệ thống có công cụ đọc repo và sửa repo tốt hơn, không nên ép dùng n8n cho việc quản lý bộ nhớ GPT.

### Bài học 010 - Không xây workflow chỉ để quản lý workflow

Nếu phát sinh vấn đề rồi tạo thêm workflow, thêm patch, thêm file để xử lý chính độ phức tạp vừa tạo ra thì kiến trúc đang trượt khỏi mục tiêu hỗ trợ người dùng.

### Bài học 011 - Patch không phải bộ nhớ chính

Patch chỉ là giấy nháp / đơn vị vận chuyển thay đổi.

Sau khi cập nhật vào đúng file, patch có thể xóa hoặc archive.

### Bài học 012 - Mục tiêu hiện tại là đóng gói V1, không hoàn hảo hóa

GPT Kiến Trúc Sư V1 chỉ cần đủ dùng để chuyển sang GPT Content.

---

## 5. TRẠNG THÁI

LM_04_ARCH ở trạng thái ARCHIVE.

Không nạp đầu phiên.

Không phải file vận hành chính.

Không cần cập nhật nếu bài học đã được chắt lọc vào 03A, 03B hoặc 04.1.
