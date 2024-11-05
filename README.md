PHP
1. Bạn có thể mô tả kiến trúc ứng dụng PHP gần đây mà bạn đã làm việc không?
  - Trả lời: Kiến trúc thường gồm một framework PHP (ví dụ: Laravel) với cấu trúc MVC. Backend giao tiếp với cơ sở dữ liệu MySQL hoặc PostgreSQL, xử lý logic nghiệp vụ, và cung cấp API RESTful cho frontend.
2. Luồng Hoạt Động trong MVC
  - Người dùng gửi yêu cầu: Người dùng tương tác với giao diện (View), ví dụ bằng cách nhấn nút hoặc gửi biểu mẫu.
  - Controller xử lý yêu cầu: Controller nhận yêu cầu và xác định hành động cần thực hiện.
  - Model tương tác với dữ liệu: Controller có thể gọi Model để truy xuất hoặc cập nhật dữ liệu.
  - View nhận dữ liệu từ Model: Sau khi nhận được dữ liệu từ Model, Controller sẽ chuyển dữ liệu đó đến View.
  - Giao diện người dùng được cập nhật: View được render với dữ liệu mới và gửi phản hồi trở lại người dùng.
3. Sự khác biệt giữa include, require, include_once, và require_once trong PHP là gì?
 - Trả lời:
    + include: Nạp và thực thi nội dung của file, nếu lỗi sẽ tiếp tục thực thi.
    + require: Nạp và thực thi nội dung của file, nếu lỗi sẽ dừng thực thi.
    + include_once và require_once: Tương tự nhưng đảm bảo file chỉ được nạp một lần
4. PHP có hỗ trợ kiểu dữ liệu nào không? Hãy liệt kê một số kiểu dữ liệu thông dụng.
  - Trả lời: PHP hỗ trợ các kiểu: Integer, Float, String, Boolean, Array, Object, NULL, và Resource.
5. Giải thích OOP trong PHP. Bạn có thể nêu các nguyên lý chính không?
  - Trả lời: OOP gồm 4 nguyên lý: Đóng gói (Encapsulation), Kế thừa (Inheritance), Đa hình (Polymorphism), và Trừu tượng (Abstraction).
  - Một số khái niệm quan trọng trong OOP bao gồm:
      + Lớp (Class): Là một mô hình hoặc khuôn mẫu để tạo ra các đối tượng. Lớp định nghĩa các thuộc tính và phương thức mà các đối tượng của nó sẽ có.
        ```javascript
          class Animal {
            // Thuộc tính (properties)
            constructor(name, type) {
              this.name = name;
              this.type = type;
            }
          
            // Phương thức (methods)
            speak() {
              console.log(`${this.name} is making a noise.`);
            }
          }
        ```
      + Đối Tượng (Object): Là một thể hiện cụ thể của một lớp. Đối tượng có thể được tạo ra từ lớp và có thể có các thuộc tính và phương thức cụ thể.
        ```javascript
            // Tạo đối tượng từ lớp Animal
            const myPet = new Animal('Buddy', 'Dog');
            
            myPet.speak(); // In ra: Buddy is making a noise.
        ```
      + Thuộc Tính (Property): Là các dữ liệu mà mỗi đối tượng của một lớp có. Thuộc tính thường đặc trưng cho trạng thái của đối tượng.
      + Phương Thức (Method): Là các hành động mà đối tượng của một lớp có thể thực hiện. Phương thức thường đặc trưng cho hành vi của đối tượng.
      + Kế Thừa (Inheritance): Là khả năng một lớp con có thể kế thừa thuộc tính và phương thức từ một lớp cha.Kế thừa giúp tái sử dụng mã nguồn và tạo ra một cấu trúc phân cấp.
      + Đóng/Gói (Encapsulation): Là nguyên tắc đóng gói dữ liệu và phương thức liên quan vào một đối tượng, bảo vệ chúng khỏi sự truy cập từ bên ngoài.
      + Đa Hình (Polymorphism): Là khả năng một đối tượng có thể hiểu và thực hiện các phương thức theo nhiều cách khác nhau. Đa hình giúp giảm sự phức tạp và tăng tính linh hoạt của mã nguồn.
        ### Ví dụ về một lớp trong JavaScript:
        
