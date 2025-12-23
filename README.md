🚀 Cài đặt môi trường
Để chạy dự án, bạn cần cài đặt các thư viện Python cần thiết. Khuyến nghị sử dụng Python 3.7 trở lên.

Các thư viện chính bao gồm:

PyTorch

SimCSE (của Princeton-NLP)

Flask, Flask-CORS

Tornado

Transformers, NumPy, Scikit-learn

Bạn có thể cài đặt thông qua pip:

Bash

pip install simcse flask flask-cors tornado torch transformers tqdm numpy
(Lưu ý: Trong các file notebook train/, quá trình cài đặt môi trường và tải dữ liệu huấn luyện đã được tích hợp sẵn trong các cell code).


🧠 Huấn luyện mô hình (Training)
Chạy 4 file notebook trong thư mục train/ (sup_bert.ipynb, sup_roberta.ipynb, unsup_bert.ipynb, unsup_roberta.ipynb) trên Kaggle là đủ. Không cần cài đặt gì thêm.


🌐 Chạy Demo
Từ thư mục gốc, chạy lệnh sau để khởi động demo:

python demo/flaskdemo.py --model_name_or_path "princeton-nlp/sup-simcse-bert-base-uncased"

Hoặc thay bằng đường dẫn model bạn đã train.
Sau đó truy cập http://localhost:8888 để sử dụng giao diện demo.

📚 Tham khảo
Dự án này dựa trên mã nguồn và nghiên cứu từ:

SimCSE: Simple Contrastive Learning of Sentence Embeddings (Gao et al., EMNLP 2021)

GitHub: princeton-nlp/SimCSE

Nhóm thực hiện: [Tên của bạn/Nhóm của bạn]
