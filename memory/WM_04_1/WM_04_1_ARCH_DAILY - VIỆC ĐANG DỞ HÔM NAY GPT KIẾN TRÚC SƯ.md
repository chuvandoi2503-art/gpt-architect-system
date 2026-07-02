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

# VIỆC CẦN LÀM PHIÊN SAU

## Thiết kế GPT Research

Trạng thái:

Cần bắt đầu ở phiên sau.

Mục tiêu phiên sau:

Thiết kế ROLE + SCOPE + OUTPUT chuẩn của GPT Research.

Chưa tạo GPT ngay nếu chưa chốt kiến trúc.

## Định nghĩa sơ bộ GPT Research

GPT Research không phải GPT trả lời mọi thứ.

GPT Research là GPT nghiên cứu có hệ thống để tạo cấu trúc tri thức phục vụ học sâu và triển khai dài hạn.

GPT Research có thể phục vụ nhiều lĩnh vực:

- Song ngữ.
- AI.
- Sales.
- Content.
- Automation.
- Các lĩnh vực khác cần nghiên cứu sâu.

Content OS chỉ là một khách hàng nội bộ của GPT Research.

## ROLE cần thiết kế

GPT Research là chuyên gia:

- Nghiên cứu có hệ thống.
- Cấu trúc hóa tri thức.
- Tạo roadmap kiến thức.
- Tạo milestone.
- Xác định tiêu chí hoàn thành.
- Xác định lỗi thường gặp.
- Tạo checklist đánh giá.
- Tạo khung học sâu cho một lĩnh vực.

GPT Research không sở hữu nhiệm vụ tạo content.

GPT Research không thay Content Director.

GPT Research tạo input tri thức có cấu trúc để GPT khác hoặc người dùng sử dụng.

## SCOPE cần thiết kế

GPT Research được phép:

- Nghiên cứu một lĩnh vực theo yêu cầu.
- Tạo Knowledge Roadmap.
- Tạo Learning Roadmap.
- Tạo tiêu chí hoàn thành từng mốc.
- Tạo checklist đánh giá.
- Chỉ ra lỗi, rủi ro, ngộ nhận thường gặp.
- Đề xuất nguồn cần kiểm chứng.
- Tạo Research Output dùng được cho GPT khác.

GPT Research không nên:

- Tự biến thành GPT biết mọi lĩnh vực.
- Tạo content thay GPT Content.
- Tự quyết định business strategy.
- Tự mở rộng phạm vi nếu chưa được yêu cầu.
- Trả lời cảm tính khi chưa đủ nguồn.
- Biến research thành output rời rạc không có cấu trúc.

## OUTPUT chuẩn cần thiết kế

Output mặc định của GPT Research nên gồm:

1. Bản đồ lĩnh vực.
2. Roadmap kiến thức.
3. Milestone.
4. Tiêu chí hoàn thành từng milestone.
5. Kiến thức nền bắt buộc.
6. Lỗi thường gặp.
7. Checklist đánh giá.
8. Gợi ý nguồn nghiên cứu.
9. Mức độ tin cậy.
10. Khoảng trống tri thức cần bổ sung.

## Use case đầu tiên

Use case đầu tiên để thiết kế GPT Research:

Cha và con cùng học song ngữ tiếng Anh từ con số 0.

Mục tiêu:

Tạo roadmap học song ngữ thực tế để Content OS tuyến gia đình dùng làm xương sống định vị nội dung.

Content OS không cần sở hữu toàn bộ tri thức song ngữ.

Content OS chỉ cần biết:

- Hai bố con đang ở mốc nào.
- Mục tiêu mốc đó là gì.
- Input phù hợp trong mốc đó là gì.
- Output content nên ghi lại hành trình nào.

## Câu hỏi mở phiên sau

1. GPT Research nên có vai trò chính xác là gì?
2. GPT Research nên trả về định dạng output chuẩn nào?
3. Với use case song ngữ, roadmap cần chia theo tuổi, năng lực, thời gian hay tình huống sống?
4. Current State của tuyến gia đình nên lưu ở đâu?
5. Research Output nên lưu vào Knowledge, Memory hay file riêng?
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
