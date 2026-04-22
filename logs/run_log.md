# Run Log – FIT4012 Lab 2

## Caesar Cipher
- [x] Đã chạy Caesar encrypt với `I LOVE YOU`, key `3` → `L ORYH BRX`
- [x] Đã chạy Caesar encrypt với `hello world`, key `5` → `mjqqt btwqi`
- [x] Đã chạy Caesar decrypt với `LORYH BRX`, key `3` → `ILOVE YOU`

## Rail Fence Cipher
- [x] Đã chạy Rail Fence encrypt với `2` rails cho `I LOVE YOU` → `I OEOULV Y`
- [x] Đã chạy Rail Fence encrypt với `4` rails cho `I LOVE YOU` → `I OYLV UOE`
- [x] Đã chạy Rail Fence decrypt với `I OEOULV Y`, `2` rails → `I LOVE YOU`

## Validation / File input
- [x] Đã kiểm tra đầu vào không hợp lệ (`HELLO123`) → báo `Invalid input`
- [x] Đã đọc dữ liệu từ `data/input.txt` bằng chế độ `Read from file and encrypt`

## Điều em học được từ bài lab
Em hiểu rõ hơn cách dịch chuyển ký tự trong Caesar Cipher và xử lý vòng lặp chữ cái.
Với Rail Fence, em nắm được cách đi zigzag khi mã hóa và cách tái tạo pattern để giải mã.
Em cũng học được cách kiểm tra đầu vào để chương trình ổn định hơn.
Cuối cùng, em quen hơn với quy trình commit/push và kiểm tra tự động trên GitHub.
