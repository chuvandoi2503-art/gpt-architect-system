# MEMORY_INDEX

Phiên bản: 04.000

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

Memory Index là bản đồ định vị Runtime của GPT KIẾN TRÚC SƯ.

GPT phải đọc file này trước khi truy cập Runtime Repository.

Memory Index dùng để:

- Định vị Core.
- Định vị Runtime.
- Định vị Memory.
- Định vị Knowledge.
- Xác định Load Strategy.

Không tự suy đoán path.

Không sử dụng Memory hội thoại làm nguồn chân lý.

---

# CORE REPOSITORY

Repository:

gpt-system-core

## 00 - HIẾN PHÁP GPT

Path:

CORE/00 - HIẾN PHÁP GPT.md

---

## 01 - QUY TẮC VẬN HÀNH

Path:

CORE/01 - QUY TẮC VẬN HÀNH.md

---

## 02 - TIÊU CHUẨN PHÂN TÁCH TRÁCH NHIỆM

Path:

CORE/02 - TIÊU CHUẨN PHÂN TÁCH TRÁCH NHIỆM.md

---

## 03 - TIÊU CHUẨN HỒ SƠ

Path:

CORE/03 - TIÊU CHUẨN HỒ SƠ.md

---

## 04 - TIÊU CHUẨN PATCH

Path:

CORE/04 - TIÊU CHUẨN PATCH.md

---

## 05 - NGUYÊN TẮC KIẾN TRÚC

Path:

CORE/05 - NGUYÊN TẮC KIẾN TRÚC.md

---

# SYSTEM (CORE)

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

Mô tả:

Hồ sơ lĩnh vực của GPT KIẾN TRÚC SƯ.

Trạng thái:

LOAD_ON_DEMAND

---

# WORKING MEMORY

## WM_03A_ARCH

Path:

memory/WM_03A/WM_03A_ARCH - BỘ NHỚ LÕI GPT KIẾN TRÚC SƯ.md

---

## WM_04_1_ARCH_DAILY

Path:

memory/WM_04_1/WM_04_1_ARCH_DAILY - VIỆC ĐANG DỞ HÔM NAY GPT KIẾN TRÚC SƯ.md

---

## WM_04_1_ARCH_LONG

Path:

memory/WM_04_1/WM_04_1_ARCH_LONG - VIỆC ĐANG DỞ DÀI HẠN GPT KIẾN TRÚC SƯ.md

---

# LONG TERM MEMORY

## LM_03B_ARCH_CURRENT

Path:

memory/LM_03B/LM_03B_ARCH_CURRENT - TRI THỨC ĐÃ KIỂM CHỨNG GPT KIẾN TRÚC SƯ.md

---

## LM_03B_ARCH_ARCHIVE_001

Path:

memory/LM_03B/LM_03B_ARCH_ARCHIVE_001 - TRI THỨC LƯU TRỮ GPT KIẾN TRÚC SƯ.md

---

## LM_04_ARCH_CURRENT

Path:

memory/LM_04/LM_04_ARCH_CURRENT - NHẬT KÝ HỌC TẬP GPT KIẾN TRÚC SƯ.md

---

## LM_04_ARCH_ARCHIVE_2026_06

Path:

memory/LM_04/LM_04_ARCH_ARCHIVE_2026_06 - NHẬT KÝ LƯU TRỮ GPT KIẾN TRÚC SƯ.md

---

# SYSTEM (RUNTIME)

## GPT_BUILDER_BACKUP

Repository:

gpt-architect-system

Path:

SYSTEM/GPT_BUILDER_BACKUP.md

---

# KNOWLEDGE UPLOAD STANDARD

GPT KIẾN TRÚC SƯ phải tải mặc định:

- CORE/00 - HIẾN PHÁP GPT.md
- CORE/01 - QUY TẮC VẬN HÀNH.md
- CORE/02 - TIÊU CHUẨN PHÂN TÁCH TRÁCH NHIỆM.md
- CORE/05 - NGUYÊN TẮC KIẾN TRÚC.md

---

# KHỞI TẠO PHIÊN MẶC ĐỊNH

## BƯỚC 1

Đọc:

- CORE/03 - TIÊU CHUẨN HỒ SƠ.md
- CORE/04 - TIÊU CHUẨN PATCH.md

Repository:

gpt-system-core

---

## BƯỚC 2

Đọc Runtime:

- RULE_ARCH
- WM_03A_ARCH
- WM_04_1_ARCH_DAILY
- LM_03B_ARCH_CURRENT

---

# LOAD ON DEMAND

Chỉ đọc khi cần:

- KN_02_ARCH
- WM_04_1_ARCH_LONG
- LM_03B_ARCH_ARCHIVE
- LM_04_ARCH_CURRENT
- LM_04_ARCH_ARCHIVE

- MEMORY_ARCHITECTURE
- PATCH_STANDARD
- GITHUB_WRITE_POLICY
- NAMING_CONVENTION

- GPT_BUILDER_BACKUP

---

# LOAD STRATEGY

AUTO LOAD:

- CORE/00
- CORE/01
- CORE/02
- CORE/05

---

SESSION LOAD:

- CORE/03
- CORE/04

- RULE_ARCH
- WM_03A_ARCH
- WM_04_1_ARCH_DAILY
- LM_03B_ARCH_CURRENT

---

LOAD ON DEMAND:

- KNOWLEDGE
- LONG MEMORY
- SYSTEM
- ARCHIVE

---

# TRẠNG THÁI SAU KHỞI TẠO

GPT KIẾN TRÚC SƯ phải biết:

- Vai trò hiện tại.
- Kiến trúc đang triển khai.
- Công việc đang dở.
- Tri thức đã kiểm chứng.
- Trạng thái phiên.

---

# NGUYÊN TẮC CUỐI CÙNG

Memory Index là bản đồ của Runtime Repository.

GPT KIẾN TRÚC SƯ không được nạp toàn bộ Repository khi khởi tạo phiên.

Chỉ nạp tối thiểu để bắt đầu vận hành.

Mọi quyết định kiến trúc phải tuân thủ:

- Thực tế > Lý thuyết.
- Vận hành được > Kiến trúc đẹp.
- Kiến trúc đi trước thực tế tối đa 1–2 bước.
- Nếu ngày mai không dùng thì hôm nay không xây.
