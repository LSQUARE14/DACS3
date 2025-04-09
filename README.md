### Sản phẩm dự tính:

- App đa thiết bị: dữ liệu lấy từ API (tự dựng & API free).
- Chạy MySQL, gồm 1 web server & 1 app điện thoại.

#### Chức năng:

#### User:

- Quản lý đặt bàn:
  - Mô tả:
    - Đặt bàn và món ăn hoặc hủy bàn thông qua app (dữ liệu lấy từ API).
    - Gửi thông báo về trạng thái đặt bàn bằng email.
    - Theo dõi thông tin & lịch sử đặt bàn.
- Giỏ hàng:
  - Mô tả: CRUD món ăn, đặt vào giỏ hàng -> Đặt bàn.
- Hiển thị menu các món ăn:
  - Mô tả: Đổ dữ liệu về và hiển thị các món ăn.
- Tìm kiếm & lọc theo các tiêu chí:
  - Mô tả:
    - Tìm kiếm món ăn theo tên.
    - Lọc các món theo các tiêu chí (hot của mùa, best seller, theo giá).
    - Hiển thị thông tin đặc biệt cho các món địa phương (Đà Nẵng).
- Đăng nhập & đăng ký:
  - Mô tả:
    - Đăng nhập, đăng ký.
    - Gửi email xác thực.
- Cổng thanh toán:
  - Mô tả:
    - Hiển thị thông tin bàn & món ăn đã đặt.
    - Mã QR để thanh toán (đặt bừa QR nào cũng được)
  - Quy trình thanh toán:
    - Khách xem QR trên app (tình trạng của bàn là: Chờ xác nhận).
    - Quy tắc: Chuyển khoản trong vòng 30p kể từ khi đặt bàn với cú pháp XXX.
    - Admin kiểm tra chuyển khoản rồi mới xác nhận.

#### Admin:

- Quản lý đặt bàn:
  - Mô tả:
    - Xác nhận bàn, hủy bàn đã được đặt (email | push notification)
    - CCRUD bàn có sẵn.
- Quản lý thực đơn:
  - Mô tả:
    - CRUD món ăn.
    - CRUD danh mục.

### Giao diện:

- Lấy cảm hứng KFC
- Navbar còn 4 mục (Trang chủ - Thực đơn - Đặt bàn - Thêm)
- Trang chủ:
  - Một nút đặt bàn ở trên
  - Một banner ảnh ở giữa.
  - Icon giỏ hàng: Nhấn vào hiện 1 dialog ngay giữa màn hình, dialog bao gồm các món ăn đã chọn và 2 nút **Thêm món** và **Thanh toán**.
  - 3 mục đề xuất:
    - Món ăn mới
    - Best seller.
    - Đặc sản.
- Trang thực đơn:
  - Một nút đặt bàn
  - Thanh category ngang (Khai vị, món chính, món lẩu, món chay, tráng miệng, đồ uống)
  - Một nút lọc (lọc theo giá).
  - Hiển thị danh sách các món ăn (một hàng, full chiều ngang)
  - Thanh nav ở dưới.
- Trang đặt hàng:
  - Một khung nhập các thông tin đặt bàn (một ô, full ngang)
  - Một danh sách các món ăn đã chọn (một cột, full ngang)
  - Một nút đặt bàn (full ngang, nhấn cái thì nó hiện dialog xác nhận đặt bàn).
- Trang xác nhận thông tin đặt hàng.
  - Y chang trang đặt hàng.
  - Kèm mục mã QR (mã QR phụ thuộc vào số tiền).
  - Ở dưới cùng thêm hai nút (Quay lại và Đặt hàng).
- Trang Thêm:
  - Bỏ phần danh mục món ăn.
  - Clone KFC.
- Trang đăng nhập đăng ký:
  - Một ô giữa màn hình gồm 2 hàng và 2 nút.
