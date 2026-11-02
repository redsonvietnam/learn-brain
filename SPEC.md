# SPEC: learn-brain vận hành thế nào

## 1. Mục đích
Một nơi duy nhất ghi mục tiêu, trình độ, lộ trình, tiến độ và lỗi đã mắc, để mọi AI người dùng dùng đều biết người học đang ở đâu mà không cần giải thích lại.

## 2. Nguyên tắc
- Chỉ dùng file Markdown và git. Không làm app, không thêm công cụ.
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
