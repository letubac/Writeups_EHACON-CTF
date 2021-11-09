- Thử thách thứ 3
- Chạy thử chương trình thì thấy nó bắt chúng ta nhập vào mã code

![image](https://user-images.githubusercontent.com/57956165/140960053-e4f6c32f-8c1d-469f-aad1-51ad838afb08.png)

- Kiểm tra nó alf file ELF 64 bit, tôi sử dụng ida pro 64 để load file lên

![image](https://user-images.githubusercontent.com/57956165/140959780-669b0622-6ab1-4fd0-9a42-96136fb8934c.png)

- f5 để xem chương trình chính 

![image](https://user-images.githubusercontent.com/57956165/140962102-203ffeec-b5a7-462e-97e7-d38afab70e32.png)

- Xem qua chương trình thì thấy nó bắt chúng ta nhập vào một chuỗi ký tự, sau đó nó sử dụng hàm atoi để chuyển 1 chuỗi thành 1 số nguyên và trừ đi 22153

![image](https://user-images.githubusercontent.com/57956165/140960498-e1b2ff07-4669-47bf-b914-ba85690d79cb.png)

- vì OLL được ký int64, cho nên để nhập đầu vào thứ 2 thì fd = 0. Như vậy tôi sẽ nhập 22153 để trừ đi 22153 và sau đó fd = 0 và tôi có thể nhập đầu vào thứ 2. 
- Bây giờ đầu vào thứ 2 chúng ta thấy buf sẽ nắm giữ để đi so sánh với chuỗi LEMMEIN, còn "\n" chính là ký tự Enter (xuống dòng)

![image](https://user-images.githubusercontent.com/57956165/140961856-4fe7aa21-aa58-4155-aa49-bbed6f143e63.png)

- Chạy chương trình và tôi đã nhận được flag

![image](https://user-images.githubusercontent.com/57956165/140961935-29c9ba45-6a83-4f91-8f62-082510101d50.png)

#Flag: EHACON{V_E_5_9_e_R}
