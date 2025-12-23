<!-- Banner -->
<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" style="border: none;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology">
  </a>
</p>

<h1 align="center"><b>XỬ LÝ NGÔN NGỮ TỰ NHIÊN</b></h>

## THÀNH VIÊN NHÓM
| STT | MSSV     | Họ và Tên         | Chức Vụ     | Email                  |
|-----|----------|-------------------|-------------|------------------------|
| 1   | 23520774 | Nguyễn Đình Khôi  | Nhóm trưởng | 23520774@gm.uit.edu.vn |
| 2   | 23520070 | Phạm Ngô Quốc Anh | Thành viên  | 23520070@gm.uit.edu.vn |
| 3   | 23520514 | Đoàn Thái Hoàng   | Thành viên  | 23520514@gm.uit.edu.vn |

## GIỚI THIỆU MÔN HỌC
* **Tên môn học:** Xử lý ngôn ngữ tự nhiên
* **Mã môn học:** CS221
* **Mã lớp:** CS221.Q12
* **Năm học:** HK1 (2025 - 2026)
* **Giảng viên**: TS.Nguyễn Thị Quý 

## Tổng quan dự án
Đồ án môn học CS221, tập trung nghiên cứu mô hình SimCSE (Simple Contrastive Learning of Sentence Embeddings). 

Mục tiêu chính của nhóm là tái hiện lại kết quả huấn luyện theo paper gốc và xây dựng giao diện trực quan để kiểm tra kết quả học của model.




## Huấn luyện mô hình (Training)
Chạy 4 file notebook này trên Kaggle là đủ. Không cần cài đặt gì thêm.


    train/ 
      sup_bert.ipynb
      unsup_bert.ipynb
      sup_roberta.ipynb
      unsup_roberta.ipynb




## Chạy Demo
Từ thư mục gốc, chạy lệnh sau để khởi động demo:

  ```bash
  # di chuyển vào thư mục demo
  cd demo

  # tải thư viện cần thiết
  pip install -r requirements

  # chạy backend bằng Flask
  python flaskdemo.py --model_name_or_path "princeton-nlp/sup-simcse-bert-base-uncased"
  ```

Hoặc thay đường dẫn model "--model_name_or_path" vào model sau khi train và tải về từ kaggle.

Sau đó truy cập http://localhost:8888 để sử dụng giao diện demo.

## Video Demo
https://github.com/anhquoc-cmy/CS221_doan.git/main/cs221_demo_nhom8.mp4


## Tham khảo
Dự án này dựa trên mã nguồn và nghiên cứu từ:

SimCSE: Simple Contrastive Learning of Sentence Embeddings (Gao et al., EMNLP 2021)

GitHub: princeton-nlp/SimCSE