6. Bạn có thể giải thích sự khác biệt giữa public, protected, và private trong lớp PHP không?
  - Trả lời:
    + public: Truy cập được ở mọi nơi.
    + protected: Truy cập được trong lớp và lớp con.
    + private: Chỉ truy cập được trong lớp hiện tại.
7. Bạn sử dụng công cụ nào để gỡ lỗi trong PHP? Hãy mô tả quy trình gỡ lỗi của bạn.
  - Trả lời: Sử dụng Xdebug để gỡ lỗi. Đặt breakpoint trong IDE (như PHPStorm) và theo dõi các biến qua từng dòng mã.
8. Sự khác biệt giữa == và === trong PHP là gì?
  - Trả lời: == so sánh giá trị mà không quan tâm kiểu dữ liệu, === so sánh cả giá trị và kiểu dữ liệu.
9. Giải thích về composer trong PHP và cách bạn quản lý các thư viện phụ thuộc của dự án.
  - Trả lời: composer là công cụ quản lý các gói phụ thuộc. Sử dụng file composer.json để khai báo và chạy composer install để cài đặt các gói.
10. Bạn đã bao giờ triển khai hệ thống RESTful API trong PHP chưa? Nếu có, hãy mô tả quy trình.
  - Trả lời: Xây dựng RESTful API bằng cách sử dụng Laravel hoặc Slim Framework. Thiết kế các route, xử lý yêu cầu qua controller, và trả về dữ liệu dưới dạng JSON.
11. Sự khác biệt giữa GET và POST trong HTTP là gì? Khi nào nên dùng từng loại?
  - Trả lời: GET để truy vấn dữ liệu (có thể được lưu trong URL), POST để gửi dữ liệu (an toàn hơn và không hiển thị trên URL).
12. Bạn xử lý dữ liệu từ một form HTML trong PHP như thế nào? Làm thế nào để bảo vệ dữ liệu đó khỏi các cuộc tấn công như XSS và SQL Injection?
  - Trả lời: Dùng htmlspecialchars() để chống XSS và sử dụng PDO với câu lệnh prepared statements để ngăn SQL Injection.
13. Mô tả cách bạn quản lý kết nối cơ sở dữ liệu trong PHP. Bạn thường sử dụng PDO hay MySQLi, và tại sao?
  - Trả lời: Thường sử dụng PDO vì nó hỗ trợ nhiều cơ sở dữ liệu và dễ dùng với prepared statements để bảo vệ khỏi SQL Injection.
14. Bạn có thể mô tả cách xử lý các session và cookie trong PHP không? Sự khác biệt giữa hai khái niệm này là gì?
  - Trả lời: Session lưu thông tin người dùng trên máy chủ, Cookie lưu trên trình duyệt của người dùng. Session thích hợp hơn khi cần bảo mật.
15. Giải thích về kỹ thuật caching trong PHP. Bạn đã bao giờ sử dụng Memcached hoặc Redis chưa?
  - Trả lời: Sử dụng caching để cải thiện hiệu suất. Đã sử dụng Redis để cache dữ liệu thường xuyên được truy cập.
16. Bạn đã làm việc với các phương thức xử lý lỗi trong PHP chưa? Mô tả cách bạn xử lý và log lỗi trong dự án.
  - Trả lời: Sử dụng try-catch để bắt lỗi, và log lỗi vào file thông qua Monolog hoặc công cụ logging khác.

Nâng cao php

1. Giải thích về khái niệm "Event Loop" trong PHP. Có điểm nào khác biệt giữa PHP và các ngôn ngữ khác (như JavaScript) trong việc xử lý bất đồng bộ không?
  - Câu trả lời: "Event Loop" là một mô hình điều phối xử lý bất đồng bộ, cho phép chương trình quản lý nhiều tác vụ đồng thời mà không cần tạo ra nhiều luồng hoặc quy trình.
