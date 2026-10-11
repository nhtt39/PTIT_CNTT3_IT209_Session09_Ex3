# Session 09 - Exercise 3: Dockerfile

## 1. File index.html
Nội dung trang HTML:
<h1>Hello Docker Session 09!</h1>

## 2. File Dockerfile
Sử dụng image nginx:alpine và sao chép index.html vào thư mục web mặc định của Nginx.

## 3. Build Docker Image
Lệnh:
docker build -t my-html-app:v1 .

Image được tạo: my-html-app:v1

## 4. Khởi chạy container
Lệnh:
docker run -d -p 8081:80 --name html-app my-html-app:v1

## 5. Kiểm tra kết quả
Lệnh:
curl http://localhost:8081

Kết quả mong đợi:
<h1>Hello Docker Session 09!</h1>
