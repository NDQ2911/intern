GD1:
1. Java
1.1. Giới thiệu Java
-Java là một ngôn ngữ lập trình hướng đối tượng, đa nền tảng, chạy trên JVM (Java Virtual Machine).
-Mạnh trong phát triển ứng dụng doanh nghiệp, ứng dụng web, Android, và hệ thống backend.

1.2. Cấu trúc cơ bản của một chương trình Java
-Cú pháp Java giống C/C++ nhưng có bộ quản lý bộ nhớ tự động (Garbage Collector).
-Một chương trình Java điển hình gồm:
	+Lớp (class) chứa thuộc tính và phương thức.
	+Phương thức main() là điểm khởi đầu của chương trình.

1.3. Các thành phần cơ bản trong Java
-Biến & kiểu dữ liệu: int, double, char, String, boolean, Array.
-Toán tử: Số học, quan hệ, logic, gán, điều kiện, bitwise.
-Cấu trúc điều kiện: if-else, switch-case.
-Vòng lặp: for, while, do-while, foreach.
-Mảng & danh sách (Array, ArrayList, LinkedList, HashMap, Set).

1.4. Lập trình hướng đối tượng (OOP)
4 tính chất OOP:
a.Đóng gói (Encapsulation)
-Khái niệm:	+Đóng gói là việc bảo vệ dữ liệu bằng cách ẩn các thuộc tính (biến) của một đối tượng và chỉ cho phép truy cập thông qua các phương thức cụ 		thể.
		+Sử dụng các mức truy cập (access modifiers) như private, protected, public để kiểm soát quyền truy cập vào dữ liệu.
-Ưu điểm:
	+Bảo mật dữ liệu: Không cho phép truy cập trực tiếp vào dữ liệu bên trong đối tượng.
	+Dễ bảo trì: Nếu cần thay đổi logic xử lý dữ liệu, chỉ cần sửa trong phương thức getter/setter mà không ảnh hưởng đến mã nguồn bên ngoài.

b.Kế thừa (Inheritance) 
-Khái niệm
	+Kế thừa cho phép một lớp (class con) tái sử dụng các thuộc tính và phương thức từ một lớp khác (class cha).
	+Lớp con có thể mở rộng (extend) hoặc ghi đè (override) phương thức của lớp cha.
	+Sử dụng từ khóa extends để kế thừa một lớp khác.
-Ưu điểm
	+Tái sử dụng mã nguồn, giúp tiết kiệm thời gian và công sức.
	+Tổ chức mã nguồn khoa học hơn, giúp dễ bảo trì và mở rộng.

c.Đa hình (Polymorphism) 
-Khái niệm
	+Đa hình cho phép một phương thức có thể có nhiều hình thái khác nhau.
	+Có hai loại đa hình trong Java:
	+Nạp chồng phương thức (Method Overloading) – cùng một tên phương thức nhưng khác tham số.
	+Ghi đè phương thức (Method Overriding) – lớp con định nghĩa lại phương thức của lớp cha.
-Ưu điểm
	+Giúp mã nguồn linh hoạt hơn: Cùng một tên phương thức nhưng có thể hoạt động theo nhiều cách khác nhau.
	+Dễ mở rộng chương trình: Lớp con có thể thay đổi cách hoạt động của phương thức mà không ảnh hưởng đến lớp cha.

d.Trừu tượng (Abstraction) 
-Khái niệm
	+Trừu tượng giúp ẩn đi những chi tiết không cần thiết và chỉ hiển thị những gì quan trọng.
	+Có hai cách thực hiện tính trừu tượng trong Java:
		Lớp trừu tượng (abstract class)
		Giao diện (interface)
-Ưu điểm
	+Giúp thiết kế chương trình tốt hơn, chỉ định rõ các phương thức cần có mà không quan tâm đến cách chúng được thực hiện.
	+Dễ mở rộng chương trình, các lớp khác nhau có thể triển khai cùng một giao diện theo cách riêng của chúng.

