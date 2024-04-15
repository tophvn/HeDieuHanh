### B1: Tạo một tệp Dockerfile trong source web để xây dựng docker.

```
FROM nginx:alpine
COPY . /usr/share/nginx/html
```
### B2: Sử dụng lệnh docker build -t reloj:tag . để xây dựng một hình ảnh Docker từ một Dockerfile và các tài nguyên liên quan. 
-t reloj:tag: Tùy chọn này được sử dụng để gán một thẻ (tag) cho hình ảnh Docker
```
docker build -t reloj:tag .
```
### B3: Dùng lệnh docker run -d -p 8080:80 reloj:tag để khởi chạy container từ hình ảnh mới tạo
```
docker run -d -p 8080:80 reloj:tag
```
### B4: Container đã được them và khởi chạy thành công.
### B5: Truy cập vào trang web vừa deploy bằng cách truy cập ``` http://localhost:8080/ ```
