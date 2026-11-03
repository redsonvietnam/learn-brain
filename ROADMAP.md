# Lộ trình

Trạng thái: [ ] chưa, [~] đang làm, [x] xong. Chỉ đánh [x] khi đạt tiêu chí.

## P0. Đọc và theo dõi code  [~]
Bài tập: exercises/P0-01-range-va-chi-so.md. Điểm: exercises/SCORE.md
- [ ] Vẽ bảng theo dõi cho mọi vòng lặp
- [ ] Hết lỗi lệch biên (range, chỉ số từ 0)
- [ ] Phân biệt `%` (chia dư) và `//` (chia nguyên)
- [ ] Đọc traceback theo 3 bước: loại lỗi, dòng nổ, ai gọi
**Qua giai đoạn khi:** làm đúng 10 bài đoán kết quả liên tiếp, và đọc đúng 3 traceback mới.

## P1. Debug theo bằng chứng và git  [ ]
Mẫu: templates/debug-note.md
- [ ] Quy trình: đọc lỗi/log, git diff xem hôm qua đổi gì, tái hiện lỗi, thu hẹp phạm vi
- [ ] Biết quay về commit tốt (revert/checkout) khi AI làm hỏng
**Qua giai đoạn khi:** tự sửa 3 lỗi thật trong app của mình theo quy trình, ghi vào LOG.md.

## P2. App vận hành thế nào  [ ]
- [ ] HTTP/API, JSON, request/response
- [ ] Database vs Excel, SQL cơ bản (SELECT, WHERE, JOIN)
- [ ] Đăng nhập: băm mật khẩu, session/token
**Qua giai đoạn khi:** tự vẽ được luồng đăng nhập và viết truy vấn nối 2-3 bảng.

## P3. Test và kiểm chứng  [ ]
- [ ] Đọc và chạy test, hiểu pass/fail
- [ ] Viết test đơn giản, thử input lạ (rỗng, quá dài, sai kiểu)
**Qua giai đoạn khi:** thêm test cho một chức năng của app và bắt được ít nhất 1 lỗi thật.

## P4. Sản phẩm thật gồm gì và thiết kế  [ ]
- [ ] Yêu cầu, mô hình dữ liệu, chia module
- [ ] Validate input, xử lý lỗi, log
- [ ] Bảo mật cơ bản: key không nằm trong code, phân quyền, dữ liệu nhạy cảm
- [ ] Backup, triển khai, tài liệu
**Qua giai đoạn khi:** viết được 1 trang thiết kế trước khi vibe code một tính năng mới.

## P5. Review code AI chuẩn dev  [ ]
- [ ] Đọc diff, nhận ra code smell và chỗ thiếu xử lý lỗi
- [ ] Chỉ đạo AI theo bước nhỏ, kiểm tra từng bước
**Qua giai đoạn khi:** review một diff lớn của AI và tìm ra ít nhất 3 vấn đề thật.