2. Giải thích về các nguyên tắc SOLID và cách áp dụng chúng trong phát triển ứng dụng PHP. Bạn đã từng áp dụng những nguyên tắc này chưa?
  - Câu trả lời: Các nguyên tắc SOLID bao gồm:
    + S (Single Responsibility Principle): Mỗi lớp nên có một lý do duy nhất để thay đổi. Ví dụ, một lớp User nên chỉ xử lý các thông tin liên quan đến người dùng, không nên xử lý việc gửi email.
    + O (Open/Closed Principle): Các lớp nên mở cho việc mở rộng nhưng đóng cho việc sửa đổi. Tôi thường sử dụng interface và abstract class để cho phép các lớp con mở rộng chức năng mà không thay đổi lớp cha.
    + L (Liskov Substitution Principle): Các lớp con phải có thể thay thế lớp cha mà không làm hỏng ứng dụng. Điều này yêu cầu các phương thức trong lớp con phải hoạt động như kỳ vọng.
    + I (Interface Segregation Principle): Nên có nhiều interface nhỏ thay vì một interface lớn. Điều này giúp các lớp không phải thực hiện các phương thức mà chúng không cần thiết.
    + D (Dependency Inversion Principle): Các lớp cấp cao không nên phụ thuộc vào các lớp cấp thấp; cả hai nên phụ thuộc vào abstraction. Tôi áp dụng điều này thông qua Dependency Injection.
3. Hãy thảo luận về cách mà bạn có thể xây dựng một API RESTful trong PHP. Các tiêu chuẩn nào bạn theo dõi để đảm bảo rằng API của bạn dễ sử dụng và bảo trì?
    - Câu trả lời: Để xây dựng một API RESTful trong PHP, tôi sẽ bắt đầu bằng cách thiết kế các endpoint để thực hiện các thao tác CRUD (Create, Read, Update, Delete) cho tài nguyên của ứng dụng. Một ví dụ là sử dụng phương thức GET để lấy danh sách người dùng, POST để tạo người dùng mới, PUT để cập nhật thông tin người dùng và DELETE để xóa người dùng.
    - Các tiêu chuẩn mà tôi sẽ theo dõi bao gồm:
    + Sử dụng các phương thức HTTP đúng cách: Chọn phương thức phù hợp cho từng loại yêu cầu.
    + URL rõ ràng và có cấu trúc: Sử dụng danh từ để đại diện cho tài nguyên (ví dụ: /api/users).
    + Trả về mã trạng thái HTTP thích hợp: Sử dụng mã như 200 OK, 404 Not Found, 500 Internal Server Error để thông báo về tình trạng yêu cầu.
    + Cung cấp thông tin rõ ràng về lỗi: Đảm bảo thông điệp lỗi là dễ hiểu và có thể giúp người dùng khắc phục vấn đề.
    + Sử dụng định dạng JSON: Để dễ dàng trao đổi dữ liệu giữa client và server.

GIT:
1. Sự khác biệt giữa git fetch và git pull là gì?
  - git fetch tải về các thay đổi từ kho lưu trữ nhưng không gộp vào, còn git pull vừa tải về vừa gộp các thay đổi.
2. Làm thế nào để hoàn tác thay đổi chưa commit?
  - Dùng git checkout -- <file> để khôi phục, hoặc git reset để hoàn tác toàn bộ.
3. Cách tạo nhánh mới và chuyển sang nhánh đó?
  - git checkout -b <tên-nhánh>.
4. Rebase và merge khác nhau thế nào?
  - Merge kết hợp nhánh mà vẫn giữ lịch sử, rebase gộp các commit và tái tạo lịch sử.
5. Cách xóa nhánh cục bộ và từ xa?
  - Cục bộ: git branch -d <tên-nhánh>. Từ xa: git push origin --delete <tên-nhánh>.
6. Làm thế nào để sửa commit cuối cùng?
  - Dùng git commit --amend.
7. Cách giải quyết xung đột trong Git?
  - Sửa xung đột thủ công trong file, sau đó git add và git commit.
8. Làm thế nào để quay lại commit cũ?
  - git checkout <commit-id> để xem hoặc git reset --hard <commit-id> để quay lại.

