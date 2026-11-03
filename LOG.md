# Nhật ký học

## 2026-11-02: đánh giá đầu vào
- Làm 2 vòng bài kiểm tra, xác định điểm mạnh/hổng (xem PROFILE.md).
- Dựng learn-brain.
- Bước tiếp theo: làm exercises/P0-01-range-va-chi-so.md, dự đoán trước rồi mới chạy.

## 2026-11-03: luyện P0 (6 vòng, 21 câu)
- Kết quả: 9 đúng, 3 đúng một phần, 9 sai. Chuỗi đúng liên tiếp tốt nhất 5, hiện tại 0 (xem exercises/SCORE.md).
- Tiến bộ: nắm range(a, b) dừng trước b (đúng các câu hỏi số vòng ở vòng 2-3), nắm % và //, đọc traceback theo 3 bước được khi có hướng dẫn, biết nói "không biết" thay vì đoán.
- Vấn đề chính: (1) trả lời bằng một con số tóm tắt thay vì cái được in ra; (2) bảng theo dõi nghĩ theo trực giác, không đi từng dòng code; (3) while: nhầm thứ tự print và dòng cập nhật, nghĩ biến tự tăng.
- Đã chốt: dùng bảng theo từng dòng (cột Dòng vừa chạy | Biến sau dòng đó | In ra). Dùng pythontutor.com sau khi tự dự đoán, không dùng trước.
- Quyết định có chủ đích: chưa đánh dấu P0 xong. Không thêm cấu trúc brain mới (ngoài PROJECTS.md và SCORE.md) cho tới khi qua P0.
- Bước tiếp theo: chạy thật 8 bài trong exercises/P0-01 và ghi vào file; làm 3 bài bảng theo từng dòng (gán biến liên tiếp, while có biến đếm, in ds[i]); điền PROJECTS.md.

## Sổ lỗi (ghi mỗi lần mắc lỗi và bài học)
| Ngày | Lỗi mắc | Bài học |
|---|---|---|
| 2026-11-02 | Tính thêm vòng thứ 4 cho `range(1, 4)` | range dừng trước số cuối |
| 2026-11-02 | Trả lời `ds[3]` là "chi" khi chỉ có 3 phần tử | Chỉ số bắt đầu từ 0, có IndexError |
| 2026-11-02 | Hiểu `%` là chia | `%` là chia lấy dư |
| 2026-11-02 | Đoán nguyên nhân trước khi đọc lỗi | Đọc lỗi/log trước, đoán sau |
| 2026-11-02 | Gặp lỗi chồng lỗi thì định chuyển sang AI khác | Quay về commit tốt, thu hẹp phạm vi |
| 2026-11-03 | Trả lời bằng một con số (5, 0, 4, 40) thay vì các dòng được in | Bảng có cột In ra riêng, đề hỏi gì đọc đúng cột đó |
| 2026-11-03 | Tính thêm số 6 cho `range(2, 6)`; trả lời 1 cho `range(1, 1)` | Số vòng = b − a, không chạm b; b − a = 0 thì không chạy |
| 2026-11-03 | Viết `7 // 2` bằng 3.5 | `//` là chia nguyên (3), `/` mới ra 3.5 |
| 2026-11-03 | while n < 30, n = n * 2: dừng ở 16, thiếu 32 | Điều kiện kiểm tra n ở đầu vòng; n = 16 vẫn chạy tiếp |
| 2026-11-03 | while n = n + 4: viết n tăng lần lượt 1, 2, 3 | while không có bộ đếm tự động, biến chỉ đổi khi có dòng đổi nó |
| 2026-11-03 | range(1, len + 1): coi ds[1] là phần tử đầu, bỏ sót IndexError | Chỉ số từ 0; i = len là ngoài khoảng |
| 2026-11-03 | Vẽ bảng bằng trực giác, không đi từng dòng | Bảng theo từng dòng code |
