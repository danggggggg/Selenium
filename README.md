Đây là một bài kiểm thử tự động hóa cho ứng dụng web OrangeHRM sử dụng Selenium WebDriver kết hợp với TestNG. Mục đích của bài kiểm thử là xác minh chức năng đăng nhập của hệ thống.

Mục đích

*Bài kiểm thử này thực hiện các bước sau:

1.Mở trang đăng nhập của OrangeHRM.
2.Nhập tên đăng nhập và mật khẩu vào các trường tương ứng.
3.Nhấn nút đăng nhập.
4.Kiểm tra nếu trang chuyển đến "Dashboard" sau khi đăng nhập thành công.

*Cấu hình môi trường
Để chạy bài kiểm thử này, ta cần chuẩn bị các bước sau:

1. Cài đặt Java:
Đảm bảo rằng Java Development Kit (JDK) đã được cài đặt trên máy tính . Có thể tải JDK từ Oracle's official website.

2. Cài đặt Maven:
Để quản lý các phụ thuộc và biên dịch dự án cần cài đặt Maven. Có thể tải Maven từ Maven's official website.

3. Cài đặt Selenium WebDriver và TestNG:
Đảm bảo đã thêm các phụ thuộc sau vào file pom.xml của Maven:
![image](https://github.com/user-attachments/assets/5d32d160-cf69-4291-a7de-d385fe35868b)

4. Cài đặt ChromeDriver:
   
![image](https://github.com/user-attachments/assets/aafeaa0c-aacf-4215-81e7-8711225b7df6)

*Chạy bài kiểm thử:

1.Run test

2.Kết quả:

Sau khi bài kiểm thử chạy, bạn sẽ thấy kết quả trong terminal. Nếu đăng nhập thành công và nội dung trang là "Dashboard", bài kiểm thử sẽ thành công.


![image](https://github.com/user-attachments/assets/0efd373b-bfc7-4272-9c84-03b039794288)


*Mô tả các phương thức trong bài kiểm thử:
1.@BeforeClass: Chạy trước tất cả các bài kiểm thử, khởi tạo trình duyệt và mở trang đăng nhập.

2.@AfterClass: Chạy sau tất cả các bài kiểm thử, đóng trình duyệt sau khi hoàn thành kiểm thử.

3.testLoginTestApplication(): Phương thức chính thực hiện kiểm tra đăng nhập. Nó nhập tên người dùng và mật khẩu vào các trường tương ứng, nhấn nút đăng nhập và xác minh kết quả là "Dashboard".

*Cấu trúc project:

![image](https://github.com/user-attachments/assets/8ef955ba-9f3a-45c1-870c-8f922ef31d02)


