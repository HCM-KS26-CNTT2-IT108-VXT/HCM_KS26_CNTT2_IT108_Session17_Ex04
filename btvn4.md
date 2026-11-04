# BÀI 4: SỰ CỐ XUNG ĐỘT PHIÊN ĐĂNG NHẬP TRÊN TRÌNH DUYỆT

## PHẦN 1. PHÂN TÍCH

### 1. So sánh Incognito Mode và Dedicated Profile

- Incognito Mode: Lưu dữ liệu tạm thời trong phiên duyệt web. Khi đóng cửa sổ, cookie và dữ liệu phiên sẽ bị xóa.
- Dedicated Profile: Lưu dữ liệu lâu dài trên ổ cứng, mỗi Profile có cookie, lịch sử, mật khẩu và Bookmark riêng.

Kết luận: Dedicated Profile phù hợp để quản lý nhiều tài khoản độc lập, hạn chế xung đột phiên đăng nhập.

### 2. Mô hình 3 Profile

- Personal: Sử dụng cho tài khoản cá nhân.
- Work: Sử dụng cho tài khoản quản trị GreenLog.
- Sandbox: Sử dụng cho tài khoản kiểm thử.

## PHẦN 2. TRIỂN KHAI

### 1. Tạo 3 Profile

Mở Chrome, chọn biểu tượng Profile → Add Chrome Profile. Tạo lần lượt Personal, Work và Sandbox với màu sắc khác nhau để dễ nhận biết.

### 2. Tổ chức Bookmark

Tạo cấu trúc thư mục:

- PERSONAL
  - Social Media
  - Email cá nhân
  - Giải trí
- WORK
  - Development: GitHub
  - Learning: Canvas LMS
  - Company: GreenLog Portal
- SANDBOX
  - Test Website
  - Demo Accounts

### 3. Thiết lập Cloud Sync

- Đăng nhập tài khoản Google vào từng Profile.
- Truy cập Settings → Sync and Google services.
- Bật đồng bộ hóa Bookmarks.
- Khi đổi máy tính, đăng nhập lại tài khoản Google và bật Sync để khôi phục Bookmark.

## PHẦN 3. KIỂM THỬ

### 1. Quy tắc sử dụng Guest Profile

- Chọn Profile → Guest để mở chế độ khách.
- Không lưu mật khẩu và thông tin cá nhân.
- Không sử dụng tài khoản cá nhân trên máy tính công cộng.
- Đóng toàn bộ cửa sổ Guest sau khi sử dụng.

### 2. Kết quả kiểm thử

- Ba Profile hoạt động độc lập, không dùng chung cookie và phiên đăng nhập.
- Bookmark được tổ chức theo từng mục đích sử dụng.
- Cloud Sync giúp bảo vệ và khôi phục Bookmark khi đổi máy tính.
- Guest Profile giúp hạn chế lưu lại thông tin cá nhân trên máy tính công cộng.

### 3. Đảm bảo an toàn

Khi trình chiếu bằng Profile Work, mật khẩu và lịch sử duyệt web của Profile Personal không hiển thị trong Profile Work do dữ liệu được lưu trữ riêng biệt.

**KẾT LUẬN:** Sử dụng nhiều Chrome Profile giúp quản lý tài khoản khoa học, hạn chế xung đột phiên đăng nhập và bảo vệ dữ liệu cá nhân.