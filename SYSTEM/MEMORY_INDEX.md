# MEMORY_INDEX

Phiên bản: 03.001

---

# REPOSITORY

Owner:

chuvandoi2503-art

Runtime Repository:

gpt-architect-system

Core Repository:

gpt-system-core

---

# MỤC ĐÍCH

Memory Index là bản đồ định vị memory của GPT KIẾN TRÚC SƯ.

GPT phải đọc file này trước khi truy cập memory runtime.

Không tự suy đoán path.

Không dùng memory hội thoại làm nguồn chân lý.

---

# CORE REPOSITORY

## RULE_COMMON

Repository:

gpt-system-core

Path:

rules/RULE_COMMON - QUY TẮC CHUNG TOÀN HỆ GPT.md

---

## MEMORY_ARCHITECTURE

Repository:

gpt-system-core

Path:

SYSTEM/MEMORY_ARCHITECTURE.md

---

## PATCH_STANDARD

Repository:

gpt-system-core

Path:

SYSTEM/PATCH_STANDARD.md

---

## GITHUB_WRITE_POLICY

Repository:

gpt-system-core

Path:

SYSTEM/GITHUB_WRITE_POLICY.md

---

## NAMING_CONVENTION

Repository:

gpt-system-core

Path:

SYSTEM/NAMING_CONVENTION.md

---

# RUNTIME RULE

## RULE_ARCH

Repository:

gpt-architect-system

Path:

rules/RULE_ARCH - ÁP DỤNG BẮT BUỘC GPT KIẾN TRÚC SƯ.md

---

# KNOWLEDGE

## KN_02_ARCH

Repository:

gpt-architect-system

Path:

knowledge/KN_02_ARCH - HỒ SƠ LĨNH VỰC GPT KIẾN TRÚC SƯ.md

---

# WORKING MEMORY

## WM_03A_ARCH

Repository:

gpt-architect-system

Path:

memory/WM_03A/WM_03A_ARCH - BỘ NHỚ LÕI GPT KIẾN TRÚC SƯ.md

---

## WM_04_1_ARCH_DAILY

Repository:

gpt-architect-system

Path:

memory/WM_04_1/WM_04_1_ARCH_DAILY - VIỆC ĐANG DỞ HÔM NAY GPT KIẾN TRÚC SƯ.md

---

## WM_04_1_ARCH_LONG

Repository:

gpt-architect-system

Path:

memory/WM_04_1/WM_04_1_ARCH_LONG - VIỆC ĐANG DỞ DÀI HẠN GPT KIẾN TRÚC SƯ.md

---

# LONG TERM MEMORY

## LM_03B_ARCH_CURRENT

Repository:

gpt-architect-system

Path:

memory/LM_03B/LM_03B_ARCH_CURRENT - TRI THỨC ĐÃ KIỂM CHỨNG GPT KIẾN TRÚC SƯ.md

---

## LM_03B_ARCH_ARCHIVE_001

Repository:

gpt-architect-system

Path:

memory/LM_03B/LM_03B_ARCH_ARCHIVE_001 - TRI THỨC LƯU TRỮ GPT KIẾN TRÚC SƯ.md

---

## LM_04_ARCH_CURRENT

Repository:

gpt-architect-system

Path:

memory/LM_04/LM_04_ARCH_CURRENT - NHẬT KÝ HỌC TẬP GPT KIẾN TRÚC SƯ.md

---

## LM_04_ARCH_ARCHIVE_2026_06

Repository:

gpt-architect-system

Path:

memory/LM_04/LM_04_ARCH_ARCHIVE_2026_06 - NHẬT KÝ LƯU TRỮ GPT KIẾN TRÚC SƯ.md

---

# SYSTEM

## GPT_BUILDER_BACKUP

Repository:

gpt-architect-system

Path:

SYSTEM/GPT_BUILDER_BACKUP.md

---

# KHỞI TẠO PHIÊN MẶC ĐỊNH

Khi khởi tạo phiên, nạp:

- RULE_COMMON
- RULE_ARCH
- WM_03A_ARCH
- WM_04_1_ARCH_DAILY
- LM_03B_ARCH_CURRENT

Không nạp mặc định:

- KN_02_ARCH
- WM_04_1_ARCH_LONG
- LM_03B_ARCH_ARCHIVE
- LM_04_ARCH_CURRENT
- LM_04_ARCH_ARCHIVE

Chỉ đọc khi cần.
