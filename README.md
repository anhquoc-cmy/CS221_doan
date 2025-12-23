# README

## Giới thiệu

Thư mục này chứa mã nguồn và hướng dẫn huấn luyện 4 mô hình ngôn ngữ dựa trên các biến thể BERT và RoBERTa cho bài toán NLI (Natural Language Inference) sử dụng phương pháp supervised và unsupervised.

## Hướng dẫn train

# CS221 Đồ án: Huấn luyện và Demo Mô hình Ngôn ngữ cho NLI

Thư mục này chứa mã nguồn, hướng dẫn huấn luyện và demo cho 4 mô hình ngôn ngữ dựa trên các biến thể BERT và RoBERTa cho bài toán NLI (Natural Language Inference), sử dụng phương pháp học có giám sát (supervised) và không giám sát (unsupervised).

## Liên kết nhanh

- [Tổng quan](#tổng-quan)
- [Cài đặt môi trường](#cài-đặt-môi-trường)
- [Cấu trúc thư mục](#cấu-trúc-thư-mục)
- [Huấn luyện mô hình](#huấn-luyện-mô-hình)
- [Chạy Demo](#chạy-demo)
- [Kết quả và So sánh](#kết-quả-và-so-sánh)
- [Liên hệ](#liên-hệ)

## Tổng quan

Dự án này tập trung vào việc áp dụng và so sánh hiệu quả của các mô hình BERT và RoBERTa trong việc tạo ra các vector biểu diễn câu (sentence embeddings) thông qua bài toán NLI. Chúng tôi cung cấp các notebook để huấn luyện mô hình theo hai hướng tiếp cận:
* **Supervised**: Sử dụng dữ liệu có nhãn.
* **Unsupervised**: Sử dụng dữ liệu không nhãn.

## Cài đặt môi trường

Để chạy mã nguồn và demo, bạn cần cài đặt môi trường Python với các thư viện cần thiết.

### Yêu cầu hệ thống
* Python 3.7+
* Thư viện: `transformers`, `torch`, `scikit-learn`, `umap-learn`, `matplotlib`, `flask` (cho demo), `gradio` (cho demo).

### Cài đặt
Chạy lệnh sau để cài đặt tất cả các thư viện phụ thuộc:

```bash
pip install -r requirements.txt
