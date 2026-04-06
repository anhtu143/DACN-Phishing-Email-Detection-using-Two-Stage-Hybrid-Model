#  PHÁT HIỆN EMAIL PHISHING BẰNG MACHINE LEARNING + DEEP LEARNING  

##  1. Overview  
 Dự án tập trung nghiên cứu và xây dựng hệ thống tự động phát hiện email lừa đảo (phishing) bằng cách ứng dụng các kỹ thuật xử lý ngôn ngữ tự nhiên (NLP) và thuật toán học máy (Machine Learning) .  Hệ thống thực hiện phân loại văn bản để xác định email thuộc nhóm Phishing (Lừa đảo) hoặc Legitimate (Hợp lệ) . 

 Phishing là một trong những vector tấn công phổ biến nhất trong an ninh mạng hiện nay.  Việc phát hiện dựa trên nội dung văn bản giúp ngăn chặn các cuộc tấn công Social Engineering ngay từ giai đoạn đầu.

---

##  2. Project Objectives
*  **Xây dựng quy trình**: Thiết lập pipeline xử lý dữ liệu hoàn chỉnh từ dữ liệu thô đến mô hình dự đoán
*  **Nghiên cứu tiền xử lý**: Đánh giá ảnh hưởng của Text Preprocessing đối với độ chính xác của mô hình
*  **So sánh mô hình**: Đối chiếu hiệu suất giữa Machine Learning truyền thống và Deep Learning
*  **Tối ưu hóa**: Cải thiện các chỉ số an toàn thông tin để giảm tỷ lệ bỏ sót cuộc tấn công

---

##  3. Methodology and Architecture  

### 3.1.  Data Preprocessing  
 Quá trình xử lý dữ liệu thô được thực hiện nghiêm ngặt để giảm nhiễu (noise) :
*  **Lowercasing**: Chuyển đổi toàn bộ văn bản về chữ thường .
*  **Noise Removal**: Loại bỏ ký tự đặc biệt, chữ số và thẻ HTML.
*  **Tokenization**: Phân tách văn bản thành các đơn vị từ đơn lẻ
*  **Stopwords Removal**: Loại bỏ các từ dừng phổ biến bằng thư viện NLTK
*  **Stemming/Lemmatization**: Đưa từ về dạng gốc để giảm kích thước vector

### 3.2.  Feature Engineering 
*  **TF-IDF**: Làm nổi bật các từ khóa đặc trưng như "verify", "urgent", "suspended"
*  **Word Embeddings**: Sử dụng vector không gian để nắm bắt ngữ nghĩa cho Deep Learning.

### 3.3.  Model Selection 
*  **Baseline Models**: Naive Bayes, Logistic Regression
*  **Advanced Models**: Support Vector Machine (SVM), Random Forest.
*  **Deep Learning**: Sử dụng LSTM hoặc GRU cho dữ liệu văn bản phi cấu trúc

---

##  4. Evaluation Metrics 
*  **Precision**: Tỷ lệ dự đoán đúng trong số các email được gán nhãn phishing
*  **Recall**: Khả năng bắt được tối đa các cuộc tấn công (giảm False Negative)
*  **F1-Score**: Chỉ số cân bằng giữa Precision và Recall

---

## 5. Technical Insights
*  **Dữ liệu thô**: Sử dụng định dạng .eml và .mbox để trích xuất đặc trưng từ Header và Body
*  **Hiệu suất**: Đặc trưng nội dung (Text-based) giúp đạt độ chính xác trên 90%
*  **Ưu tiên bảo mật**: Xử lý False Negative là ưu tiên hàng đầu để bảo vệ người dùng

---

##  6. Future Enhancements 
*  Tích hợp mô hình Transformer (BERT, RoBERTa)
*  Mở rộng phân tích URL và tệp tin đính kèm (Attachments)
*  Triển khai dưới dạng API hoặc Plugin trình duyệt
---

##  7. References 
* Alhogail, A. et al. (2021).  Applying machine learning and NLP to detect phishing email
* Fette et al. (2007).  Learning to Detect Phishing Emails
* Thakur et al. (2023).  Deep Learning-based Phishing Detection Review

---

##  8. Author 
*  **Student**: Đặng Lê Anh Tú 
*  **Major**: Cybersecurity 
*  **University**: Ho Chi Minh City University of Technology (HUTECH) 
