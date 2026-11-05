# Kat — cửa hàng ăn vặt

Website tĩnh nhiều trang cho cửa hàng ăn vặt Kat. Khách xem thực đơn, lọc món, tùy chỉnh topping, chọn giao hàng hoặc lấy tại quán, dùng voucher, thanh toán demo, tra cứu đơn và xem lịch sử mua hàng. Khách có thể xem món và giỏ hàng khi chưa đăng nhập; cần đăng nhập để đặt hàng.

## Mở website

Có thể mở `index.html` trực tiếp trong Chrome để xem trang chủ và thực đơn. Nếu trình duyệt chặn bộ nhớ cục bộ khi mở tệp, website dùng dữ liệu dự phòng trong trang hiện tại. Hãy chạy máy chủ cục bộ để lưu và chia sẻ dữ liệu nhất quán giữa các trang:

```powershell
py -m http.server 8000
```

Sau đó mở `http://localhost:8000/`. Dừng máy chủ bằng `Ctrl+C`.

## Các trang

- `index.html` — trang chủ giới thiệu Kat, chọn hình thức nhận món và dẫn tới các trang con; logo Kat luôn quay về đây.
- `menu.html` — 21 nhóm món với 48 lựa chọn giá; tìm theo tên, lọc theo danh mục và khoảng giá, sắp xếp, cuộn xuống để nạp tiếp món. Gà rán và đồ chiên chung một tab. Mỗi ô món mở popup tùy chọn; trên desktop hiển thị sáu món một hàng. Không có footer để tập trung vào món.
- `offers.html` — chín combo cho một người, nhóm bạn hoặc buổi tụ họp; popup cho chọn nước giá đến 15.000đ. Không có footer để tập trung vào combo.
- `stores.html` — danh sách chi nhánh, địa chỉ và giờ mở cửa placeholder.
- `feedback.html` — biểu mẫu góp ý, thông tin liên hệ placeholder và đánh giá khách hàng.
- `cart.html` — giỏ hàng, tùy chỉnh số lượng, giao hàng hoặc lấy tại quán, địa chỉ đã lưu hoặc địa chỉ mới, voucher, tiền mặt khi nhận và QR demo. Người mua đăng nhập trước khi đặt; tài khoản được điền sẵn và sau đăng nhập quay lại giỏ hàng.
- `orders.html` — tra cứu đơn bằng mã đơn và số điện thoại; tài khoản đã đăng nhập có lịch sử mua hàng theo từng đơn.
- `login.html` — trang đăng nhập chung và tạo tài khoản. Sau khi đăng nhập, website quay lại trang đang xem; tài khoản quản trị có thêm mục quản lý cửa hàng trong menu tài khoản. `admin-login.html` là lối vào riêng cho quản trị và mở cùng biểu mẫu đăng nhập.
- `admin.html` — quản lý món, danh mục, combo, đơn hàng, voucher, góp ý, đánh giá và tài khoản; lọc đơn; báo cáo top năm khách hàng theo khoảng ngày.

Trang chủ dùng bố cục ảnh món lớn, thẻ món gợi ý và nội dung tiệm ăn vặt. Thanh điều hướng cố định màu cam có năm mục ở giữa: Thực đơn, Ưu đãi, Đơn hàng, Cửa hàng và Góp ý. Giỏ hàng và tài khoản dùng biểu tượng. Các trang có footer dùng cùng một mẫu; Thực đơn và Ưu đãi không hiện footer.

## Tài khoản demo

- Quản trị: `admin` / `admin123`; số điện thoại `0900000000` — xem [admin-account.txt](admin-account.txt).
- Khách hàng: `khachhang` / `123456`; số điện thoại `0912345678` — xem [customer-account.txt](customer-account.txt).
- Không có nút tự điền tài khoản trên giao diện; đăng nhập bằng số điện thoại hoặc tên đăng nhập tại cùng một trang.

## Dữ liệu và placeholder

Website lưu dữ liệu trong `localStorage` của trình duyệt. Dữ liệu không đồng bộ giữa thiết bị hoặc trình duyệt. Đây là bản demo không có máy chủ, xác thực an toàn, cơ sở dữ liệu dùng chung hay cổng thanh toán. Mật khẩu demo được lưu dưới dạng văn bản; không dùng dữ liệu thật hoặc triển khai cho khách hàng.

Tên chi nhánh, địa chỉ, giờ mở cửa, số điện thoại và email đang là placeholder để chủ quán tự cập nhật. QR chưa kết nối ngân hàng và không tạo giao dịch chuyển khoản. Đơn mới bắt đầu ở trạng thái “Chờ xác nhận”; nút theo dõi mở đúng chi tiết đơn vừa đặt. Ảnh món là ảnh minh họa Pexels; nguồn và tác giả nằm trong [images/SOURCES.md](images/SOURCES.md). Hãy thay bằng ảnh món của Kat trước khi sử dụng thật.

## Hướng thiết kế

Kat dùng bảng màu sáng làm giao diện mặc định duy nhất. Trang chủ đưa lựa chọn giao hàng/lấy tại quán, ưu đãi, thực đơn, chi nhánh và theo dõi đơn vào một luồng rõ ràng. Maika và Popeyes chỉ là tài liệu tham khảo cho cấu trúc trang và cách điều hướng; Kat giữ tên, thông tin cửa hàng, câu chữ và nội dung riêng. Ghi chú nghiên cứu ở `opendesigner/review/REFERENCE-REVIEW.md`.

## Tài liệu dự án

- `DESIGN.md`, `PRODUCT.md`, `opendesigner/` — hệ thống thiết kế, quyết định, nghiên cứu và rà soát.
- `css/`, `js/`, `images/` — giao diện, tương tác và ảnh minh họa.
