# SPEC: learn-brain vận hành thế nào

## 1. Mục đích
Một nơi duy nhất ghi mục tiêu, trình độ, lộ trình, tiến độ và lỗi đã mắc, để mọi AI người dùng dùng đều biết người học đang ở đâu mà không cần giải thích lại.

## 2. Nguyên tắc
- Nguồn dữ liệu và bằng chứng chuẩn là Markdown và git. `dashboard.html` là giao diện tĩnh phụ trợ để luyện tập và nhập/xuất `exercises/SCORE.md`; không thay thế file Markdown, nhật ký hay bằng chứng trong repo.
- Không tạo web app/backend hoặc thêm framework, thư viện hay dịch vụ bên ngoài.
- AI là gia sư; tiến bộ phải do người học chứng minh được.
- Ít mà dùng thật: chưa tới phase nào thì chưa tạo tài liệu cho phase đó.

## 3. Cấu trúc
```
README.md  AGENTS.md  SPEC.md
PROFILE.md  ROADMAP.md  MAP.md  LOG.md
exercises/   P<phase>-<số>-<tên-ngắn>.md
templates/   debug-note.md  (design-1page.md ở P4, review-diff.md ở P5)
```

## 4. Khi nào cập nhật gì
- PROFILE.md: khi đánh giá lại trình độ (sau mỗi phase hoặc kiểm tra lại).
- ROADMAP.md: tick checklist khi làm xong; đổi trạng thái phase khi đạt tiêu chí.
- MAP.md: đổi `:::todo` thành `:::doing` hoặc `:::done` đúng với ROADMAP.md.
- LOG.md: cuối mỗi phiên.
- exercises/: tạo mới khi vào phase; mỗi file có phần Dự đoán / Kết quả thật / Sai ở đâu.

## 5. Quy trình phiên
Đầu: đọc PROFILE, ROADMAP, cuối LOG. Giữa: dự đoán trước, chạy sau, so sánh. Cuối: ghi LOG, cập nhật ROADMAP/MAP, commit. Dừng gấp: xuất BÁO CÁO PHIÊN (xem AGENTS.md).

## 6. Quy ước commit
`log: ...` nhật ký, `roadmap: ...` lộ trình/bản đồ, `exercise: ...` bài tập, `profile: ...` hồ sơ.

## 7. Không làm
- Không biến brain thành app hay thêm tính năng cho đẹp.
- Không để phase "xong" theo cảm giác.
- Không lưu mật khẩu, key, dữ liệu thật.

## 8. Mở rộng
Tới P4 thì AI tạo templates/design-1page.md; tới P5 thì templates/review-diff.md. Khi phát hiện hổng mới, thêm vào PROFILE.md và tạo bài tập tương ứng.


## 9. Phân vai
- AI gia sư (Claude hoặc AI đang dùng): soạn nội dung, ra bài, chấm, giải thích; không tự tuyên bố qua phase.
- opencode / ChatGPT: ghi file, commit, push theo khối dán, rồi báo cáo File / Đã làm / Kết quả.
- Tôi: làm bài, chạy thật, kiểm tra diff trên GitHub, quyết định qua phase theo tiêu chí.
- Ghi điểm vào exercises/SCORE.md ngay sau khi chấm mỗi câu.

## 10. File bổ sung
- PROJECTS.md: mô tả app thật; nguồn bài tập từ P1.
- exercises/SCORE.md: bảng điểm và thống kê loại lỗi.
- dashboard.html: giao diện tĩnh chạy cục bộ, không backend và không phụ thuộc bên ngoài; SCORE.md vẫn là nguồn chuẩn.
- Đóng băng khung: không thêm cấu trúc mới (ngoài bài tập) cho tới khi qua P0.

## 11. Bốn vòng lặp
- Ngày (10 phút): làm bài trên dashboard, dự đoán trước rồi mới xem đáp án, ghi điểm.
- Tuần (30 phút): xuất SCORE.md và commit; xem lại kỹ năng yếu nhất; viết 1 ghi chú debug.
- Phase: nộp bằng chứng (mục 12), người học tự xác nhận.
- Dự án: dùng bamso làm đề thật theo từng phase (xem PROJECTS.md).

## 12. Cổng bằng chứng
AI không tự xác nhận qua phase. Chỉ người học xác nhận, và chỉ khi bằng chứng đã nằm trong repo.
- P0: SCORE.md có chuỗi 10 đúng liên tiếp và 3 traceback mới đọc đúng.
- P1: 3 ghi chú debug đã commit (mẫu templates/debug-note.md), mỗi cái có giả thuyết viết trước.
- P2: docs/dang-nhap.md (sơ đồ luồng đăng nhập) và 1 truy vấn nối bảng chạy thật.
- P3: commit thêm test, CI xanh, test bắt được lỗi thật.
- P4: specs/<tên>.md một trang, viết trước khi vibe code tính năng.
- P5: reviews/PR-<số>.md với ít nhất 3 vấn đề, đối chiếu với CI.

## 13. Nhịp và quy tắc chặn
- Ít nhất 3 buổi 10 phút mỗi tuần.
- Thiếu buổi thì dừng thêm cấu trúc hoặc tính năng mới cho brain.
- Thư mục debug-notes/, docs/, specs/, reviews/ chỉ tạo khi tới phase tương ứng.
