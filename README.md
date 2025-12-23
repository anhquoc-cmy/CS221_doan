<!-- Banner -->
<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" style="border: none;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology">
  </a>
</p>

<h1 align="center"><b>XỬ LÝ NGÔN NGỮ TỰ NHIÊN</b></h>

## THÀNH VIÊN NHÓM
| STT    | MSSV          | Họ và Tên              |Chức Vụ    | Github                                                  | Email                   |
| ------ |:-------------:| ----------------------:|----------:|--------------------------------------------------------:|-------------------------:
| 1      | 23520774      | Nguyễn Đình Khôi       |Nhóm trưởng|[trong-khanh-1109](https://github.com/trong-khanh-1109)  |19521676@gm.uit.edu.vn   |
| 2      | 23520070      | Phạm Ngô Quốc Anh      |Thành viên |[ducducqn123](https://github.com/ducducqn123)            |19521383@gm.uit.edu.vn   |
| 3      | 23520070      | Đoàn Thái Hoàng        |Thành viên |[danhtrinh15092001](https://github.com/danhtrinh15092001)|19521326@gm.uit.edu.vn   |

## GIỚI THIỆU MÔN HỌC
* **Tên môn học:** Xử lý ngôn ngữ tự nhiên
* **Mã môn học:** CS221
* **Mã lớp:** CS221.Q12
* **Năm học:** HK1 (2025 - 2026)
* **Giảng viên**: TS.Nguyễn Thị Quý 

##Tổng quan dự án
Đồ án môn học CS221, tập trung nghiên cứu mô hình SimCSE (Simple Contrastive Learning of Sentence Embeddings). 

Mục tiêu chính của nhóm là tái hiện lại kết quả huấn luyện theo paper gốc và xây dựng ứng dụng thực tế để kiểm tra chất lượng vector embeddings.


##Huấn luyện mô hình (Training)
Chạy 4 file notebook trong thư mục train/ trên Kaggle là đủ. Không cần cài đặt gì thêm.

train/ 

      train/sup_bert.ipynb
      
      train/sup_roberta.ipynb
      
      train/unsup_bert.ipynb
      
      train/unsup_roberta.ipynb




🌐 Chạy Demo
Từ thư mục gốc, chạy lệnh sau để khởi động demo:

  ```bash
  cd demo

  pip install -r requirement

  python flaskdemo.py --model_name_or_path "princeton-nlp/sup-simcse-bert-base-uncased"
  ```

Hoặc thay đường dẫn model "--model_name_or_path" vào model sau khi train và tải về từ kaggle.

Sau đó truy cập http://localhost:8888 để sử dụng giao diện demo.

📚 Tham khảo
Dự án này dựa trên mã nguồn và nghiên cứu từ:

SimCSE: Simple Contrastive Learning of Sentence Embeddings (Gao et al., EMNLP 2021)

GitHub: princeton-nlp/SimCSE
