# InternalRequest_Management-tichhopAI
Hệ thống phê duyệt đề nghị nội bộ
# Hệ thống phê duyệt đề nghị nội bộ (ASP.NET Core MVC)


## Yêu cầu

- Visual Studio 2022 (workload ASP.NET) hoặc .NET 8 SDK

- SQL Server Express hoặc LocalDB


## Chạy thử

1. Clone repo, mở file .sln bằng Visual Studio.

2. Chuột phải project -> Manage User Secrets, dán:

{

"ConnectionStrings": { "DefaultConnection": "Server=.\\SQLEXPRESS;Database=QuanLyPheDuyetDeNghiDb;Trusted_Connection=True;TrustServerCertificate=True" },

"Gemini": { "ApiKey": "<khóa Gemini của bạn, có thể bỏ trống>" }

}

3. Nhấn F5. Database và dữ liệu mẫu tự tạo ở lần chạy đầu.


## Tài khoản demo (mật khẩu: 123)

admin | giamdoc | truongphong | nhanvien | nhanvien2


## Ghi chú

- Không có khóa Gemini thì 3 tính năng AI báo "chưa cấu hình", các chức năng khác vẫn chạy.

- Nếu AI báo "không tìm thấy mô hình", đổi Gemini:Model trong appsettings.json theo tên mô hình hiện hành trong Google AI Studio.
