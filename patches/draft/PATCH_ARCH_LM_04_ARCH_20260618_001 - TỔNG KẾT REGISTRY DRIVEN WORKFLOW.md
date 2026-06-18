# PATCH_ARCH_LM_04_ARCH_20260618_001 - TỔNG KẾT REGISTRY DRIVEN WORKFLOW

## PATCH METADATA

PATCH_ID: PATCH_ARCH_LM_04_ARCH_20260618_001
PATCH_STATUS: DRAFT
GPT_ID: ARCH
TARGET_ID: LM_04_ARCH
ACTION: APPEND_ONLY
CONFIDENCE: ĐÃ_XÁC_NHẬN
CREATED_BY: GPT_ARCH
PURPOSE: Ghi nhận kết quả refactor WF_PATCH_V1 và WF_MERGE_PATCH_V1 sang Registry Driven.

---

## BÀI HỌC MỚI - REGISTRY DRIVEN WORKFLOW

Quan sát:

Trong quá trình mở rộng workflow từ một GPT sang nhiều GPT, đã phát hiện nếu hardcode GPT_ID, TARGET_ID và file path trong từng workflow thì hệ thống sẽ nhanh chóng trở nên cồng kềnh.

Nếu mỗi GPT cần một bộ workflow riêng, 10 GPT có thể tạo thành 40 workflow hoặc nhiều hơn.

Kết luận:

Không nên nhân bản workflow theo từng GPT.

Nên dùng workflow chung và điều hướng bằng Registry.

Đã tạo file Registry chung:

```text
system/GPT_REGISTRY.json
