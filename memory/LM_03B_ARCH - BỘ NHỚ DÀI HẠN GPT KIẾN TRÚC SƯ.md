# LM_03B_ARCH - BỘ NHỚ DÀI HẠN GPT KIẾN TRÚC SƯ

Phiên bản: 02.000  
Trạng thái: V1 RÚT GỌN  
Vai trò: Long-term Memory, chỉ lưu quyết định dài hạn đã xác nhận

---

## 1. VAI TRÒ CỦA 03B

03B lưu các quyết định, nguyên tắc và tri thức đã được xác nhận, còn giá trị sử dụng dài hạn.

03B không phải nhật ký học tập.

03B không phải danh sách công việc.

03B không nạp đầu phiên theo mặc định.

Chỉ truy xuất 03B khi:

- Working Memory không đủ.
- Cần kiểm tra lại quyết định dài hạn.
- Có mâu thuẫn kiến trúc.
- Người dùng yêu cầu tra lại.

---

## 2. GPT KHÔNG PHẢI NGUỒN CHÂN LÝ

Đã xác nhận.

GPT không phải:

- Kho lưu trữ tri thức gốc.
- Git.
- Database.
- Hệ quản lý version.
- Nguồn chân lý duy nhất.

Nguồn chân lý phải nằm ngoài GPT.

GitHub là nguồn chân lý hiện tại cho tài liệu lõi.

---

## 3. KIẾN TRÚC HỆ THỐNG ĐÃ CHỐT

Kiến trúc V1 rút gọn:

```text
ChatGPT / GPT Kiến Trúc Sư
↓
GitHub Connector
↓
GitHub Repository
↓
Codex
```

Vai trò:

GitHub:

- Version.
- Lịch sử thay đổi.
- Nguồn chân lý.
- Diff.
- Rollback.

GPT Kiến Trúc Sư:

- Suy luận.
- Phân tích.
- Thiết kế kiến trúc.
- Cảnh báo rủi ro.
- Đề xuất nội dung cập nhật.

Codex:

- Sửa repo.
- Tạo diff.
- Tạo PR.
- Hỗ trợ review thay đổi.

n8n:

- Không dùng cho bộ nhớ GPT ở V1.
- Chỉ dùng cho workflow nghiệp vụ thực tế.

---

## 4. KIẾN TRÚC BỘ NHỚ ĐÃ CHỐT

Knowledge:

- KN_00
- KN_01
- KN_02_ARCH

Working Memory đầu phiên:

- RULE_COMMON
- RULE_ARCH
- WM_03A_ARCH
- WM_04_1_ARCH

Long-term Memory:

- LM_03B_ARCH

Archive:

- LM_04_ARCH

Nguyên tắc:

Không nạp toàn bộ bộ nhớ đầu phiên.

Chỉ nạp những gì cần để vận hành phiên hiện tại.

---

## 5. QUYẾT ĐỊNH VỀ 04

Đã xác nhận.

LM_04_ARCH là archive/history.

LM_04_ARCH không phải Working Memory.

LM_04_ARCH không bắt buộc cập nhật thường xuyên.

LM_04_ARCH không nạp đầu phiên.

Bài học quan trọng sau khi kiểm chứng phải được chắt lọc vào:

- 03A nếu GPT phải luôn nhớ.
- 03B nếu là quyết định dài hạn.
- 04.1 nếu là trạng thái hiện tại.

---

## 6. QUYẾT ĐỊNH VỀ PATCH

Đã xác nhận.

Patch là đơn vị vận chuyển thay đổi, không phải bộ nhớ chính.

Patch có thể dùng để:

- Ghi đề xuất cuối phiên.
- Chia nội dung cập nhật theo đích.
- Hỗ trợ người dùng copy vào file đúng.
- Làm audit tạm thời nếu cần.

Patch không dùng để:

- Lưu tri thức dài hạn.
- Thay thế 03B.
- Thay thế 04.1.
- Tích lũy thành kho tri thức ngày càng lớn.

Sau khi cập nhật Git xong, patch có thể xóa hoặc archive.

---

## 7. QUYẾT ĐỊNH VỀ WORKFLOW

Đã xác nhận.

Không xây thêm workflow chỉ để tối ưu bộ nhớ GPT.

Không ưu tiên WF_CONSOLIDATE_MEMORY_V1.

Không dùng n8n để đọc/sửa repo memory ở V1 nếu GitHub Connector và Codex xử lý được.

Workflow chỉ đáng xây nếu phục vụ công việc thực tế của người dùng.

n8n dành cho:

- CRM.
- Lead.
- Form.
- Email.
- Google Sheet.
- Calendar.
- Telegram.
- Báo cáo.
- Automation nghiệp vụ.

---

## 8. QUYẾT ĐỊNH VỀ CODEX

Đã xác nhận ở mức kiến trúc.

Codex phù hợp để thay phần n8n từng được dùng cho repo memory.

Vai trò Codex:

- Mở repo.
- Sửa file.
- Tạo diff.
- Tạo PR.
- Hỗ trợ review thay đổi.

Codex không quyết định tri thức cuối cùng.

Người dùng vẫn là người duyệt cuối cùng.

GPT Kiến Trúc Sư phân tích và đề xuất.

---

## 9. QUYẾT ĐỊNH VỀ QC

Chỉ dùng:

- PASS
- PASS CÓ LƯU Ý
- FAIL

PASS nghĩa là đủ điều kiện sử dụng.

Nếu đã kết luận PASS thì không đề xuất sửa thêm trong cùng lần QC.

Nếu còn lỗi ảnh hưởng vận hành hoặc kiến trúc thì phải kết luận FAIL.

---

## 10. QUYẾT ĐỊNH VỀ PHÁT TRIỂN FRAMEWORK

Hoàn thiện một GPT mẫu trước.

GPT mẫu hiện tại:

GPT Kiến Trúc Sư.

Thứ tự:

```text
GPT Kiến Trúc Sư V1 đủ dùng
↓
Kiểm thử phiên mới
↓
GPT Content
↓
GPT CRM
↓
GPT khác
```

Không xây GPT hoàn hảo.

Mục tiêu là đủ dùng, dễ nhân bản và tạo giá trị thực tế.

---

## 11. REVIEW KIẾN TRÚC THEO VÒNG ĐỜI

GPT Kiến Trúc Sư phải nhìn vượt yêu cầu trước mắt.

Khi thiết kế hệ thống mới, phải xem:

- Rủi ro triển khai.
- Rủi ro mở rộng.
- Rủi ro dài hạn.
- Chi phí vận hành.
- Khả năng nhân bản.
- Khả năng giảm việc thật cho người dùng.

Nếu một thành phần mới làm hệ thống phức tạp hơn nhưng không giảm việc thực tế, phải cảnh báo.

---

## 12. NGUYÊN TẮC TỐI GIẢN HIỆN TẠI

Đã xác nhận.

Mục tiêu hiện tại không phải mở rộng bộ nhớ.

Mục tiêu hiện tại là đóng gói GPT Kiến Trúc Sư V1 nhanh nhất để chuyển sang GPT Content.

Cảnh báo:

Nếu việc quản trị bộ nhớ ngoài chiếm nhiều công hơn giá trị GPT tạo ra, kiến trúc đang sai.
