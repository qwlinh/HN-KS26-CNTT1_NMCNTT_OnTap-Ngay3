# BÀI LÀM – THI THỬ HACKATHON 01

- **Mã đề:** Thi thử
- **Họ tên:** Vũ Quốc Linh
- **Lớp:** CNTT1
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):** Wíndown

## 4.2. Thao tác máy tính cơ bản bằng CLI 

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng
pwd
ls -force
mv nhap_hang.txt docs
mv logo_van_phong_pham.PNG media
cp media/logo_van_phong_pham.PNG backup
rm temp_131.tmp
ls
cd logs
ls
cd ..
```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
    Directory: C:\Users\linhs\Downloads\starter-kit(4)\van-phong-pham-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/23/2026   9:14 AM                backup
d-----        10/23/2026   9:10 AM                data
d-----        10/23/2026   9:13 AM                docs
d-----        10/23/2026   9:10 AM                logs
d-----        10/23/2026   9:13 AM                media
-a----        10/19/2026   9:41 AM             78 .env
-a----        10/19/2026  10:00 AM           2253 bai_lam.md


    Directory: C:\Users\linhs\Downloads\starter-kit(4)\van-phong-pham-website\backup


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           6053 logo_van_phong_pham.PNG


    Directory: C:\Users\linhs\Downloads\starter-kit(4)\van-phong-pham-website\data


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           6105 don_ban _thang_10.xlsx


    Directory: C:\Users\linhs\Downloads\starter-kit(4)\van-phong-pham-website\docs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM             51 nhap_hang.txt


    Directory: C:\Users\linhs\Downloads\starter-kit(4)\van-phong-pham-website\logs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           1053 shop.log


    Directory: C:\Users\linhs\Downloads\starter-kit(4)\van-phong-pham-website\media


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           6053 logo_van_phong_pham.PNG


```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
Get-Content .\logs\shop.log | Select-String "ERROR" > .\logs\daily_report.txt

Get-Content .\logs\daily_report.txt
```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
2025-10-28 08:24:28 [ERROR] Thanh toan bi tu choi
```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [x] Heading 1: tên dự án
- [x] Mô tả ngắn có cả **in đậm** và *in nghiêng*
- [x] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [x] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
- [x] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [x] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
Get-Content .\logs\shop.log | Select-String "ERROR" | Measure-Object -Line

(Select-String -Path .\logs\shop.log -Pattern "ERROR").Count
```

### Nội dung file logs/auto_report.txt

```text


```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
# Ghi lệnh vào đây (xoá dòng này)

```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng (xoá dòng này)

```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.8. Excel

> Phần Excel được chấm trực tiếp trên file `data/don_ban_thang_10.xlsx`, không cần ghi vào đây.
