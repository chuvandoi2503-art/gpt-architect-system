# PATCH_ARCH_LM_03B_ARCH_20260618_001 - NGUYÊN TẮC REGISTRY VÀ AUTOMATION SAFETY

## PATCH METADATA

PATCH_ID: PATCH_ARCH_LM_03B_ARCH_20260618_001
PATCH_STATUS: DRAFT
GPT_ID: ARCH
TARGET_ID: LM_03B_ARCH
ACTION: APPEND_ONLY
CONFIDENCE: ĐÃ_XÁC_NHẬN
CREATED_BY: GPT_ARCH
PURPOSE: Ghi nhận nguyên tắc Registry Driven Workflow và Automation Safety First vào bộ nhớ dài hạn đã xác nhận.

---

## NGUYÊN TẮC REGISTRY DRIVEN WORKFLOW

Đã xác nhận.

Workflow không nên hardcode:

- GPT_ID.
- TARGET_ID.
- File path.
- Mapping giữa target và file GitHub.

Thay vào đó, hệ thống sử dụng Registry chung.

Registry hiện tại:

```text
system/GPT_REGISTRY.json
