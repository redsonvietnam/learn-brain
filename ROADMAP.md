# Lộ trình

Trạng thái: [ ] chưa, [~] đang làm, [x] xong. Chỉ đánh [x] khi bằng chứng đã nằm trong repo và người học tự xác nhận (xem SPEC.md mục 12).

## P0. Đọc và theo dõi code  [~]
Bài tập: exercises/P0-01-range-va-chi-so.md. Điểm: exercises/SCORE.md
- [ ] Vẽ bảng theo dõi theo từng dòng code
- [ ] Hết lỗi lệch biên (range, chỉ số từ 0)
- [ ] Đọc đúng cái được in ra, không chỉ giá trị cuối
- [ ] Vòng while: thứ tự dòng và điều kiện kiểm tra
- [ ] Đọc traceback: loại lỗi, dòng nổ, ai gọi
**Bằng chứng:** SCORE.md có chuỗi 10 đúng liên tiếp và 3 traceback mới đọc đúng.
**Việc thật trên bamso:** đọc một hàm nhỏ và vẽ bảng theo dõi.

## P1. Debug theo bằng chứng và git  [ ]
Mẫu: templates/debug-note.md
- [ ] Quy trình: đọc lỗi, git diff, tái hiện, thu hẹp phạm vi
- [ ] Quay về commit tốt khi AI làm hỏng
**Bằng chứng:** 3 ghi chú debug đã commit, mỗi cái có giả thuyết viết trước.
**Việc thật trên bamso:** quét bí mật trong lịch sử git (kết quả ghi ở nơi riêng tư, không ghi vào repo Public).

## P2. App vận hành thế nào  [ ]
- [ ] HTTP/API, JSON, request/response
- [ ] Database vs Excel, SQL cơ bản (SELECT, WHERE, JOIN)
- [ ] Đăng nhập: băm mật khẩu, session/token
**Bằng chứng:** docs/dang-nhap.md (sơ đồ luồng đăng nhập) và 1 truy vấn nối bảng chạy thật.
**Việc thật trên bamso:** vẽ luồng kiosk, lấy số, màn hình gọi số.

## P3. Test và kiểm chứng  [ ]
- [ ] Đọc và chạy test, hiểu pass/fail
- [ ] Viết test đơn giản, thử input lạ (rỗng, quá dài, sai kiểu)
**Bằng chứng:** commit thêm test, CI xanh, test bắt được lỗi thật.
**Việc thật trên bamso:** đọc một file test và thêm một test.

## P4. Sản phẩm thật và thiết kế  [ ]
- [ ] Yêu cầu, mô hình dữ liệu, chia module
- [ ] Validate input, xử lý lỗi, log
- [ ] Bảo mật cơ bản: key không nằm trong code, phân quyền ở server, dữ liệu nhạy cảm
- [ ] Backup, triển khai, tài liệu
**Bằng chứng:** specs/<tên>.md một trang, viết trước khi vibe code tính năng.
**Việc thật trên bamso:** viết spec cho một tính năng nhỏ.

## P5. Review code AI chuẩn dev  [ ]
- [ ] Đọc diff, nhận ra code smell và chỗ thiếu xử lý lỗi
- [ ] Chỉ đạo AI theo bước nhỏ, kiểm tra từng bước
**Bằng chứng:** reviews/PR-<số>.md với ít nhất 3 vấn đề, đối chiếu với CI.
**Việc thật trên bamso:** làm cổng duyệt cuối cho một PR.

## Đích
Đủ sức làm cổng duyệt cuối cho một PR của bamso: tự đọc diff, hiểu kết quả CI, quyết định merge dựa trên bằng chứng, không chỉ dựa vào lời AI báo cáo.
