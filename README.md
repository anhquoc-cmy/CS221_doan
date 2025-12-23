# README

## Giới thiệu

Thư mục này chứa mã nguồn và hướng dẫn huấn luyện 4 mô hình ngôn ngữ dựa trên các biến thể BERT và RoBERTa cho bài toán NLI (Natural Language Inference) sử dụng phương pháp supervised và unsupervised.

## Cấu trúc thư mục

- `code/`
  - `sup_bert.ipynb`: Notebook huấn luyện mô hình BERT với dữ liệu có giám sát (supervised)
  - `sup_roberta.ipynb`: Notebook huấn luyện mô hình RoBERTa với dữ liệu có giám sát (supervised)
  - `unsup_bert.ipynb`: Notebook huấn luyện mô hình BERT với dữ liệu không giám sát (unsupervised)
  - `unsup_roberta.ipynb`: Notebook huấn luyện mô hình RoBERTa với dữ liệu không giám sát (unsupervised)
- `model1/`, `model2/`, `model3/`, `model4/`: Thư mục lưu trữ các checkpoint, cấu hình, và kết quả huấn luyện của từng mô hình.

## Hướng dẫn sử dụng

1. **Cài đặt môi trường**
   - Yêu cầu Python 3.7+ và các thư viện: `transformers`, `torch`, `scikit-learn`, `umap-learn`, `matplotlib`, ...
   - Cài đặt các thư viện cần thiết:
     ```bash
     pip install -r requirements.txt
     ```
     (Tạo file `requirements.txt` nếu chưa có)

2. **Huấn luyện mô hình**
   - Mở từng notebook trong thư mục `code/` bằng Jupyter Notebook hoặc JupyterLab.
   - Chạy tuần tự các cell để huấn luyện mô hình tương ứng.
   - Kết quả và checkpoint sẽ được lưu trong các thư mục `model1/`, `model2/`, ...

3. **So sánh embedding**
   - Các file HTML như `embedding_comparison_tsne.html`, `embedding_comparison_umap.html` dùng để trực quan hóa và so sánh embedding của các mô hình.

## Ghi chú
- Các file `config.json`, `tokenizer_config.json`, ... trong thư mục model là cấu hình và trạng thái của mô hình sau khi huấn luyện.
- Có thể cần điều chỉnh đường dẫn dữ liệu hoặc tham số huấn luyện trong các notebook cho phù hợp với môi trường của bạn.

## Liên hệ
Nếu có thắc mắc hoặc cần hỗ trợ, vui lòng liên hệ tác giả dự án.
