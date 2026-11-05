# Vì sao Kat trông như vậy

## Sản phẩm

Kat là website đặt đồ ăn vặt cho người đặt món không thường xuyên, phần lớn thao tác bằng điện thoại. Chủ dự án chọn tên Kat và yêu cầu tên quán, địa chỉ, giờ mở cửa, số điện thoại cùng email để ở dạng placeholder có thể tự cập nhật. Maika và Popeyes là nguồn tham khảo về cấu trúc trang và luồng đặt món; thông tin cửa hàng của họ không được dùng làm dữ liệu của Kat.

Trang chủ dùng carousel ảnh tràn toàn chiều ngang, ghép thông điệp giao hàng vào cùng hero, kèm thẻ giá món nổi. Mũi tên hiện khi tương tác, tự mờ sau ba giây; ảnh tự chuyển mờ dần sau mỗi năm giây và bấm mũi tên sẽ trượt ngang, riêng vòng cuối về đầu sẽ mờ dần. Phần giới thiệu nói về quán ăn vặt do bốn sinh viên lập nên. Khối đánh giá khách hàng được gỡ khỏi homepage để trang gọn hơn. Khách lọc thực đơn theo tên món, danh mục và ba khoảng giá; danh sách nạp thêm món khi cuộn xuống. Giỏ hàng yêu cầu đăng nhập trước khi đặt, dùng địa chỉ đã lưu hoặc nhập địa chỉ khác, rồi chọn tiền mặt khi nhận hoặc QR chưa kết nối thanh toán. Tài khoản khách và quản trị đăng nhập bằng số điện thoại tại hai URL riêng; tra cứu đơn bằng số điện thoại.

## Năm lựa chọn định hình giao diện

1. **Tính cách:** Câu chữ thân thiện, mạnh mẽ và vui tươi giúp thực đơn dễ gần và làm rõ món ăn vặt.
2. **Nền tảng:** Website nhiều trang bằng HTML, CSS và JavaScript thuần bám sát yêu cầu bàn giao và chạy mà không cần cài thư viện.
3. **Hướng hình ảnh:** Giao diện chỉ giữ bảng màu sáng; theme tối cũ đã bị loại bỏ. Nền trắng, ảnh món ăn và khoảng trắng tạo nhịp điệu chính.
4. **Mật độ:** Bố cục thoáng dành chỗ cho ảnh món, tùy chọn và giá trên màn hình điện thoại. Nạp món khi cuộn giúp duyệt thực đơn dài không cần đổi trang.
5. **Vai trò màu thương hiệu:** Kat dùng palette Maika gốc theo yêu cầu mới: đỏ burgundy `#8C2224`, hover `#6E1B1C`, nền trắng, tiêu đề `#111111`, nội dung `#252525`, chữ phụ `#666666`, viền `#E5E5E5`, chữ footer `#E0E0E0` và hover liên kết footer `#F1D0A5`.

## Các nguyên tắc được áp dụng

- Hệ thống đã kiểm tra 94 cặp màu qua 6 tổ hợp chế độ và mật độ; kết quả không có lỗi hoặc cảnh báo.
- CSS dùng token thiết kế đã xuất cho màu, khoảng cách, chữ, góc bo, chuyển động và đổ bóng.
- Có vòng focus nhìn thấy được và hỗ trợ cài đặt giảm chuyển động.
- Khi dùng điều khiển cao 24 px, hệ thống khuyến nghị vùng chạm 44 px.
- Địa chỉ, giờ hoạt động và liên hệ không được tự điền bằng dữ liệu Maika hoặc Popeyes.

## Những điểm còn mở

- Mô tả người dùng dựa trên tài liệu bàn giao và nghiên cứu nhanh; cần xác nhận với khách hàng thật của Kat.
- Logo Kat do người dùng cung cấp được lưu tại `images/kat-logo.png`. Ảnh món Pexels vẫn chỉ để minh họa; nguồn nằm ở `images/SOURCES.md`. Hướng dẫn giọng điệu và font thương hiệu riêng vẫn chưa có.
- Bản build có 3 ghi chú: vùng chạm cho điều khiển 24 px, mười bước tỷ lệ chưa dùng và tài sản thương hiệu còn thiếu.
- Ảnh người dùng gửi là ảnh giao diện cũ trước khi đổi tên và bảng màu. Chưa kiểm tra trực quan các trang sau thay đổi; báo cáo tại `opendesigner/review/REPORT.md` ghi rõ phạm vi còn thiếu.

## Cách đề xuất thay đổi

Chủ dự án phê duyệt thay đổi cho hệ thống thiết kế. Dùng skill `opendesigner-extend` để đọc các lựa chọn hiện có, xem ảnh hưởng của thay đổi và ghi quyết định mới vào `opendesigner/decisions.md`.

## Dành cho đội thiết kế

Ưu tiên cung cấp logo, ảnh món thật, hướng dẫn giọng điệu, font thương hiệu và biểu tượng riêng. Dùng `images/SOURCES.md` để xác định và thay ảnh minh họa hiện tại.

---

Ghi chú: Q-aud-01, Q-aud-02, Q-plat-01, Q-scope-07; D-0006, D-0007, D-0011–D-0015, D-0018–D-0024, D-0049–D-0063.
