# Test Cases – FIT4012 Lab 2

## Caesar Cipher
- [x] Encrypt `I LOVE YOU` với key `3` → `L ORYH BRX`
- [x] Encrypt `hello world` với key `5` → `mjqqt btwqi`
- [x] Decrypt `LORYH BRX` với key `3` → `ILOVE YOU`

## Rail Fence Cipher
- [x] Encrypt `I LOVE YOU` với `2` rails → `I OEOULV Y`
- [x] Encrypt `I LOVE YOU` với `4` rails → `I OYLV UOE`
- [x] Decrypt bản mã `I OEOULV Y` với `2` rails → `I LOVE YOU`

## Validation / File input
- [x] Kiểm tra đầu vào không hợp lệ (`HELLO123`) → báo lỗi hợp lệ
- [x] Đọc thông điệp từ `data/input.txt` → chương trình đọc và mã hóa thành công
