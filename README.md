#  PHÁT HIỆN EMAIL PHISHING BẰNG MACHINE LEARNING + DEEP LEARNING [cite: 1]

##  1. Overview [cite: 1]
 Dự án tập trung nghiên cứu và xây dựng hệ thống tự động phát hiện email lừa đảo (phishing) bằng cách ứng dụng các kỹ thuật xử lý ngôn ngữ tự nhiên (NLP) và thuật toán học máy (Machine Learning)[cite: 1].  Hệ thống thực hiện phân loại văn bản để xác định email thuộc nhóm Phishing (Lừa đảo) hoặc Legitimate (Hợp lệ)[cite: 2]. 

 Phishing là một trong những vector tấn công phổ biến nhất trong an ninh mạng hiện nay[cite: 3].  Việc phát hiện dựa trên nội dung văn bản giúp ngăn chặn các cuộc tấn công Social Engineering ngay từ giai đoạn đầu[cite: 4].

---

##  2. Project Objectives [cite: 5]
*  **Xây dựng quy trình**: Thiết lập pipeline xử lý dữ liệu hoàn chỉnh từ dữ liệu thô đến mô hình dự đoán[cite: 5].
*  **Nghiên cứu tiền xử lý**: Đánh giá ảnh hưởng của Text Preprocessing đối với độ chính xác của mô hình[cite: 6].
*  **So sánh mô hình**: Đối chiếu hiệu suất giữa Machine Learning truyền thống và Deep Learning[cite: 7].
*  **Tối ưu hóa**: Cải thiện các chỉ số an toàn thông tin để giảm tỷ lệ bỏ sót cuộc tấn công[cite: 8].

---

##  3. Methodology and Architecture [cite: 9]

### 3.1.  Data Preprocessing [cite: 9]
 Quá trình xử lý dữ liệu thô được thực hiện nghiêm ngặt để giảm nhiễu (noise)[cite: 9]:
*  **Lowercasing**: Chuyển đổi toàn bộ văn bản về chữ thường[cite: 9].
*  **Noise Removal**: Loại bỏ ký tự đặc biệt, chữ số và thẻ HTML[cite: 10].
*  **Tokenization**: Phân tách văn bản thành các đơn vị từ đơn lẻ[cite: 11].
*  **Stopwords Removal**: Loại bỏ các từ dừng phổ biến bằng thư viện NLTK[cite: 12].
*  **Stemming/Lemmatization**: Đưa từ về dạng gốc để giảm kích thước vector[cite: 13].

### 3.2.  Feature Engineering [cite: 14]
*  **TF-IDF**: Làm nổi bật các từ khóa đặc trưng như "verify", "urgent", "suspended"[cite: 14].
*  **Word Embeddings**: Sử dụng vector không gian để nắm bắt ngữ nghĩa cho Deep Learning[cite: 15].

### 3.3.  Model Selection [cite: 16]
*  **Baseline Models**: Naive Bayes, Logistic Regression[cite: 16].
*  **Advanced Models**: Support Vector Machine (SVM), Random Forest[cite: 17].
*  **Deep Learning**: Sử dụng LSTM hoặc GRU cho dữ liệu văn bản phi cấu trúc[cite: 17].

---

##  4. Evaluation Metrics [cite: 18]
*  **Precision**: Tỷ lệ dự đoán đúng trong số các email được gán nhãn phishing[cite: 18].
*  **Recall**: Khả năng bắt được tối đa các cuộc tấn công (giảm False Negative)[cite: 19].
*  **F1-Score**: Chỉ số cân bằng giữa Precision và Recall[cite: 20].

---

## 5. Technical Insights
*  **Dữ liệu thô**: Sử dụng định dạng .eml và .mbox để trích xuất đặc trưng từ Header và Body[cite: 20].
*  **Hiệu suất**: Đặc trưng nội dung (Text-based) giúp đạt độ chính xác trên 90%[cite: 21].
*  **Ưu tiên bảo mật**: Xử lý False Negative là ưu tiên hàng đầu để bảo vệ người dùng[cite: 22].

---

##  6. Future Enhancements [cite: 23]
*  Tích hợp mô hình Transformer (BERT, RoBERTa)[cite: 23].
*  Mở rộng phân tích URL và tệp tin đính kèm (Attachments)[cite: 24].
*  Triển khai dưới dạng API hoặc Plugin trình duyệt[cite: 25].

---

##  7. References [cite: 26]
* Alhogail, A. et al. (2021).  Applying machine learning and NLP to detect phishing email[cite: 26].
* Fette et al. (2007).  Learning to Detect Phishing Emails[cite: 27].
* Thakur et al. (2023).  Deep Learning-based Phishing Detection Review[cite: 27].

---

##  8. Author [cite: 28]
*  **Student**: Đặng Lê Anh Tú [cite: 28]
*  **Major**: Cybersecurity [cite: 28]
*  **University**: Ho Chi Minh City University of Technology (HUTECH) [cite: 28]
