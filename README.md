# CS221 PROJECT: SimCSE Contrastive Learning of Sentence Embeddings


🚀 THỰC HIỆN BỞI: NHÓM 8 🚀

📖 Tổng quan dự án
Đồ án môn học CS221, tập trung nghiên cứu mô hình SimCSE (Simple Contrastive Learning of Sentence Embeddings). 

Mục tiêu chính của nhóm là tái hiện lại kết quả huấn luyện theo paper gốc và xây dựng ứng dụng thực tế để kiểm tra chất lượng vector embeddings.


🧠 Huấn luyện mô hình (Training)
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
  python setup.py develop
  python python flaskdemo.py --model_name_or_path "princeton-nlp/sup-simcse-bert-base-uncased"
  ```

Hoặc thay đường dẫn model "--model_name_or_path" vào model sau khi train và tải model về từ kaggle.

Sau đó truy cập http://localhost:8888 để sử dụng giao diện demo.

📚 Tham khảo
Dự án này dựa trên mã nguồn và nghiên cứu từ:

SimCSE: Simple Contrastive Learning of Sentence Embeddings (Gao et al., EMNLP 2021)

GitHub: princeton-nlp/SimCSE
