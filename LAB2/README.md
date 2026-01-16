# Xử lý ảnh cơ bản với PIL và OpenCV

## 1. Giới thiệu

Repository này gồm **hai tệp notebook** minh họa các thao tác xử lý ảnh cơ bản bằng Python:

* `2.2.1_basic_image_manipulation_PIL.ipynb`: sử dụng thư viện **PIL (Pillow)**
* `2.2.2_basic_image_manipulation_open_CV.ipynb`: sử dụng thư viện **OpenCV (cv2)**

Mục tiêu là giúp người học:

* Hiểu **lý thuyết nền tảng** của xử lý ảnh
* Thực hành các **phép biến đổi cơ bản**
* So sánh sự khác nhau giữa **PIL** và **OpenCV** trong thực tế

---

## 2. Lý thuyết cơ bản

### 2.1 PIL (Pillow)

* Là thư viện xử lý ảnh mức cơ bản trong Python.
* Dễ sử dụng, cú pháp trực quan, phù hợp cho người mới học.
* Ảnh được biểu diễn dưới dạng đối tượng `PIL.Image`.
* Hệ màu mặc định: **RGB**.

### 2.2 OpenCV (cv2)

* Thư viện mạnh mẽ, hiệu năng cao, chuyên dùng cho **Computer Vision**.
* Phổ biến trong các ứng dụng realtime, AI, xử lý video.
* Ảnh được biểu diễn dưới dạng **NumPy array**.
* Hệ màu mặc định: **BGR** (Blue – Green – Red).

---

## 3. Nội dung thực hành trong hai tệp

### 3.1 Các thao tác chung

Cả hai notebook đều thực hiện các thao tác xử lý ảnh cơ bản sau:

* Đọc ảnh từ file
* Hiển thị ảnh
* Thay đổi kích thước (Resize)
* Xoay ảnh (Rotate)
* Cắt ảnh (Crop)
* Chuyển ảnh sang ảnh xám (Grayscale)

---

### 3.2 Thực hành với PIL (`2.2.1_basic_image_manipulation_PIL.ipynb`)

Đặc điểm chính:

* Mỗi phép biến đổi tương ứng với **một hàm rõ ràng**.
* Ít thao tác với chỉ số mảng.
* Phù hợp để minh họa **ý tưởng và khái niệm**.

Ví dụ thao tác tiêu biểu:

* `Image.open()` để đọc ảnh
* `resize()` để đổi kích thước
* `rotate()` để xoay ảnh
* `crop()` để cắt vùng ảnh
* `convert('L')` để chuyển sang ảnh xám

---

### 3.3 Thực hành với OpenCV (`2.2.2_basic_image_manipulation_open_CV.ipynb`)

Đặc điểm chính:

* Ảnh là mảng NumPy → thao tác trực tiếp bằng chỉ số hàng/cột.
* Linh hoạt và kiểm soát chi tiết hơn.
* Yêu cầu hiểu về **ma trận ảnh** và **hệ tọa độ**.

Ví dụ thao tác tiêu biểu:

* `cv2.imread()` để đọc ảnh
* `cv2.resize()` để đổi kích thước
* `cv2.rotate()` hoặc ma trận affine để xoay
* Cắt ảnh bằng slicing NumPy
* `cv2.cvtColor()` để chuyển ảnh xám

---

## 4. So sánh PIL và OpenCV

| Tiêu chí     | PIL (Pillow)     | OpenCV (cv2)      |
| ------------ | ---------------- | ----------------- |
| Mục đích     | Xử lý ảnh cơ bản | Thị giác máy tính |
| Độ khó       | Dễ học           | Khó hơn           |
| Kiểu dữ liệu | `PIL.Image`      | `NumPy array`     |
| Hệ màu       | RGB              | BGR               |
| Hiệu năng    | Trung bình       | Cao               |

---

## 5. Kết luận

* **PIL** phù hợp cho người mới học và các bài toán xử lý ảnh đơn giản.
* **OpenCV** phù hợp cho các ứng dụng nâng cao, yêu cầu hiệu năng và xử lý chuyên sâu.
* Hai notebook giúp người học thấy rõ **sự khác biệt giữa tư duy xử lý ảnh mức cao (PIL)** và **mức thấp (OpenCV)**.
---

## 6. Phần câu hỏi (Questions)

### **Bài 1 – PIL**

* Thực hiện các thao tác xử lý ảnh cơ bản: **đọc ảnh**, **resize**, **rotate**, **crop**, **chuyển ảnh xám**.
* Tập trung vào việc **hiểu khái niệm** và **sử dụng các hàm có sẵn** của PIL.
* Mục tiêu: làm quen xử lý ảnh ở mức **high-level**, **dễ tiếp cận cho người mới**.

### **Bài 2 – OpenCV**

* Thực hiện các thao tác tương tự nhưng trên **ảnh dạng mảng NumPy**.
* Bao gồm **resize**, **rotate**, **crop bằng slicing**, **chuyển màu BGR → Grayscale**.
* Mục tiêu: hiểu **cấu trúc dữ liệu ảnh**, **hệ màu BGR**, và xử lý ảnh ở mức **low-level**.

### **Nhận xét chung**

* **PIL** giúp **nắm nhanh kiến thức nền tảng**.
* **OpenCV** giúp **hiểu sâu** và **kiểm soát chi tiết** hơn.
* Hai phần **Questions bổ trợ cho nhau** trong quá trình học xử lý ảnh.
