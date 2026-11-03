# Bảng điểm P0

Quy tắc: mỗi câu một dòng, ghi ngay sau khi chấm. Kết quả: Đ (đúng), M (đúng một phần), S (sai). M và S làm đứt chuỗi. P0 qua khi chuỗi Đ liên tiếp ≥ 10 và đã đọc đúng 3 traceback mới (xem ROADMAP.md).

Mã lỗi: L1 lệch biên range · L2 chỉ số từ 0 · L3 phép toán (% // /) · L4 trả lời con số tóm tắt thay vì cái in ra · L5 nhầm thứ tự dòng/điều kiện while · L6 nhẩm không vẽ bảng · L7 bảng theo trực giác, không đi từng dòng · L8 đọc traceback.

**Chuỗi đúng liên tiếp hiện tại: 0 · Tốt nhất: 5 · Tổng: 21 câu (9 Đ, 3 M, 9 S)**

| # | Ngày | Bài | KQ | Lỗi |
|---|---|---|---|---|
| 1 | 2026-11-03 | for range(5) print i | S | L4 |
| 2 | 2026-11-03 | range(2, 6) tổng | S | L1 |
| 3 | 2026-11-03 | ds[0], ds[2], len | Đ | |
| 4 | 2026-11-03 | 17 % 5, 10 % 2, 7 // 2 | M | L3 |
| 5 | 2026-11-03 | range(3, 7) | Đ | |
| 6 | 2026-11-03 | range(1, 1) | S | L1 |
| 7 | 2026-11-03 | viết range in 1 đến 5 | Đ | |
| 8 | 2026-11-03 | 9 // 2, 9 / 2, 9 % 2 | Đ | |
| 9 | 2026-11-03 | tổng số lẻ range(1, 5) | Đ | |
| 10 | 2026-11-03 | range(2, 9) số vòng | Đ | |
| 11 | 2026-11-03 | traceback ds[len(ds)] | Đ | |
| 12 | 2026-11-03 | while đếm ngược 3, 2, 1 | S | L4 |
| 13 | 2026-11-03 | print(i * 2) range(3) | S | L4, L6 |
| 14 | 2026-11-03 | while x * 3 < 20 | S | L6 |
| 15 | 2026-11-03 | ds range(1, len) | M | L1, L4 |
| 16 | 2026-11-03 | traceback phan_tu_cuoi([]) | M | L8 |
| 17 | 2026-11-03 | range(4) print i + 10 | Đ | |
| 18 | 2026-11-03 | while n * 2 < 30 | S | L5 |
| 19 | 2026-11-03 | ds range(2, len) | Đ | |
| 20 | 2026-11-03 | while n + 4 < 10 | S | L7 |
| 21 | 2026-11-03 | ds range(1, len + 1) có lỗi | S | L2, L7 |

**Thống kê lỗi:** L4 ×4 · L1 ×3 · L6 ×2 · L7 ×2 · L2 ×1 · L3 ×1 · L5 ×1 · L8 ×1
