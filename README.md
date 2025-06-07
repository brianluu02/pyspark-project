## 📘 Project Overview: Online Banking Analysis
🔹 Tổng quan:
Dự án này là lần đầu tiên nhóm chúng tôi triển khai quy trình phân tích dữ liệu ngân hàng trực tuyến bằng Apache Spark và hệ sinh thái Big Data. Chúng tôi đã tải xuống và xử lý 3 tập dữ liệu từ Kaggle: loan, credit card, và transaction.

Sau bước làm sạch dữ liệu, nhóm đã xây dựng pipeline xử lý dữ liệu lớn bằng Spark, Hive, HDFS, và các công cụ hiện đại khác. Việc triển khai các use case được thực hiện trong môi trường Jupyter Notebook sử dụng PySpark.

## 🔹 Quy trình xử lý:
Data Ingestion:
- Tập dữ liệu từ Kaggle.
Data Processing:
- Làm sạch và chuẩn hóa dữ liệu trong 
- Thực hiện các truy vấn phân tích
Data Analysis:
Phân tích sâu bằng PySpark trong Jupyter Notebook.
Áp dụng các use case cụ thể cho từng dataset.
    1. 💼 Loan Dataset (Dữ liệu khoản vay)
📄 File: loan.csv

📌 Phân tích thực hiện:
Số lượng khoản vay theo loại khoản vay: housing, shopping, gold loan, v.v.

Thống kê số người vay trên 1 lakh (₹100,000).

Xác định người có thu nhập cao (> ₹60,000) và mối quan hệ với các yếu tố rủi ro:

Có lịch sử trả séc (bounced checks).

Tình trạng độc thân hoặc không có người phụ thuộc.

Chi tiêu cao so với thu nhập.

Tính toán tỷ lệ trả nợ thành công / thất bại theo loại khoản vay.

💡 Mục tiêu khai thác:
Phát hiện rủi ro tín dụng tiềm ẩn:

Thu nhập thấp nhưng vay cao.

Lịch sử tín dụng kém.

Khoản vay vượt quá khả năng chi trả.

Hỗ trợ các hệ thống chấm điểm tín dụng và ra quyết định duyệt vay.

2. 💳 Credit Card Dataset (Dữ liệu thẻ tín dụng)
📄 File: credit_card.csv

📌 Phân tích thực hiện:
Khách hàng có điểm tín dụng tốt (credit score > 700).

Khách hàng đủ điều kiện mở thẻ nhưng vẫn đang hoạt động trong hệ thống.

Phân bố khách hàng theo địa lý (ví dụ: Spain, Germany, France).

Khách hàng có thu nhập cao nhưng đã rời bỏ ngân hàng (customer churn).

Mối quan hệ giữa điểm tín dụng - lương - tình trạng khách hàng (hoạt động hoặc exited).

💡 Mục tiêu khai thác:
Xác định khách hàng tiềm năng (giữ lại, upsell, marketing).

Phân tích nguyên nhân rời bỏ ngân hàng.

Tạo mô hình phân khúc khách hàng theo vùng, tuổi, giới tính và điểm tín dụng.

3. 💰 Transaction Dataset (Dữ liệu giao dịch)
📄 File: txn.csv

📌 Phân tích thực hiện:
Tổng số lượng giao dịch theo từng tài khoản.

Giao dịch rút tiền lớn nhất, nhỏ nhất.

Giao dịch gửi tiền lớn nhất theo tài khoản.

Phân tích loại giao dịch phổ biến (withdrawal, deposit, payment).

Xác định tài khoản có biến động giao dịch bất thường.

💡 Mục tiêu khai thác:
Phân tích hành vi sử dụng tài khoản.

Nhận diện tài khoản có dấu hiệu gian lận hoặc rửa tiền.

Hỗ trợ hệ thống giám sát giao dịch trong ngân hàng.


⚙️ Technologies Used
Apache Spark & Spark SQL – Xử lý dữ liệu phân tán.

Hive – Lưu trữ và truy vấn dữ liệu dạng bảng.

Jupyter Notebook – Môi trường phân tích dữ liệu tương tác.

Power BI – Trực quan hóa dữ liệu cuối cùng.
