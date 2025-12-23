**CS221 Project - SimCSE: Contrastive Learning of Sentence Embeddings
Dự án này là bài tập môn học (đồ án) CS221, tập trung vào việc nghiên cứu, cài đặt và demo mô hình SimCSE (Simple Contrastive Learning of Sentence Embeddings). Dự án bao gồm các notebook để huấn luyện mô hình (cả Supervised và Unsupervised) trên nền tảng BERT/RoBERTa và một ứng dụng web demo sử dụng Flask.


🧠 Huấn luyện mô hình (Training)
Chạy 4 file notebook trong thư mục train/ (sup_bert.ipynb, sup_roberta.ipynb, unsup_bert.ipynb, unsup_roberta.ipynb) trên Kaggle là đủ. Không cần cài đặt gì thêm.


🌐 Chạy Demo
Từ thư mục gốc, chạy lệnh sau để khởi động demo:

  ```bash
  cd demo
  pip install -r requirement
  python python flaskdemo.py --model_name_or_path "princeton-nlp/sup-simcse-bert-base-uncased"
  ```

Hoặc thay bằng đường dẫn model sau khi tải về từ kaggle.
Sau đó truy cập http://localhost:8888 để sử dụng giao diện demo.

📚 Tham khảo
Dự án này dựa trên mã nguồn và nghiên cứu từ:

SimCSE: Simple Contrastive Learning of Sentence Embeddings (Gao et al., EMNLP 2021)

GitHub: princeton-nlp/SimCSE

Nhóm thực hiện: Nhóm 8
