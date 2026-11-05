# Kat — website đặt món ăn vặt

Kat là website nhiều trang cho một quán ăn vặt nhỏ. Khách có thể xem món, chọn loại và giá, đặt giao hàng hoặc đến lấy tại quán, rồi theo dõi đơn. Giao diện được xây bằng HTML, CSS và JavaScript thuần; không cần cài thư viện hay chạy bước build.

## Chạy website

Mở PowerShell tại thư mục dự án và chạy máy chủ tĩnh:

    py -m http.server 8000

Mở http://localhost:8000 trong Chrome. Dừng máy chủ bằng Ctrl+C.

## Các trang

- Trang chủ (index.html): giới thiệu Kat, món nổi bật và đường dẫn tới các phần chính.
- Thực đơn (menu.html): tìm món, lọc danh mục và giá, sắp xếp, cuộn để tải thêm. Bấm vào thẻ món để mở popup chọn loại, khẩu vị và topping.
- Ưu đãi hôm nay (offers.html): xem và đặt các combo; chọn thức uống đi kèm hoặc bỏ nước nếu combo hỗ trợ.
- Cửa hàng (stores.html): xem địa chỉ và giờ mở cửa của hai cơ sở.
- Giỏ hàng (cart.html): cập nhật số lượng, chọn giao hàng hoặc lấy tại quán, áp dụng voucher và đặt hàng.
- Theo dõi đơn hàng (orders.html): tra cứu bằng mã đơn và số điện thoại hoặc xem lịch sử sau khi đăng nhập.
- Góp ý (feedback.html): gửi phản hồi về món ăn và dịch vụ.
- Đăng nhập (login.html): khách đăng nhập hoặc tạo tài khoản bằng số điện thoại.
- Đăng nhập quản trị (admin-login.html) và quản lý cửa hàng (admin.html): quản lý thực đơn, danh mục, đơn hàng, combo, voucher, đánh giá, góp ý và tài khoản.

## Thêm món và lựa chọn trong quản trị

Trong form món ăn:

- Giá bán hoặc giá thấp nhất là giá của món không có lựa chọn. Khi món có lựa chọn, hệ thống lấy giá thấp nhất trong các lựa chọn.
- Giá gốc là giá tham khảo hiển thị gạch ngang; để trống hoặc nhập 0 nếu không áp dụng.
- Lựa chọn và giá có một dòng cho mỗi lựa chọn theo mẫu Tên lựa chọn | giá bằng đồng. Ví dụ:

      Mẹt viên chiên nhỏ | 35000
      Mẹt viên chiên lớn | 55000

  Khách chọn một loại trong popup và giá được tính theo loại đó.
- Có thể tải ảnh chính cho món và ảnh riêng cho từng lựa chọn. Nếu lựa chọn không có ảnh riêng, popup dùng ảnh chính của món.

## Cơ sở

- Cơ sở chính: 273 An Dương Vương, Phường Chợ Quán (Quận 5 cũ), TP. HCM.
- Cơ sở 1: 105 Bà Huyện Thanh Quan, Phường Xuân Hòa (Quận 3 cũ), TP. HCM.
- Cả hai cơ sở mở cửa từ 8:00 đến 18:00.

## Lưu ý về dữ liệu

Website lưu tài khoản, thực đơn, giỏ hàng và đơn trong bộ nhớ cục bộ của trình duyệt. Dữ liệu không tự đồng bộ giữa thiết bị hoặc trình duyệt. Đây là bản demo, chưa có máy chủ, cơ sở dữ liệu dùng chung, xác thực an toàn hay cổng thanh toán thật. Hình thức QR chỉ minh họa quy trình; không tạo giao dịch ngân hàng.

Số điện thoại, email và liên kết mạng xã hội đang là thông tin mẫu.