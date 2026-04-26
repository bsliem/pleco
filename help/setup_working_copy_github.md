# ÔN LẠI TOÀN BỘ WORKFLOW SETUP VỪA RỒI

## Biến iPhone + Working Copy thành máy GitHub di động

------

# PHẦN I — MỤC TIÊU

## Bạn muốn:

### iPhone → Working Copy → GitHub → Push file TXT / OCR / Pleco / Kinh văn

------

# PHẦN II — CÁC BƯỚC ĐÃ LÀM

# BƯỚC 1: Cài Working Copy

## App Store:

### Working Copy

------

# BƯỚC 2: Kết nối GitHub

## Working Copy:

```
Settings → Hosting Providers → GitHub
```

------

# BƯỚC 3: Authentication

## Ban đầu lỗi:

```
No way to authenticate with github.com
```

------

## Cách sửa:

### Trong GitHub Provider:

- OAuth Authentication → ON
- Enable Provider → ON
- Test

------

# BƯỚC 4: SSH Key

## Working Copy tự tạo SSH key:

```
WorkingCopy@iPhone-26042026
```

------

## GitHub:

SSH key được add vào account thành công qua email xác nhận.

------

# BƯỚC 5: SSH Transfers

## Đặt:

```
SSH Transfers → Always
```

------

# Ý nghĩa:

## Từ nay dùng:

```
git@github.com:...
```

## Thay vì:

```
https://github.com/...
```

### SSH ổn định hơn, không cần nhập password/token liên tục.

------

# BƯỚC 6: Tạo repo GitHub

## Repo:

```
pleco
```

------

# BƯỚC 7: Lấy SSH remote

## GitHub:

```
Code → SSH
```

### URL:

```
git@github.com:bsliem/pleco.git
```

------

# BƯỚC 8: Working Copy remote origin

```
Repository Settings → Remotes → origin
```

### Dán:

```
git@github.com:bsliem/pleco.git
```

------

# BƯỚC 9: Commit + Push

## Trong Working Copy:

### Tick file:

```
leng yan zhou full.txt
```

### Commit message:

```
leng yan zhou iphone
```

### Push:

ON

### Commit

------

# KẾT QUẢ:

## Push thành công lên:

```
github.com/bsliem/pleco
```

------

# PHẦN III — WORKFLOW HẰNG NGÀY

# Khi muốn upload file mới:

## 1.

```
Open repo in Working Copy
```

## 2.

```
Add / Edit / Import file
```

## 3.

```
Commit message
```

## 4.

```
Push ON
```

## 5.

```
Commit
```

------

# PHẦN IV — CẤU TRÚC TỐI ƯU GỢI Ý

```
pleco/
 ├── leng_yan_zhou/
 ├── kim_cang/
 ├── phap_hoa/
 ├── hebrew/
 ├── cna_d/
 └── papers/
```

------

# PHẦN V — README NÊN THÊM

```
# Pleco Text Archive

Kho văn bản dùng cho:
- Pleco Clipboard Reader
- OCR iPhone
- TXT backup
- Kinh văn
- Hebrew
- Research notes
```

------

# PHẦN VI — NẾU DÙNG TRÊN iSH

## Clone:

```
git clone git@github.com:bsliem/pleco.git
```

------

# PHẦN VII — MẸO QUAN TRỌNG

# HTTPS:

```
Hay lỗi auth
```

# SSH:

```
Ổn định, lâu dài
```

------

# PHẦN VIII — COMMIT STYLE KHUYÊN DÙNG

```
2026-04-26 | iphone | pleco | add leng yan zhou
```

------

# TÓM TẮT SIÊU NGẮN:

## SETUP:

```
Working Copy
→ Hosting Providers
→ GitHub
→ Test
→ SSH Key
→ SSH Always
→ Repo
→ origin = git@github.com...
```

------

## DAILY:

```
Import
→ Commit
→ Push
```

------

# THÀNH TỰU:

## Bạn đã setup xong:

### Mobile OCR → TXT → Git → Backup → Cross-device sync

## Nói thật:

Đây là setup rất mạnh cho:

### Pleco + Kinh văn + Nghiên cứu + iSH + GitHub archive.