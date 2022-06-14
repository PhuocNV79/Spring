### `16 @ConfigurationProperties`

- Giả sử, ứng dụng của tôi sẽ yêu cầu có một số giá trị toàn cục, mà thay vì cấu hình ở trong code, tôi muốn lưu nó ở bên ngoài, để tiện thay đổi mỗi khi cần.
- Thì tôi sẽ làm như sau, tạo ra một class chứa các thông tin đó:
- ![image](https://user-images.githubusercontent.com/96764572/173467580-61bcb350-c6df-4a1d-ad45-b86e9cac1d65.png)

-`@PropertySource("classpath:loda.yml")` // Đánh dấu để lấy config từ trong file loda.yml
- `@ConfigurationProperties(prefix = "loda")` // Chỉ lấy các config có tiền tố là "loda"
- Sử dụng `@PropertySource` để định nghĩa tên của file config. Nếu không có annotation này, Spring sẽ sử dụng file mặc định (classpath:application.yml trong thư mục resources)
- `@ConfigurationProperties`, annotation này đánh dấu class bên dưới nó là properties, các thuộc tính sẽ được tự động nạp vào khi Spring khởi tạo.
- **Ngoài ra, để chạy được tính năng này, bạn cần kích hoạt nó bằng cách gắn `@EnableConfigurationProperties` lên một configuration nào đó. Ở đây tôi gắn lên hàm main luôn.**
- ![image](https://user-images.githubusercontent.com/96764572/173467246-ee9baeb9-b78a-4205-8397-b80c99b1d7f5.png)

#### Nested Properties
-Chúng ta có thể config các thuộc tính bên trong Class kể cả khi nó là Lists, Maps hay một class khác.
![image](https://user-images.githubusercontent.com/96764572/173468041-3a3960c7-cdd9-4e9d-a473-f775ae55e0a4.png)


