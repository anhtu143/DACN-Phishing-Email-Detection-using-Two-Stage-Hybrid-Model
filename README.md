PHÁT HIỆN EMAIL PHISHING BẰNG MACHINE LEARNING + DEEP LEARNING
1. Overview
Dự án tập trung nghiên cứu và xây dựng hệ thống tự động phát hiện email lừa đảo (phishing) bằng cách ứng dụng các kỹ thuật xử lý ngôn ngữ tự nhiên (NLP) và thuật toán học máy (Machine Learning). Hệ thống thực hiện phân loại văn bản để xác định email thuộc nhóm Phishing (Lừa đảo) hoặc Legitimate (Hợp lệ).

Phishing là một trong những vector tấn công phổ biến nhất trong an ninh mạng hiện nay. Việc phát hiện dựa trên nội dung văn bản giúp ngăn chặn các cuộc tấn công Social Engineering ngay từ giai đoạn đầu.

2. Project Objectives
Xây dựng quy trình xử lý dữ liệu (Pipeline) hoàn chỉnh từ dữ liệu thô đến mô hình dự đoán.

Nghiên cứu ảnh hưởng của tiền xử lý văn bản (Text Preprocessing) đối với độ chính xác của mô hình bảo mật.

So sánh hiệu suất giữa các thuật toán Machine Learning truyền thống và các hướng tiếp cận Deep Learning.

Tối ưu hóa mô hình dựa trên các chỉ số an toàn thông tin (giảm tỷ lệ bỏ sót cuộc tấn công).

3. Methodology and Architecture
3.1. Data Preprocessing
Quá trình xử lý dữ liệu thô được thực hiện nghiêm ngặt để giảm nhiễu (noise) và tăng chất lượng đặc trưng:

Lowercasing: Chuyển đổi toàn bộ văn bản về chữ thường.

Noise Removal: Loại bỏ các ký tự đặc biệt, chữ số và các thẻ HTML không cần thiết.

Tokenization: Phân tách văn bản thành các đơn vị từ đơn lẻ.

Stopwords Removal: Loại bỏ các từ dừng phổ biến (the, a, in, on...) bằng thư viện NLTK.

Stemming/Lemmatization: Đưa từ về dạng gốc để giảm kích thước vector không gian.

3.2. Feature Engineering
Chuyển đổi văn bản thành dạng số để mô hình có thể tính toán:

TF-IDF (Term Frequency - Inverse Document Frequency): Kỹ thuật trọng tâm giúp làm nổi bật các từ khóa mang tính đặc trưng của email lừa đảo (ví dụ: "verify", "urgent", "suspended") và giảm tầm quan trọng của các từ phổ biến.

Word Embeddings (đối với Deep Learning): Sử dụng các vector không gian để nắm bắt ngữ nghĩa của văn bản.

3.3. Model Selection
Hệ thống thử nghiệm và đánh giá trên các thuật toán:

Baseline Models: Naive Bayes, Logistic Regression.

Advanced Models: Support Vector Machine (SVM), Random Forest.

Deep Learning: Long Short-Term Memory (LSTM) hoặc GRU để xử lý dữ liệu dạng chuỗi văn bản phi cấu trúc.

4. Evaluation Metrics
Trong bài toán bảo mật, việc đánh giá không chỉ dựa trên Accuracy (Độ chính xác tổng quát) mà tập trung vào:

Precision: Tỷ lệ email được dự đoán là phishing thực sự là phishing.

Recall: Khả năng bắt được tối đa các cuộc tấn công, hạn chế việc để lọt email độc hại (False Negative).

F1-Score: Chỉ số cân bằng giữa Precision và Recall.

5. Technical Insights
Dữ liệu thô ban đầu ở định dạng .eml và .mbox cho phép trích xuất đặc trưng sâu hơn từ Header và Body.

Kết quả thực nghiệm cho thấy các đặc trưng từ nội dung (Text-based features) có khả năng phân loại hiệu quả cao với độ chính xác đạt trên 90% tùy vào tập dữ liệu.

Việc xử lý False Negative là ưu tiên hàng đầu để đảm bảo an toàn cho người dùng cuối.

6. Future Enhancements
Tích hợp mô hình Transformer (BERT, RoBERTa) để nâng cao khả năng hiểu ngữ cảnh của email.

Mở rộng phân tích các đặc trưng từ URL độc hại và tệp tin đính kèm (Attachments).

Triển khai hệ thống dưới dạng API phục vụ cho các ứng dụng thực tế hoặc Plugin trình duyệt.

7. References
Alhogail, A. et al. (2021). Applying machine learning and NLP to detect phishing email.

Fette et al. (2007). Learning to Detect Phishing Emails.

Thakur et al. (2023). Deep Learning-based Phishing Detection Review.

8. Author
Student: Đặng Lê Anh Tú

Major: Cybersecurity

University: Ho Chi Minh City University of Technology (HUTECH)
