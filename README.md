# Business-Intelligence-Application-for-Supply-Chain-Data-Analysis

**I. Introduction**
- Tổng quan: Đồ án môn học Business Intelligence, ứng dụng Business Intelligence (BI) để phân tích dữ liệu chuỗi cung ứng của DataCo Global (Raw data được lấy từ Kaggle). Mục tiêu của việc phân tích dữ liệu nhằm đánh giá hiệu suất kinh doanh hiện tại, phát hiện các vấn đề trong việc vận hành chuỗi cung ứng đặc biệt là khâu giao hàng, đồng thời đề xuất chiến lược dựa trên dữ liệu nhằm tối ưu chi phí, tăng trưởng doanh thu và cải thiện tỷ lệ giao hàng đúng hạn.
- Team size: 6
- Role taken: Leader

**II. Data**
- DataCo Smart Supply Chain for Big Data Analysis (Kaggle).
- Số bản ghi: 178,396 dòng
- Số thuộc tính: 53 cột, bao gồm thông tin về đơn hàng, sản phẩm, khách hàng, thị trường và vận chuyển.

**III. Approach**
- ETL Process: Thực hiện trích xuất, tiền xử lý và xây dựng mô hình dữ liệu dạng Snowflake schema trong Power BI.
  + Extract (Trích xuất): Thu thập dữ liệu gốc từ Kaggle.
  + Transform (Chuyển đổi): Làm sạch dữ liệu bằng Excel & Power BI (loại bỏ giá trị thiếu, trùng lặp, định dạng dữ liệu, tạo quan hệ).
  + Load (Nạp): Xây dựng mô hình dữ liệu Snowflake schema trong Power BI phục vụ phân tích.
- Data Visualization (Power BI Dashboards): Thiết kế dashboard trực quan theo các dimension quan tâm.
  + Tổng quan: Doanh thu, chi phí, lợi nhuận ròng, biên lợi nhuận, số lượng bán ra, mức giảm giá.
  + Theo thị trường: Hiệu suất kinh doanh theo châu lục, quốc gia, khu vực.
  + Theo khách hàng: Phân tích theo phân khúc khách hàng (Segment).
  + Theo sản phẩm: Doanh thu, chi phí và lợi nhuận theo danh mục sản phẩm.
  + Theo giao hàng: Tỷ lệ giao hàng đúng hạn vs trễ hạn.
  + Theo thời gian: Xu hướng hiệu suất kinh doanh qua năm, quý, tháng.
- Predictive Analytics: Ứng dụng các mô hình Machine Learning (Logistic Regression, Neural Network, Decision Tree, SVM) để dự báo rủi ro giao hàng trễ và đánh giá hiệu quả bằng AUC/F1-score thông qua Orange Data Mining.
Sử dụng bộ lọc để phân tích theo thị trường, khách hàng, sản phẩm.

Chạy mô hình dự báo để phân tích rủi ro giao hàng trễ.
