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


4. MongoDB
4.1. Giới thiệu MongoDB
-MongoDB là một hệ quản trị cơ sở dữ liệu NoSQL, sử dụng mô hình tài liệu (document-based) thay vì bảng như SQL.
-Lưu trữ dữ liệu dưới dạng JSON/BSON giúp linh hoạt trong xử lý dữ liệu không có cấu trúc cố định.
-Phù hợp với hệ thống yêu cầu mở rộng theo chiều ngang (horizontal scaling) như hệ thống phân tán.

4.2. Các thao tác cơ bản trong MongoDB
-CRUD (Create, Read, Update, Delete) với MongoDB:
+insertOne(), insertMany() để thêm tài liệu.
+find(), findOne() để truy vấn dữ liệu.
+updateOne(), updateMany() để cập nhật tài liệu.
+deleteOne(), deleteMany() để xóa tài liệu.
-Use case: Một ứng dụng mạng xã hội có thể sử dụng MongoDB để lưu trữ danh sách bài viết, bình luận, nơi dữ liệu có thể thay đổi linh hoạt theo từng bài đăng.

4.3. Cấu trúc dữ liệu trong MongoDB
-Cơ sở dữ liệu MongoDB chứa Collection (tương tự bảng trong SQL), mỗi Collection chứa Document (dữ liệu dạng JSON/BSON).
-Không có ràng buộc schema chặt chẽ, phù hợp với dữ liệu có cấu trúc động.
-Use case: Một ứng dụng thương mại điện tử có thể lưu thông tin sản phẩm trong MongoDB mà không cần cố định số lượng thuộc tính, giúp dễ dàng mở rộng dữ -liệu sản phẩm.

4.4. Chỉ mục (Index) trong MongoDB
-MongoDB hỗ trợ Index để tối ưu tốc độ truy vấn với createIndex().
-Các loại Index phổ biến:
+Single-field index (Chỉ mục trên một trường)
	+Chỉ mục trên một trường cụ thể giúp tối ưu tìm kiếm trên trường đó.
	+Ví dụ: db.users.createIndex({ username: 1 })
	+Use case:
		Một ứng dụng mạng xã hội có thể sử dụng chỉ mục trên username để tăng tốc tìm kiếm tài khoản người dùng.
		Một hệ thống thương mại điện tử có thể lập chỉ mục trên price để tối ưu lọc sản phẩm theo giá.
+Compound index (Chỉ mục trên nhiều trường)
	+Chỉ mục trên nhiều trường giúp tối ưu truy vấn kết hợp nhiều điều kiện.
	+Ví dụ: db.orders.createIndex({ userId: 1, createdAt: -1 })
	+Use case:
		Trong một trang web thương mại điện tử, nếu thường xuyên lọc đơn hàng theo userId và createdAt, thì chỉ mục này giúp tăng tốc truy vấn.
		Trong hệ thống quản lý nhân viên, có thể lập chỉ mục { department: 1, salary: -1 } để nhanh chóng tìm nhân viên theo phòng ban và lương 		giảm dần.
+Text index (Chỉ mục tìm kiếm văn bản)
	+Được sử dụng để tìm kiếm chuỗi văn bản, hỗ trợ tìm kiếm toàn văn (full-text search).
	+Ví dụ: db.articles.createIndex({ content: "text" })
	+Use case:
		Một blog hoặc hệ thống tin tức có thể sử dụng text index để tìm kiếm bài viết theo từ khóa.
		Một hệ thống thương mại điện tử có thể dùng text index để tìm kiếm sản phẩm theo mô tả.

4.5. Mô hình phân tán trong MongoDB
-Replication: Sao chép dữ liệu giữa nhiều node để đảm bảo dữ liệu luôn có sẵn.
-Sharding: Phân mảnh dữ liệu để tăng hiệu suất truy vấn trên tập dữ liệu lớn.
-Use case: Một hệ thống IoT thu thập dữ liệu từ hàng triệu cảm biến có thể sử dụng Sharding để phân tán dữ liệu theo vị trí địa lý.


5. Linux
5.1. Giới thiệu Linux
-Linux là một hệ điều hành mã nguồn mở, phổ biến trên server, cloud, và hệ thống nhúng.
-Cung cấp khả năng quản lý tài nguyên tốt, ổn định và bảo mật cao.
-Use case: Trong môi trường doanh nghiệp, Linux được sử dụng cho máy chủ web (Apache, Nginx), cơ sở dữ liệu (MySQL, PostgreSQL), và containerization (Docker, Kubernetes).

5.2. Các lệnh cơ bản trong Linux
-Quản lý file và thư mục: ls, cd, mkdir, rm, cp, mv
-Quản lý quyền truy cập: chmod, chown
-Quản lý tiến trình: ps, top, kill
-Use case: Trong môi trường DevOps, quản trị viên hệ thống sử dụng các lệnh này để quản lý file log, cấu hình server, và theo dõi hiệu suất hệ thống.

5.3. Hệ thống tập tin và phân quyền
-Linux sử dụng hệ thống tập tin dạng cây (/ root directory là thư mục gốc).
-Phân quyền theo User, Group, Others với các mức truy cập r (read), w (write), x (execute).
-Use case: Trong công ty, tài liệu nội bộ có thể bị giới hạn quyền truy cập chỉ cho nhóm nhân viên cụ thể bằng lệnh chmod.

5.4. Shell scripting trong Linux
-Viết script với bash để tự động hóa các công việc lặp lại.
-Ví dụ: Script kiểm tra dung lượng ổ đĩa và gửi cảnh báo nếu gần đầy.
-Use case: DevOps sử dụng Shell script để tự động hóa quá trình backup dữ liệu và khởi động lại dịch vụ khi gặp sự cố.

5.5. Quản lý tiến trình và dịch vụ trong Linux
-Kiểm tra tiến trình với ps, top, htop.
-Quản lý dịch vụ với systemctl (dành cho systemd) hoặc service.
-Use case: Quản trị viên sử dụng systemctl restart apache2 để khởi động lại web server khi xảy ra lỗi.

5.6. Mạng và bảo mật trong Linux
-Kiểm tra mạng với ifconfig, ip, ping, netstat, curl.
-Cấu hình tường lửa với iptables, ufw.
Use case: Trong công ty, firewall được cấu hình để chỉ cho phép kết nối từ địa chỉ IP nội bộ nhằm tăng cường bảo mật.