SQL:
1. SQL là gì?
  - Câu trả lời: SQL (Structured Query Language) là ngôn ngữ tiêu chuẩn được sử dụng để quản lý và thao tác với cơ sở dữ liệu quan hệ. Nó cho phép người dùng thực hiện các thao tác như truy vấn, chèn, cập nhật và xóa dữ liệu, cũng như tạo và quản lý cấu trúc của cơ sở dữ liệu.

2. Sự khác biệt giữa INNER JOIN, LEFT JOIN và RIGHT JOIN là gì?
  - Câu trả lời:
      + INNER JOIN: Chỉ trả về các hàng có giá trị khớp trong cả hai bảng.
      + LEFT JOIN (hoặc LEFT OUTER JOIN): Trả về tất cả các hàng từ bảng bên trái và các hàng khớp từ bảng bên phải. Nếu không có khớp, giá trị từ bảng bên phải sẽ là NULL.
      + RIGHT JOIN (hoặc RIGHT OUTER JOIN): Trả về tất cả các hàng từ bảng bên phải và các hàng khớp từ bảng bên trái. Nếu không có khớp, giá trị từ bảng bên trái sẽ là NULL.
3. Giải thích khái niệm về khóa chính (Primary Key) và khóa ngoại (Foreign Key)?
  - Câu trả lời:
      + Khóa chính (Primary Key): Là một cột hoặc tập hợp các cột trong một bảng mà có giá trị duy nhất cho mỗi hàng. Nó không cho phép giá trị NULL và được sử dụng để xác định duy nhất một bản ghi trong bảng.
      + Khóa ngoại (Foreign Key): Là một cột hoặc tập hợp các cột trong một bảng dùng để tạo mối quan hệ với khóa chính của bảng khác. Khóa ngoại có thể cho phép giá trị NULL và giúp duy trì tính toàn vẹn của dữ liệu giữa các bảng.
4. Viết câu truy vấn SQL để lấy tất cả các bản ghi từ bảng employees có lương lớn hơn 50000.
  - Câu trả lời:
    + SELECT * FROM employees WHERE salary > 50000;
5. Làm thế nào để thêm một bản ghi mới vào bảng?
    - Câu trả lời: Để thêm một bản ghi mới vào bảng, bạn sử dụng câu lệnh INSERT INTO. Ví dụ, để thêm một nhân viên mới vào bảng employees:
      + INSERT INTO employees (name, position, salary) VALUES ('John Doe', 'Developer', 60000);
6. Giải thích các loại chỉ mục (Index) trong SQL và tại sao chúng quan trọng?
    - Câu trả lời: Chỉ mục là một cấu trúc dữ liệu giúp tăng tốc độ truy vấn trên một bảng. Có hai loại chỉ mục chính:
    - Chỉ mục đơn: Chỉ sử dụng cho một cột.
    - Chỉ mục đa cột: Sử dụng cho nhiều cột.
    - Chỉ mục giúp cải thiện hiệu suất tìm kiếm và truy vấn dữ liệu, nhưng cũng có thể làm giảm hiệu suất khi chèn, cập nhật hoặc xóa bản ghi vì cần phải cập nhật chỉ mục tương ứng.
7. Viết câu truy vấn để cập nhật thông tin lương của một nhân viên có ID = 1.
    - Câu trả lời:
       + UPDATE employees SET salary = 70000 WHERE id = 1;
8. Làm thế nào để xóa một bản ghi trong bảng?
    - Câu trả lời: Để xóa một bản ghi, bạn sử dụng câu lệnh DELETE. Ví dụ, để xóa một nhân viên có ID = 1:
      + DELETE FROM employees WHERE id = 1;
9. Giải thích về GROUP BY và HAVING.
    - Câu trả lời:
      + GROUP BY: Được sử dụng để nhóm các bản ghi có cùng giá trị trong một hoặc nhiều cột, thường đi kèm với các hàm tổng hợp như COUNT(), SUM(), AVG().
      + HAVING: Được sử dụng để lọc các nhóm được tạo bởi câu lệnh GROUP BY. Nó cho phép áp dụng điều kiện lên các nhóm, tương tự như WHERE, nhưng áp dụng cho các nhóm thay vì các bản ghi riêng lẻ.
