# (Bài tập tổng hợp) Hành Trình Xử Lý 1 Lỗi Cài Đặt Thật

## Phần 1: Googling đúng cách
### 1. Lý do Google trả về kết quả kém chất lượng.
- Google chỉ tìm theo đúng từng từ mình gõ.

### 2. Bóc tách lỗi ở mục 3a theo 3 thành phần cốt lõi:

| Thành phần | Nội dung bóc tách |
| :--- | :--- |
| Tên phần mềm / Hệ điều hành | Node.js / Windows 11 |
| Mã lỗi nguyên văn | 'npm' is not recognized as an internal or external command, operable program or batch file. |
| Thao tác đang làm | Mở Terminal kiểm tra phiên bản bằng lệnh `npm -v` sau khi cài đặt. |

### 3. 3 câu truy vấn Google** tối ưu, mỗi câu dùng 1 toán tử khác nhau:

- Giới hạn trong StackOverflow (`site:`):
  `site:stackoverflow.com "npm is not recognized" windows 11`
- Dùng ngoặc kép cho lỗi nguyên văn (`" "`): 
  `"npm is not recognized as an internal or external command" nodejs`
- Loại trừ bài viết cũ không liên quan (`-`):
  `npm is not recognized windows nodejs -windows-xp`

## Phần 2: Thẩm định StackOverflow


### 1. So sánh Câu trả lời A và B
* Câu trả lời A: Có tích xanh, 186 upvotes, mới (2 năm trước), khớp đúng tags `[node.js]`, `[windows]`, `[npm]`.
* Câu trả lời B: Không tích xanh, 2 upvotes, quá cũ (9 năm trước), sai tags `[windows-xp]`.

### 2. Lựa chọn & Cảnh báo "bẫy"
- Lựa chọn: Chọn A.
- Bẫy B: Hướng dẫn cài lại driver mạng cho Windows XP, làm theo sẽ gây hỏng hệ thống.

### 3. Quy trình 30 Giây Đọc lướt
1. Nhìn ngay Accepted Answer và Upvotes cao nhất.
2. Kiểm tra Tags hệ điều hành/phần mềm có khớp không.
3. Đọc thẳng vào giải pháp code/ngắn gọn, bỏ qua thảo luận dài dòng.
## Phần 3 – Hỏi AI đúng cách và nhận diện rủi ro

### 1. Prompt hoàn chỉnh (3 thành phần)
- Ngữ cảnh: Dùng Windows 11, mới cài Node.js, đã thêm đường dẫn vào biến môi trường PATH nhưng khi gõ lệnh vẫn bị lỗi.
- Lỗi nguyên văn: `'npm' is not recognized as an internal or external command, operable program or batch file.`
- Yêu cầu: Giải thích nguyên nhân gốc rễ và hướng dẫn các bước khắc phục tiếp theo.

### 2. Đánh giá lệnh của AI (`del /f /s /q C:\Windows\System32\*`)
- cực kỳ nguy hiểm, tuyệt đối không làm theo! Lệnh này xóa toàn bộ file hệ thống cốt lõi, làm sập hoàn toàn Windows.

### 3. Cách phản hồi / hỏi lại AI
- Từ chối lệnh xóa file hệ thống, yêu cầu AI đề xuất phương án an toàn khác.
## Phần 4 – Viết Bug Report chuẩn để nhờ hỗ trợ

### 1. Tin nhắn kém
> *"Thầy ơi máy em lỗi gõ npm không được, cứu với ạ!"*

### 2. Bug Report chuẩn
| Mảnh ghép | Nội dung |
| :--- | :--- |
| Context | Cài Node.js trên Windows 11, đã thêm đường dẫn vào PATH nhưng gõ lệnh vẫn lỗi. |
| Expected | Hiển thị số phiên bản npm. |
| Actual | Báo lỗi `'npm' is not recognized as an internal or external command...` |
| Log & Screenshot | Mã lỗi nguyên văn kèm ảnh chụp màn hình Terminal. |

### 3. Phím tắt & Lưu ý bảo mật
- Phím tắt chụp màn hình: `Windows + Shift + S`.
- Lưu ý bảo mật: Che thông tin cá nhân nhạy cảm trước khi gửi ảnh.
