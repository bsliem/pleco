# Pleco Text Archive

## Mục đích dự án

Kho lưu trữ này được tạo ra để quản lý, chỉnh sửa, đồng bộ và đọc các file `.txt` — đặc biệt là văn bản tiếng Hoa — giữa nhiều thiết bị Apple, bao gồm:

- MacBook (RStudio / text editor)
- iPhone (nhiều thiết bị khác nhau)
- Working Copy (Git client trên iPhone)
- GitHub (trung tâm đồng bộ)
- Pleco Reader / Clipboard Reader (đọc và tra cứu tiếng Hoa)

---

# Mục tiêu cốt lõi

Pleco hỗ trợ đọc và tra từ rất mạnh đối với văn bản tiếng Hoa, nhưng việc quản lý nhiều file dài (Kinh văn, chú, cổ văn, nghiên cứu, OCR...) trên nhiều thiết bị có thể khó khăn.

Dự án này giải quyết vấn đề đó bằng cách:

## Quy trình:

### Trên MacBook:
- Dùng RStudio hoặc text editor để:
  - OCR cleanup
  - chỉnh sửa nội dung
  - chuẩn hóa encoding UTF-8
  - chia đoạn / thêm phiên âm / xử lý hàng loạt

### Push lên GitHub:
- Lưu trữ trung tâm
- Version control
- Backup
- Đồng bộ nhiều máy

### Trên iPhone:
- Dùng Working Copy để:
  - pull file mới nhất
  - sync giữa nhiều iPhone
  - export / copy sang Pleco Reader

### Trong Pleco:
- Đọc TXT tiếng Hoa
- Clipboard Reader
- Tap tra từ
- Phân tích Hán tự
- Học kinh văn / cổ văn / nghiên cứu

---

# Workflow chuẩn

## MacBook:
```bash
Edit TXT → Commit → Push GitHub