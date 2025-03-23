
GD1:
-Java: 	+Các kiến thức cơ bản về Java 
	+JDBC
-MySQL	+Các câu lệnh và cách dùng cơ bản
-MongoDB cơ bản và cách kết nối với code bằng node.js

GD2:
1. Phân biệt OLTP vs OLAP
-OLTP (Online Transaction Processing:
Xử lý giao dịch nhanh, chính xác.
Dữ liệu cập nhật liên tục, dùng trong ngân hàng, thương mại điện tử.
Thiết kế Normalized (ít trùng lặp, tối ưu ghi).
Người dùng: khách hàng, nhân viên.

OLAP (Online Analytical Processing):
Phân tích dữ liệu lớn, hỗ trợ ra quyết định.
Tổng hợp dữ liệu từ nhiều nguồn, dùng trong báo cáo doanh thu, BI.
Thiết kế Denormalized (tối ưu truy vấn nhanh).
Người dùng: nhà phân tích, quản lý.

3. ETL (Extract - Transform - Load) vs ELT (Extract - Load - Transform)
ETL:
Trích xuất → Biến đổi → Tải vào.
Làm sạch dữ liệu trước khi lưu, đảm bảo chất lượng.
Dùng cho hệ thống truyền thống (ngân hàng, tài chính).

ELT:
Trích xuất → Tải vào → Biến đổi.
Tải dữ liệu thô trước, xử lý sau khi cần.
Phù hợp với Big Data, Data Lake (Hadoop, Snowflake).
