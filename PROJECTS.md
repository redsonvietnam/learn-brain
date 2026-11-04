# Dự án thật

Mục đích: từ P1 trở đi, bài đọc code và debug dùng chính app của tôi thay vì ví dụ rời.
Quy tắc: chỉ mô tả. Không dán mật khẩu, API key hay dữ liệu thật của cơ quan vào đây.

## App 1: bamso
- Repo: redsonvietnam/bamso (đang Public).
- Làm gì: hệ thống xếp hàng lấy số: kiosk lấy số, màn hình gọi số, console cho cán bộ, trang admin. (Tóm tắt từ mô tả PR và sơ đồ tự động, chưa xác nhận bằng đọc code; tôi sẽ sửa lại cho đúng.)
- Ai dùng, khoảng bao nhiêu người: (chưa điền)
- Stack: TypeScript, Next.js, Prisma, SQLite, Redis; đăng nhập JWT có MFA; cập nhật thời gian thực bằng SSE.
- Quy trình: PR có CI (lint, kiểm tra kiểu, test, build) và review độc lập trước khi merge. Quyết định merge cuối cùng là của tôi.
- Chạy thế nào (lệnh): (chưa điền)
- Thư mục chính và việc của từng thư mục: (chưa điền)
- Có đụng dữ liệu nhạy cảm không (có/không, loại): (chưa điền)
- Việc mở về bảo mật: ghi riêng ở nơi riêng tư, không ghi vào repo này vì repo đang Public.
- Điều tôi muốn hiểu nhất về app này: (chưa điền)

## App hay prototype? (tick khi đúng)
- [ ] Nhập sai/để trống không làm app sập
- [ ] Có đăng nhập và phân quyền
- [ ] Mật khẩu, key không nằm trong code
- [ ] Có test chạy được
- [ ] Có log để biết lỗi gì
- [ ] Có backup dữ liệu
- [ ] Người khác đọc code có hiểu được
