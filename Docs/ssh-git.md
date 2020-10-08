# SSH Git

Với việc phải đăng nhập mật khẩu mỗi lần thực hiện push lên kho repo ta có cách đơn giản hơn để thực hiện việc đó.

* Tại máy ảo linux thực hiện tạo SSH keygen:

`ssh-keygen -o -t rsa -C "your@email.com"`

your@email.com: Là địa chỉ Email mà bạn thực hiện đặng nhập Github

![huydv](/image/Screenshot_3.png)
* Đầu tiên máy tính hỏi bạn muốn lưu key vào đâu (mặc định nó sẽ lưu vào `(/root/.ssh/`)
* Tiếp theo bạn sẽ phải nhập mật khẩu cho Keygen với những lần đăng nhập bằng keygen
* Thực hiện copy file `rsa.pub`

* Chuyển sang github.com của bạn

Chọn Setting:

![huydv](/image/Screenshot_4.png)

![huydv](/image/Screenshot_5.png)

Chọn **New SSH key**

![huydv](/image/Screenshot_6.png)

Điền thông tin:

![huydv](/image/Screenshot_7.png)

Add key.

## Thực hiện clone repo:

Copy link:

![huydv](/image/Screenshot_8.png)

Clone tại máy linux:

`git clone [link]`

Nhập password đã tạo cho key ở bên trên:

![huydv](/image/Screenshot_9.png)

test:

![huydv](/image/Screenshot_10.png)

![huydv](/image/Screenshot_11.png)

Lên repo kiểm tra:

Đã xuất hiện 
![huydv](/image/Screenshot_12.png)

Chúc các bạn thực hiện thành công. 