1.5. Xử lý ngoại lệ (Exception Handling)
-Dùng try-catch-finally để bắt và xử lý lỗi. Giúp chương trình không bị ngắt đột ngột khi gặp lỗi
-Các loại ngoại lệ phổ biến: NullPointerException, ArrayIndexOutOfBoundsException, IOException, SQLException.

1.6. Luồng I/O (Input/Output Streams)
-Làm việc với tệp tin: FileReader, FileWriter, BufferedReader, BufferedWriter.
-Đọc/ghi dữ liệu dạng nhị phân với ObjectInputStream, ObjectOutputStream.

1.7. Luồng (Thread) trong Java
-Xử lý đa luồng (Thread, Runnable).
-Đồng bộ hóa (synchronized, wait(), notify()).

1.8. JDBC - Kết nối Java với cơ sở dữ liệu
-JDBC (Java Database Connectivity) giúp Java làm việc với cơ sở dữ liệu.
-Các bước kết nối:
	+Tải driver JDBC (MySQL, PostgreSQL, Oracle).
	+Tạo kết nối với DriverManager.getConnection().
	+Thực thi truy vấn với Statement hoặc PreparedStatement.
	+Xử lý kết quả bằng ResultSet.
	+Đóng kết nối để tránh rò rỉ tài nguyên.
 
2. SQL (Structured Query Language)
2.1. Tổng quan về SQL
-Ngôn ngữ truy vấn cơ sở dữ liệu quan hệ (RDBMS).
-Được sử dụng trong MySQL, PostgreSQL, SQL Server, Oracle.

2.2. Các loại lệnh SQL
-DDL (Data Definition Language) – Định nghĩa dữ liệu:
+CREATE TABLE, ALTER TABLE, DROP TABLE, TRUNCATE TABLE.
-DML (Data Manipulation Language) – Quản lý dữ liệu:
+INSERT INTO, UPDATE, DELETE, SELECT.
-DCL (Data Control Language) – Phân quyền:
+GRANT, REVOKE.
-TCL (Transaction Control Language) – Quản lý giao dịch:
+COMMIT, ROLLBACK, SAVEPOINT.

2.3. Cấu trúc cơ sở dữ liệu quan hệ
-Bảng (Table) chứa các bản ghi (row) và cột (column).
-Khóa chính (Primary Key) đảm bảo mỗi bản ghi là duy nhất.
-Khóa ngoại (Foreign Key) tạo quan hệ giữa các bảng.

2.4. Tối ưu hóa truy vấn SQL
-Index giúp tăng tốc truy vấn (CREATE INDEX).
-EXPLAIN kiểm tra hiệu suất truy vấn.
-Chuẩn hóa dữ liệu (Normalization) giúp tránh dữ liệu trùng lặp.

3. Vận hành cơ sở dữ liệu
3.1. Hiểu cách hoạt động của cơ sở dữ liệu
-CSDL lưu trữ dữ liệu dưới dạng bảng với các mối quan hệ.
-Hệ thống RDBMS đảm bảo tính nhất quán và toàn vẹn dữ liệu.

3.2. Quản lý quyền truy cập và bảo mật
-Tạo người dùng (CREATE USER) và phân quyền (GRANT).
-Hạn chế truy cập với REVOKE.
-Sử dụng mã hóa để bảo vệ dữ liệu.

3.3. Backup & Restore cơ sở dữ liệu
-Backup dữ liệu bằng mysqldump:	mysqldump -u root -p database_name > backup.sql
-Khôi phục dữ liệu:		mysql -u root -p database_name < backup.sql

3.4. Giám sát và tối ưu hệ thống
-Theo dõi hiệu suất với SHOW PROCESSLIST, SHOW STATUS.
-Tối ưu hóa cấu trúc bảng với OPTIMIZE TABLE.
