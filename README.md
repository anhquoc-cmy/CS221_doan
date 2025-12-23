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
Để huấn luyện lại các mô hình, hãy mở và chạy các file Jupyter Notebook trong thư mục train/.

Ví dụ quy trình trong sup_bert.ipynb:

Notebook sẽ tự động clone repo gốc princeton-nlp/SimCSE.

Tải xuống dữ liệu cần thiết (Wiki cho unsupervised hoặc NLI cho supervised).

Cài đặt các dependency.

Chạy script train.py để fine-tune mô hình.

Mô hình sau khi huấn luyện sẽ được lưu tại thư mục output (ví dụ: result/my-sup-simcse-bert-base-uncased).

🌐 Chạy Demo
Ứng dụng demo cho phép bạn nhập một câu truy vấn và tìm các câu có ý nghĩa tương đồng nhất trong tập dữ liệu mẫu.

1. Chuẩn bị
Đảm bảo bạn đã có mô hình (hoặc sử dụng pre-trained model từ HuggingFace) và các file dữ liệu mẫu trong demo/static/.

2. Lệnh chạy
Từ thư mục gốc của dự án, chạy lệnh sau:

Bash

python demo/flaskdemo.py --model_name_or_path <đường_dẫn_model_hoặc_tên_model>
Các tham số tùy chọn:

--model_name_or_path: Đường dẫn đến thư mục model đã train của bạn hoặc tên model trên HuggingFace (VD: princeton-nlp/sup-simcse-bert-base-uncased). Mặc định là None.

--port: Cổng chạy server (mặc định: 8888).

--sentences_dir: Thư mục chứa file dữ liệu mẫu (mặc định: demo/static).

--example_sentence: Tên file chứa corpus các câu (mặc định: example_sentence.txt).

Ví dụ chạy thực tế:

Bash

# Sử dụng model pre-trained của Princeton NLP
python demo/flaskdemo.py --model_name_or_path princeton-nlp/sup-simcse-bert-base-uncased

# Hoặc sử dụng model bạn đã train (ví dụ đường dẫn kết quả từ notebook)
python demo/flaskdemo.py --model_name_or_path result/my-sup-simcse-bert-base-uncased
3. Sử dụng
Sau khi server khởi động thành công (log hiện Starting Index server at http://127.0.0.1:8888), hãy mở trình duyệt và truy cập:

👉 http://localhost:8888

📚 Tham khảo
Dự án này dựa trên mã nguồn và nghiên cứu từ:

SimCSE: Simple Contrastive Learning of Sentence Embeddings (Gao et al., EMNLP 2021)

GitHub: princeton-nlp/SimCSE

Nhóm thực hiện: [Tên của bạn/Nhóm của bạn]
