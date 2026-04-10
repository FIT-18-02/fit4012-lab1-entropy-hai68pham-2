# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Hiểu và áp dụng các khái niệm entropy và độ dư thừa thông tin để đánh giá dữ liệu. Cài đặt và kiểm chứng thuật toán tìm nghịch đảo modulo bằng Euclid mở rộng.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính

### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0.0 | 8.0 | Chuỗi lặp hoàn toàn, entropy thấp, dễ đoán |
| abcd | 2.0 | 6.0 | Chuỗi đa dạng, entropy cao hơn |
| hello world | 2.845 | 5.155 | Mức trung bình, có lặp nhưng không hoàn toàn |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | Không tồn tại |

## 4. Kết luận
Qua bài lab, em hiểu rõ hơn về entropy và độ dư thừa thông tin trong dữ liệu. Em nhận thấy dữ liệu càng lặp lại thì entropy càng thấp và redundancy càng cao, từ đó dễ bị dự đoán hơn. Ngoài ra, em cũng hiểu cách sử dụng thuật toán Euclid mở rộng để tìm nghịch đảo modulo. Khó khăn lớn nhất là hiểu cách hoạt động của thuật toán, nhưng sau khi chạy thử nhiều ví dụ, em đã nắm rõ hơn.
