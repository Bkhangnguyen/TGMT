# So sánh PIL và OpenCV trong xử lý ảnh

## Cơ bản 

* PIL (Pillow) : Thư viện xử lý ảnh mức cơ bản, cú pháp đơn giản, thích hợp cho người nhập môn.

* OpenCV (cv2) : Thư viện mạnh mẽ, hiệu năng cao, dùng cho thị giác máy tính ở mức chuyên sâu.

## So sánh 

Tiêu chí :

* PIL : 

- Dễ học dễ sử dụng , áp dụng đơn giản .

- Hiệu năng của PIL ở ngưỡng trung bình, chạy đủ nhanh cho các tác vụ đơn giản, nhưng không tối ưu cho xử lý nặng hoặc số lượng lớn ảnh.

- Thường làm việc với Image object, ít tối ưu cho xử lý song song hoặc thời gian thực.

- PIL dùng cho học tập và các tác vụ đơn giản .

* OpenCV : 

- Khó học hơn PIL do cú pháp và khái niệm phức tạp hơn, hướng tới người dùng có kiến thức nền về xử lý ảnh.

- Hiệu năng cao: xử lý nhanh, tối ưu tài nguyên, tận dụng tốt NumPy, CPU đa nhân và có thể mở rộng với GPU.

- Phù hợp cho bài toán lớn, ảnh độ phân giải cao, xử lý video hoặc thời gian thực.

- Các dự án thực tế như nhận diện khuôn mặt, phát hiện vật thể thường được sử dụng rộng rãi hơn.


## Kết luận

* Chọn **PIL** nếu cần xử lý ảnh đơn giản, nhanh gọn.
* Chọn **OpenCV** nếu cần hiệu năng cao và các thuật toán xử lý ảnh nâng cao.

