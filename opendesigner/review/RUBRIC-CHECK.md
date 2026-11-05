# Biên bản đánh giá Web 1 — rà theo tiêu chí

Rà soát theo file `BienBanDanhGia_Web1_2025-caoth.doc` ngày 2026-11-05. Phần điểm dưới đây là chấm theo mã nguồn và tiêu chí nhìn thấy trong biên bản. Giao diện laptop/desktop trên Chrome chưa được chấm trực tiếp; bạn sẽ kiểm tra lần cuối.

## Điểm tạm theo tiêu chí nhìn thấy

| Nhóm | Điểm | Căn cứ |
|---|---:|---|
| Chức năng người mua | 12/12 mục | Các mục trong checklist đều có trong mã nguồn. |
| Chức năng quản trị | 8/8 mục | Các mục trong checklist đều có trong mã nguồn, gồm lọc đơn cập nhật trực tiếp. |
| **Tổng điểm phần tiêu chí nhìn thấy** | **10/10 điểm** | Biên bản ghi tổng 12 điểm nhưng nội dung trích xuất chỉ phân bổ được 10; 2 điểm còn lại chưa có tiêu chí để chấm. |

Điểm này xác nhận mức độ hoàn thành chức năng trong mã nguồn, không thay cho điểm của giảng viên hoặc phần chấm giao diện trực tiếp trên Chrome.

## Chức năng người mua

| Tiêu chí | Trạng thái | Bằng chứng |
|---|---|---|
| Hiển thị món theo danh mục | Đạt trong mã nguồn | `menu.html`, `js/main.js`, `js/initdata.js` |
| Xem chi tiết món | Đạt trong mã nguồn | Popup món có lựa chọn, giá từng loại, topping và khẩu vị trong `js/main.js` |
| Tìm tên món tương đối | Đạt trong mã nguồn | So khớp chuỗi con không phân biệt hoa thường trong `js/main.js` |
| Tìm nâng cao đồng thời theo tên, danh mục và khoảng giá | Đạt trong mã nguồn | Bộ lọc kết hợp ở `getVisibleProducts()` trong `js/main.js` |
| Nạp tiếp kết quả khi cuộn | Đạt trong mã nguồn | Lọc và sắp xếp trước khi nạp từng nhóm 8 món bằng `IntersectionObserver` trong `js/main.js` |
| Đăng ký tài khoản mua hàng | Đạt trong mã nguồn | `login.html`, `js/login.js`, `js/auth.js` |
| Giỏ hàng và tự điền thông tin người mua đã đăng nhập | Đạt trong mã nguồn | `cart.html`, `js/cart.js`; giỏ giữ món khi quay lại sau đăng nhập |
| Dùng địa chỉ đã lưu hoặc nhập địa chỉ mới | Đạt trong mã nguồn | Lựa chọn địa chỉ ở `cart.html` và lưu sau đặt hàng trong `js/cart.js` |
| Chọn tiền mặt hoặc thanh toán trực tuyến minh họa | Đạt trong mã nguồn | COD và QR demo ở `cart.html`; không mở cổng thanh toán thật |
| Lưu đơn sau giao dịch | Đạt trong mã nguồn | `saveOrder()` trong `js/cart.js` |
| Theo dõi ngay đơn vừa đặt | Đạt trong mã nguồn | Đơn bắt đầu ở trạng thái “Đang chuẩn bị”; nút theo dõi mang mã đơn và số điện thoại sang `orders.html` |
| Xem lịch sử mua hàng theo từng đơn | Đạt trong mã nguồn | `renderPurchaseHistory()` trong `js/orders.js` |

## Chức năng quản trị

| Tiêu chí | Trạng thái | Bằng chứng |
|---|---|---|
| URL đăng nhập quản trị riêng | Đạt trong mã nguồn | `admin-login.html` có biểu mẫu riêng; `js/admin-login.js` và `js/auth.js` chỉ cho tài khoản quản trị vào dashboard |
| Thêm, sửa, khóa và mở khóa tài khoản | Đạt trong mã nguồn | `renderUsers()`, `saveUser()` và `toggleUserStatus()` trong `js/admin.js` |
| Thêm món đúng danh mục, tải ảnh và xem trước | Đạt trong mã nguồn | `openProductForm()` và đọc ảnh trong `js/admin.js` |
| Sửa món với thông tin, danh mục và ảnh hiện tại | Đạt trong mã nguồn | `openProductForm(product)` trong `js/admin.js` |
| Xóa món chưa bán; ẩn món có trong đơn chưa hủy | Đạt trong mã nguồn | Xử lý `data-delete-product` trong `js/admin.js`; món có đơn đang chờ, đang chuẩn bị, đang giao hoặc hoàn thành được ẩn để giữ lịch sử |
| Cập nhật trạng thái theo chiều tiến; hủy đơn đang xử lý | Đạt trong mã nguồn | Chuỗi trạng thái và kiểm tra `canAdvance` trong `js/admin.js` |
| Lọc đơn theo trạng thái, ngày và địa điểm | Đạt trong mã nguồn | Bộ lọc cập nhật vùng kết quả riêng trong `js/admin.js`, không thay bộ lọc đang thao tác |
| Top 5 khách hàng theo thời gian, tổng tiền giảm dần và xem từng đơn | Đạt trong mã nguồn | `renderOverview()` nhóm đơn hoàn thành, lọc ngày, sắp xếp tổng mua và tạo link chi tiết |

## Dữ liệu và kiểm tra

- Dữ liệu demo nằm trong cơ sở dữ liệu cục bộ của trình duyệt (`localStorage`); không có máy chủ hoặc dữ liệu dùng chung giữa thiết bị.
- Mỗi voucher chỉ dùng một lần cho cùng tài khoản hoặc số điện thoại; lịch sử đơn lưu lượt dùng trong `localStorage`, nên thiết bị riêng biệt không đồng bộ lượt dùng.
- Có 1–4 đánh giá mẫu cho từng món; điểm sao và số lượt hiển thị được tính từ các đánh giá đang công khai.
- Admin có thể tạo món mới trong danh mục, thêm món đã có vào danh mục, hoặc gỡ món khỏi danh mục mà không xóa món.
- Nâng phiên bản dữ liệu lên `6` đồng bộ lại 21 nhóm món/48 lựa chọn, gộp tab gà rán với đồ chiên, cập nhật giá lẻ của 9 combo, bật tùy chỉnh món và thêm quản lý góp ý/combo, bỏ tab combo cũ, giữ nguyên hai tài khoản mẫu và mọi chỉnh sửa tài khoản, giữ tài khoản/món/danh mục tùy chỉnh và bỏ các mã giảm giá mẫu.
- Kiểm tra logic cục bộ với dữ liệu cũ: hai tài khoản mẫu đăng nhập được, tab combo cũ bị gỡ, voucher mẫu bị gỡ, dữ liệu tùy chỉnh được giữ.
- Đối chiếu menu với danh sách người dùng gửi: đủ 48/48 lựa chọn, không thiếu và không thừa.
- Chưa chạy kiểm tra JavaScript cho các thay đổi lượt này. OpenDesigner review/validate: đạt, không lỗi hoặc cảnh báo.
- Chưa kiểm tra trực tiếp giao diện laptop/desktop trên Chrome trong lượt này theo yêu cầu để bạn tự rà lần cuối; điểm hiển thị chưa chấm.
- Biên bản ghi tổng 12 điểm nhưng hai phần tiêu chí trích xuất cộng 10 điểm; 2 điểm còn lại không có tiêu chí rõ trong nội dung hiện có.
