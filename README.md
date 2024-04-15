### B1: Tạo một tệp Dockerfile trong source web để xây dựng docker.

```
FROM nginx:alpine
COPY . /usr/share/nginx/html
```
![alt](https://i.upanh.org/2024/04/15/1c039bedc534d0b8e.png)

### B2: Sử dụng lệnh docker build -t reloj:tag . để xây dựng một hình ảnh Docker từ một Dockerfile và các tài nguyên liên quan. 
-t reloj:tag: Tùy chọn này được sử dụng để gán một thẻ (tag) cho hình ảnh Docker
```
docker build -t reloj:tag .
```
![alt](https://i.upanh.org/2024/04/15/23152bd63b8b5f566.png)

### B3: Dùng lệnh docker run -d -p 8080:80 reloj:tag để khởi chạy container từ hình ảnh mới tạo
```
docker run -d -p 8080:80 reloj:tag
```
![alt](https://i.upanh.org/2024/04/15/3c568db8366150cdd.png)
### B4: Container đã được them và khởi chạy thành công.
![alt](https://i.upanh.org/2024/04/15/41a7192a4a0be48c9.png)
### B5: Truy cập vào trang web vừa deploy bằng cách truy cập 
```
http://localhost:8080/ 
```
![alt](https://i.upanh.org/2024/04/15/5841a7d90feae1182.png)

### B5: Thành công

![alt](https://i.upanh.org/2024/04/15/6b91fa11f54bf596d.png)
