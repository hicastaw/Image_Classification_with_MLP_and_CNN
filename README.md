# 🧠 Image Classification: MLP vs. CNN

Đây là báo cáo dự án học sâu tập trung vào việc phân loại hình ảnh trên bộ dữ liệu **CIFAR-10**. Dự án này so sánh hiệu suất giữa hai kiến trúc mạng nơ-ron cơ bản: **Multi-Layer Perceptron (MLP)** và **Convolutional Neural Network (CNN)**.

## ✨ Tổng quan dự án

Mục tiêu chính là chứng minh sự vượt trội của CNN so với MLP trong các bài toán thị giác máy tính. Chúng tôi đã xây dựng, huấn luyện và đánh giá chi tiết cả hai mô hình, từ khâu chuẩn bị dữ liệu đến phân tích kết quả.

## 📈 Hiệu suất mô hình

Sau quá trình huấn luyện 20 epochs, kết quả cho thấy một sự khác biệt rõ rệt về hiệu suất:

- **MLP**: Đạt độ chính xác kiểm tra là **52.99%**. Mô hình này gặp khó khăn trong việc phân biệt các lớp có đặc điểm tương đồng do làm mất thông tin không gian của hình ảnh.
- **CNN**: Đạt độ chính xác kiểm tra ấn tượng **80.03%**. Hiệu suất vượt trội này đến từ khả năng của CNN trong việc tự động trích xuất các đặc trưng theo thứ bậc và tận dụng cấu trúc không gian của hình ảnh.

## 📊 So sánh trực quan

| Đặc điểm | MLP | CNN |
| :--- | :--- | :--- |
| **Kiến trúc** | Mạng kết nối đầy đủ (Fully Connected Network) | Tích chập và gộp (Convolutional & Pooling Layers) |
| **Xử lý hình ảnh** | Làm phẳng thành vector 1D (Mất thông tin không gian) | Xử lý trực tiếp 2D (Tận dụng cấu trúc không gian) |
| **Kết quả** | `52.99%` độ chính xác | `80.03%` độ chính xác |

## 🛠️ Công nghệ sử dụng

* **Python**
* **PyTorch** & **torchvision**
* **NumPy**
* **Matplotlib** & **Seaborn**
