# Report 1 Page – FIT4012 Lab 2

## 1. Mục tiêu
Mục tiêu của lab là cài đặt đầy đủ hai mã cổ điển Caesar và Rail Fence, bao gồm cả mã hóa và giải mã. 
Bên cạnh đó, chương trình cần xử lý chữ thường, giữ dấu cách, kiểm tra đầu vào hợp lệ, và đọc dữ liệu từ file theo yêu cầu đề bài. 
Cuối cùng là hoàn thiện quy trình kiểm thử, ghi log và nộp bài qua GitHub.

## 2. Cách làm
- Hoàn thiện Caesar Cipher cho chữ thường, dấu cách và giải mã.
- Hoàn thiện Rail Fence Cipher cho giải mã, giữ dấu cách, kiểm tra đầu vào và đọc file.
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Caesar Cipher
| Input | Key | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 3 | `L ORYH BRX` | Giữ nguyên dấu cách, dịch đúng 3 ký tự. |
| hello world | 5 | `mjqqt btwqi` | Hỗ trợ chữ thường đúng yêu cầu Q1. |
| LORYH BRX | 3 | `ILOVE YOU` | Giải mã Caesar hoạt động đúng cho Q3. |

### 3.2 Rail Fence Cipher
| Input | Rails | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 2 | `I OEOULV Y` | Mã hóa zigzag đúng với 2 rails. |
| I LOVE YOU | 4 | `I OYLV UOE` | Đã thử thay đổi rails theo Q4. |
| I OEOULV Y | 2 | `I LOVE YOU` | Giải mã Rail Fence đúng với Q5. |

### 3.3 Input validation / file input
- Trường hợp đầu vào không hợp lệ:
- Nhập `HELLO123` thì chương trình báo `Invalid input. Only letters and spaces are allowed.`
- Kết quả đọc từ `data/input.txt`:
- Chế độ `Read from file and encrypt` đọc được nội dung file và tạo bản mã thành công.

## 4. Kết luận
Qua lab này em hiểu rõ hơn cách hoạt động của hai thuật toán mã hóa cổ điển, đặc biệt là cơ chế dịch vòng của Caesar và pattern zigzag của Rail Fence.
Khó khăn lớn nhất là phần giải mã Rail Fence do phải tái tạo đúng mẫu đường ray theo chiều đi lên/xuống.
Việc viết test case, run log và dùng GitHub Actions giúp em kiểm tra bài có hệ thống hơn trước khi nộp.
