# Dự án Portfolio Cá Nhân - Nguyễn Minh Hiếu

## 1. Tên dự án
Portfolio cá nhân / Website giới thiệu bản thân - Nguyễn Minh Hiếu

## 2. Mô tả dự án
Dự án này là một trang web portfolio cá nhân được xây dựng bằng HTML, CSS và các tài nguyên tĩnh để giới thiệu thông tin cá nhân, kỹ năng, dự án tiêu biểu, cũng như các phương thức liên hệ. Trang web có thiết kế tối giản, hiện đại, dễ nhìn, thân thiện với màn hình di động và phù hợp để sử dụng như CV trực tuyến hoặc landing page cá nhân.

Mục tiêu của dự án:
- Giới thiệu thông tin cá nhân và chuyên môn.
- Trình bày kỹ năng kỹ thuật và kinh nghiệm làm việc.
- Hiển thị các dự án đã thực hiện.
- Tạo một kênh liên hệ nhanh chóng cho nhà tuyển dụng, khách hàng hoặc đối tác.

## 3. Chức năng
Website cung cấp các chức năng chính sau:
- Header và navigation điều hướng qua các section chính.
- Hero section giới thiệu bản thân với tên, vai trò và lời chào.
- Section kỹ năng: hiển thị các công nghệ và kỹ năng chính.
- Section dự án: trình bày các dự án tiêu biểu bằng thẻ card.
- Section liên hệ: cung cấp email, số điện thoại và các kênh liên hệ.
- Thiết kế responsive thích ứng với màn hình máy tính, tablet và điện thoại.
- Sử dụng HTML5 và CSS3 để tối ưu trải nghiệm người dùng.

## 4. Công nghệ sử dụng
- HTML5
- CSS3
- Flexbox và CSS Grid
- Responsive Web Design
- JavaScript cơ bản (nếu có bổ sung trong tương lai)
- Git & GitHub
- Hệ thống tĩnh không cần framework phức tạp

## 5. Yêu cầu môi trường
Để chạy dự án, bạn cần:
- Trình duyệt web: Chrome, Edge, Firefox, Safari
- Một máy tính có hệ điều hành Windows, macOS hoặc Linux
- Tùy chọn:
  - Python 3.x (để chạy local server đơn giản)
  - Node.js (nếu muốn dùng trình phục vụ tĩnh từ npm)
  - Docker (nếu muốn triển khai theo container)

## 6. Cấu trúc thư mục dự án
```text
nmhieu1999/
├── README.md
├── nmhhieu1999.html
├── styles.css
├── asset/
│   └── img/
│       ├── boomonline.web
│       ├── chuotchui.web
│       └── ...
└── ...
```

## 7. Cài đặt
### 7.1. Tải xuống dự án
Bạn có thể clone repository hoặc download file ZIP về máy:

```bash
git clone https://github.com/your-username/nmhieu1999.git
cd nmhieu1999
```

Nếu dự án đang ở local workspace, bạn chỉ cần mở thư mục chứa tệp HTML và CSS.

## 8. Cấu hình
Dự án là website tĩnh, nên cấu hình rất đơn giản:
- Không cần file `.env`.
- Không cần database.
- Chỉ cần đảm bảo các đường dẫn đến file CSS và hình ảnh là chính xác.
- Kiểm tra các đường dẫn trong file HTML như:

```html
<link rel="stylesheet" href="./styles.css" />
<img src="./asset/img/boomonline.web" alt="Ảnh minh họa dự án" />
```

Nếu bạn đổi tên file hoặc thư mục hình ảnh, cần cập nhật lại đường dẫn tương ứng.

## 9. Chạy thử dự án
### 9.1. Trên Windows
Mở PowerShell hoặc Command Prompt trong thư mục dự án:

```powershell
cd path\to\nmhieu1999
python -m http.server 8000
```

Sau đó mở trình duyệt và truy cập:

```text
http://localhost:8000/
```

Nếu máy chưa cài Python, bạn có thể mở file `nmhhieu1999.html` trực tiếp trong trình duyệt.

### 9.2. Trên macOS
Mở Terminal và chạy:

```bash
cd /path/to/nmhieu1999
python3 -m http.server 8000
```

Sau đó truy cập:

```text
http://localhost:8000/
```

### 9.3. Trên Linux
Mở Terminal và chạy:

```bash
cd /path/to/nmhieu1999
python3 -m http.server 8000
```

Khi server khởi động, mở trình duyệt và vào địa chỉ:

```text
http://localhost:8000/
```

### 9.4. Sử dụng Node.js (nếu đã cài)
Bạn có thể sử dụng một static server khác:

```bash
cd /path/to/nmhieu1999
npx serve .
```

Sau đó truy cập địa chỉ mà terminal hiển thị, thường là:

```text
http://localhost:3000/
```

### 9.5. Chạy bằng Docker
Nếu bạn muốn chạy bằng Docker, trước tiên cần tạo file `Dockerfile` trong thư mục gốc, ví dụ:

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

Sau đó chạy các lệnh sau:

```bash
docker build -t nmhieu1999-portfolio .
docker run -d -p 8080:80 --name nmhieu1999 nmhieu1999-portfolio
```

Mở trình duyệt tại:

```text
http://localhost:8080/
```

## 10. Kiểm tra và xác minh
Sau khi chạy dự án, hãy kiểm tra các yếu tố sau:
- Trang mở đúng và hiển thị đầy đủ nội dung.
- Các hình ảnh có tải thành công.
- Menu điều hướng hoạt động.
- Giao diện hiển thị đúng trên desktop và mobile.
- Liên kết liên hệ và các button điều hướng không bị lỗi.

## 11. Thông tin liên hệ
- Họ tên: Nguyễn Minh Hiếu
- Email: minhhieu192111@gmail.com
- Số điện thoại: 091.999.4953
- LinkedIn: linkedin.com/in/nguyenminhhieu
- GitHub: (nếu có, bạn có thể thêm liên kết thật của bạn)

## 12. Ghi chú
Dự án này là phiên bản portfolio tĩnh và dễ mở rộng. Nếu muốn nâng cấp, bạn có thể tích hợp thêm:
- Bảng điều khiển quản trị nội dung
- Danh mục dự án động
- Form liên hệ gửi email
- Animation, hiệu ứng chuyển động phức tạp hơn
- Tích hợp API và dữ liệu thực tế

## 13. License
Dự án này đang được sử dụng cho mục đích cá nhân và học tập. Nếu bạn muốn sử dụng lại cho mục đích thương mại hoặc chia sẻ công khai, vui lòng liên hệ tác giả để được cấp phép phù hợp.

---

Nếu bạn muốn, tôi có thể tiếp tục viết thêm phiên bản README chuyên nghiệp hơn theo kiểu GitHub chuẩn, bao gồm badges, phần Features, Tech Stack, project structure, installation, usage, screenshots, và contact section phù hợp để đăng lên GitHub.
