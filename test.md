Test Case Xác thực người dùng
| ID Test Case | Chức năng | Vai trò | Tiền điều kiện | Bước thực hiện | Dữ liệu đầu vào | Kết quả mong đợi |
|-------------|-----------|----------|----------------|----------------|-----------------|------------------|
| ID_01 | Đăng ký | Người dùng | Người dùng chưa có tài khoản | 1. Mở trang Đăng ký<br>2. Nhập email hợp lệ<br>3. Nhập mật khẩu hợp lệ<br>4. Nhập họ tên<br>5. Nhập số điện thoại<br>6. Nhấn nút 'Đăng ký' | Email: user@example.com<br>Password: Test@123<br>Họ tên: Nguyễn Văn A<br>SĐT: 0123456789 | - Đăng ký thành công<br>- Chuyển đến trang Đăng nhập<br>- Hiển thị thông báo thành công |
| ID_02 | Đăng nhập | Người dùng | Đã có tài khoản | 1. Mở trang Đăng nhập<br>2. Nhập email<br>3. Nhập mật khẩu<br>4. Nhấn nút 'Đăng nhập' | Email: user@example.com<br>Password: Test@123 | - Đăng nhập thành công<br>- Chuyển đến trang chủ<br>- Hiển thị thông tin người dùng |
| ID_03 | Đặt tour | Khách hàng | Đã đăng nhập | 1. Chọn tour<br>2. Nhập thông tin đặt tour<br>3. Xác nhận đặt tour | - Số người lớn: 2<br>- Số trẻ em: 1<br>- Ngày đi: 2024-03-20 | - Đặt tour thành công<br>- Hiển thị thông tin đặt tour<br>- Gửi email xác nhận |
| ID_04 | Quản lý tour | Admin | Đăng nhập với quyền admin | 1. Vào trang quản lý<br>2. Thêm tour mới<br>3. Nhập thông tin tour | - Tên tour: Tour Đà Lạt<br>- Giá: 2,000,000<br>- Số lượng: 20<br>- Hình ảnh: 3 ảnh | - Tour được thêm thành công<br>- Hiển thị trong danh sách<br>- Upload ảnh thành công |
| ID_05 | Thanh toán | Khách hàng | Đã đặt tour | 1. Chọn phương thức<br>2. Nhập thông tin<br>3. Xác nhận thanh toán | - Số tiền: 5,000,000<br>- Phương thức: VNPAY<br>- Thông tin thẻ | - Thanh toán thành công<br>- Cập nhật trạng thái đơn<br>- Gửi email xác nhận |
Test Case Quản lý Tour
| ID Test Case | Chức năng | Vai trò | Tiền điều kiện | Bước thực hiện | Dữ liệu đầu vào | Kết quả mong đợi |
|-------------|-----------|----------|----------------|----------------|-----------------|------------------|
| ID_06 | Thêm tour | Admin | Đăng nhập admin | 1. Vào mục Quản lý tour<br>2. Click "Thêm mới"<br>3. Nhập thông tin<br>4. Upload ảnh<br>5. Lưu | - Tên: Tour Hạ Long<br>- Giá: 3,000,000<br>- Lịch trình: 3N2Đ<br>- Ảnh: 4 ảnh | - Tour mới được tạo<br>- Ảnh được lưu trữ<br>- Hiển thị trong list |
| ID_07 | Sửa tour | Admin | Tour đã tồn tại | 1. Chọn tour cần sửa<br>2. Cập nhật thông tin<br>3. Lưu thay đổi | - Giá mới: 3,500,000<br>- Thêm ảnh mới<br>- Cập nhật mô tả | - Thông tin được cập nhật<br>- Hiển thị thông báo<br>- Refresh danh sách |
Test Case Quản lý Đặt Tour
| ID Test Case | Chức năng | Vai trò | Tiền điều kiện | Bước thực hiện | Dữ liệu đầu vào | Kết quả mong đợi |
|-------------|-----------|----------|----------------|----------------|-----------------|------------------|
| ID_08 | Xác nhận đặt tour | Admin | Có đơn đặt mới | 1. Xem chi tiết đơn<br>2. Kiểm tra thông tin<br>3. Xác nhận đơn | - Mã đơn: DT001<br>- Thông tin KH<br>- Số tiền: 6,000,000 | - Đơn được xác nhận<br>- Email thông báo<br>- Cập nhật slot tour |
| ID_09 | Hủy đơn | Admin | Đơn chưa thanh toán | 1. Chọn đơn hủy<br>2. Nhập lý do<br>3. Xác nhận hủy | - Mã đơn: DT002<br>- Lý do: "Quá hạn"<br>- Ghi chú admin | - Đơn chuyển trạng thái<br>- Thông báo khách<br>- Cập nhật số lượng |
