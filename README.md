## Demo

Chúng tôi cung cấp các bản demo đơn giản để minh họa khả năng của mô hình trong việc tìm kiếm và so sánh độ tương đồng ngữ nghĩa của các câu. Mã nguồn demo nằm trong thư mục `demo/`.

### Flask Demo
<div align="center">
  <img src="https://raw.githubusercontent.com/princeton-nlp/SimCSE/main/figure/demo.gif" width="750" alt="Demo Preview">
</div>

Chúng tôi cung cấp một Web demo dựa trên [Flask](https://github.com/pallets/flask) để hiển thị cách mô hình được sử dụng trực tiếp cho bài toán truy xuất thông tin (information retrieval). 

Để chạy demo này trên máy cục bộ (local), hãy làm theo các bước sau:

1. **Cài đặt thư viện**:
   Đảm bảo bạn đã cài đặt `flask` và các thư viện yêu cầu:
   ```bash
   pip install flask
   # Cài đặt thêm faiss nếu muốn tăng tốc độ tìm kiếm (tùy chọn)
   # pip install faiss-cpu
