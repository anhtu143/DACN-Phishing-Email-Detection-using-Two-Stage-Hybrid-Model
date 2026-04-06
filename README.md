# [cite_start]PHÁT HIỆN EMAIL PHISHING BẰNG MACHINE LEARNING + DEEP LEARNING [cite: 1]

## [cite_start]1. Overview [cite: 1]
[cite_start]Dự án tập trung nghiên cứu và xây dựng hệ thống tự động phát hiện email lừa đảo (phishing) bằng cách ứng dụng các kỹ thuật xử lý ngôn ngữ tự nhiên (NLP) và thuật toán học máy (Machine Learning)[cite: 1]. [cite_start]Hệ thống thực hiện phân loại văn bản để xác định email thuộc nhóm Phishing (Lừa đảo) hoặc Legitimate (Hợp lệ)[cite: 2]. 

[cite_start]Phishing là một trong những vector tấn công phổ biến nhất trong an ninh mạng hiện nay[cite: 3]. [cite_start]Việc phát hiện dựa trên nội dung văn bản giúp ngăn chặn các cuộc tấn công Social Engineering ngay từ giai đoạn đầu[cite: 4].

---

## [cite_start]2. Project Objectives [cite: 5]
* [cite_start]**Xây dựng quy trình**: Thiết lập pipeline xử lý dữ liệu hoàn chỉnh từ dữ liệu thô đến mô hình dự đoán[cite: 5].
* [cite_start]**Nghiên cứu tiền xử lý**: Đánh giá ảnh hưởng của Text Preprocessing đối với độ chính xác của mô hình[cite: 6].
* [cite_start]**So sánh mô hình**: Đối chiếu hiệu suất giữa Machine Learning truyền thống và Deep Learning[cite: 7].
* [cite_start]**Tối ưu hóa**: Cải thiện các chỉ số an toàn thông tin để giảm tỷ lệ bỏ sót cuộc tấn công[cite: 8].

---

## [cite_start]3. Methodology and Architecture [cite: 9]

### 3.1. [cite_start]Data Preprocessing [cite: 9]
[cite_start]Quá trình xử lý dữ liệu thô được thực hiện nghiêm ngặt để giảm nhiễu (noise)[cite: 9]:
* [cite_start]**Lowercasing**: Chuyển đổi toàn bộ văn bản về chữ thường[cite: 9].
* [cite_start]**Noise Removal**: Loại bỏ ký tự đặc biệt, chữ số và thẻ HTML[cite: 10].
* [cite_start]**Tokenization**: Phân tách văn bản thành các đơn vị từ đơn lẻ[cite: 11].
* [cite_start]**Stopwords Removal**: Loại bỏ các từ dừng phổ biến bằng thư viện NLTK[cite: 12].
* [cite_start]**Stemming/Lemmatization**: Đưa từ về dạng gốc để giảm kích thước vector[cite: 13].

### 3.2. [cite_start]Feature Engineering [cite: 14]
* [cite_start]**TF-IDF**: Làm nổi bật các từ khóa đặc trưng như "verify", "urgent", "suspended"[cite: 14].
* [cite_start]**Word Embeddings**: Sử dụng vector không gian để nắm bắt ngữ nghĩa cho Deep Learning[cite: 15].

### 3.3. [cite_start]Model Selection [cite: 16]
* [cite_start]**Baseline Models**: Naive Bayes, Logistic Regression[cite: 16].
* [cite_start]**Advanced Models**: Support Vector Machine (SVM), Random Forest[cite: 17].
* [cite_start]**Deep Learning**: Sử dụng LSTM hoặc GRU cho dữ liệu văn bản phi cấu trúc[cite: 17].

---

## [cite_start]4. Evaluation Metrics [cite: 18]
* [cite_start]**Precision**: Tỷ lệ dự đoán đúng trong số các email được gán nhãn phishing[cite: 18].
* [cite_start]**Recall**: Khả năng bắt được tối đa các cuộc tấn công (giảm False Negative)[cite: 19].
* [cite_start]**F1-Score**: Chỉ số cân bằng giữa Precision và Recall[cite: 20].

---

## 5. Technical Insights
* [cite_start]**Dữ liệu thô**: Sử dụng định dạng .eml và .mbox để trích xuất đặc trưng từ Header và Body[cite: 20].
* [cite_start]**Hiệu suất**: Đặc trưng nội dung (Text-based) giúp đạt độ chính xác trên 90%[cite: 21].
* [cite_start]**Ưu tiên bảo mật**: Xử lý False Negative là ưu tiên hàng đầu để bảo vệ người dùng[cite: 22].

---

## [cite_start]6. Future Enhancements [cite: 23]
* [cite_start]Tích hợp mô hình Transformer (BERT, RoBERTa)[cite: 23].
* [cite_start]Mở rộng phân tích URL và tệp tin đính kèm (Attachments)[cite: 24].
* [cite_start]Triển khai dưới dạng API hoặc Plugin trình duyệt[cite: 25].

---

## [cite_start]7. References [cite: 26]
* Alhogail, A. et al. (2021). [cite_start]Applying machine learning and NLP to detect phishing email[cite: 26].
* Fette et al. (2007). [cite_start]Learning to Detect Phishing Emails[cite: 27].
* Thakur et al. (2023). [cite_start]Deep Learning-based Phishing Detection Review[cite: 27].

---

## [cite_start]8. Author [cite: 28]
* [cite_start]**Student**: Đặng Lê Anh Tú [cite: 28]
* [cite_start]**Major**: Cybersecurity [cite: 28]
* [cite_start]**University**: Ho Chi Minh City University of Technology (HUTECH) [cite: 28]
