- Trong thử thách thứ 2 này tôi cũng nhận được một file
- Chạy thử chương trình thì nó bắt chung ta nhập mã pin, để lấy flag

![image](https://user-images.githubusercontent.com/57956165/140954227-cafb67f4-e5ba-4a5c-bf55-58337caa7613.png)

- Kiểm tra nó là file: ELF 64 bit, tôi sử dụng ida pro 64 để load file lên

![image](https://user-images.githubusercontent.com/57956165/140954263-5874839c-d3f0-4cb5-b747-ef85307ed410.png)

- f5 để kiểm tra chương trình chính

![image](https://user-images.githubusercontent.com/57956165/140954296-d24fc7db-4bc5-4782-a8b6-bc2f49be58ef.png)

- Xem qua chúng ta thấy chuỗi nhập vào là mảng gồm 10 ký tự, sau đó nó sẽ chuyển từ string sang int (sử dụng hàm atoi), sau đó nó sẽ trải qua hàm function(v3) để xử lý, nếu kq == 8208 thì xuất ra flag, ngược lại thì sai

![image](https://user-images.githubusercontent.com/57956165/140954901-168832e1-a93d-46e5-bf93-bdd7dbdd910c.png)

![image](https://user-images.githubusercontent.com/57956165/140954911-021c765c-8022-448b-abaa-b5e1e3ad9780.png)

- Mã pin nhập vào chính là: 8208 ==> nhận được flag

![image](https://user-images.githubusercontent.com/57956165/140954977-522c5188-b678-45b9-8845-33b47810e209.png)
