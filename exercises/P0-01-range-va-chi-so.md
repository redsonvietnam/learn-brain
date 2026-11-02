# P0-01: range, chỉ số, phép chia dư

Cách làm: ghi **Dự đoán** (kèm bảng theo dõi nếu có vòng lặp) trước, rồi mới chạy thật, rồi ghi **Kết quả thật** và **Sai ở đâu**. Không hỏi AI trước khi chạy.

## Bài 1
```python
for i in range(5):
    print(i)
```
Dự đoán: 
Kết quả thật: 
Sai ở đâu: 

## Bài 2
```python
total = 0
for i in range(2, 6):
    total = total + i
print(total)
```
Dự đoán: 
Kết quả thật: 
Sai ở đâu: 

## Bài 3
```python
ds = [7, 8, 9]
print(ds[0], ds[2], len(ds))
```
Dự đoán: 
Kết quả thật: 
Sai ở đâu: 

## Bài 4
```python
print(17 % 5, 10 % 2, 7 // 2)
```
Dự đoán: 
Kết quả thật: 
Sai ở đâu: 

## Bài 5
```python
count = 0
for n in range(1, 8):
    if n % 3 == 0:
        count += 1
print(count)
```
Dự đoán: 
Kết quả thật: 
Sai ở đâu: 

## Bài 6
Muốn in các số từ 1 đến 10 (gồm cả 10) nhưng code này sai ở đâu? Sửa thế nào?
```python
for i in range(1, 10):
    print(i)
```
Dự đoán: 
Kết quả thật: 
Sai ở đâu: 

## Bài 7
```python
ds = ["a", "b", "c"]
for i in range(len(ds) + 1):
    print(ds[i])
```
Dự đoán (in ra gì, lỗi gì, ở dòng nào): 
Kết quả thật: 
Sai ở đâu: 

## Bài 8
```python
x = 10
while x > 0:
    x -= 4
    print(x)
```
Dự đoán (kèm bảng theo dõi): 
Kết quả thật: 
Sai ở đâu: 
