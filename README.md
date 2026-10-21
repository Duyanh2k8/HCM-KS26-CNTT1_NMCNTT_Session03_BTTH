# (Bài Tập Tổng Hợp) Kiến Trúc Hệ Điều Hành & Tư Duy Quản Lý File
## Phần 1 — Kiến trúc Hệ điều hành :
### 1.	Chức năng cốt lõi của hệ điều hành
Đây là chức năng quản lý tiến trình và quản lý tài nguyên. Hệ điều hành phân chia CPU, RAM và các tài nguyên khác cho Word, Chrome, VS Code và Portal để các phần mềm có thể chạy cùng lúc mà không ảnh hưởng quá nhiều đến nhau.
### 2.	Shell hay Kernel xử lý trước?
Khi double-click vào file báo cáo, người dùng tương tác trước với Shell, cụ thể là giao diện File Explorer của Windows. Shell tiếp nhận thao tác của người dùng, còn Kernel chịu trách nhiệm quản lý CPU, RAM và các hoạt động của hệ thống để thực hiện yêu cầu. Người dùng thường không tương tác trực tiếp với Kernel vì đây là phần cốt lõi, hoạt động ở mức hệ thống.
## Phần 2 — Cây thư mục & Ổ đĩa :
### 1.	Xác định thành phần trong cây thư mục
-	**Root Directory:** D:\
-	**Parent Directory:**
D:\Nam1\HocKy1\MonHoc\CongNgheThongTin\BaiTapLon\Session02\BaoCaoCuoiKy\Chuong1\Hinh anh\
-	**Vai trò của file:** anh 1.jpg là lá trong cây thư mục vì file không chứa các thư mục con.
### 2.	Vì sao không nên lưu dự án ở Desktop hoặc Downloads?
-	Thứ nhất, các thư mục này thường chứa nhiều file cá nhân và file tải về nên dễ bị nhầm lẫn hoặc xóa nhầm khi dọn dẹp.
-	Thứ hai, nếu ổ C bị lỗi hoặc cần cài lại Windows, dữ liệu trong User Profile có thể gặp rủi ro nếu chưa được sao lưu.
## Phần 3 — Đường dẫn Path :
### 1.	Absolute Path của file anh 1.jpg
D:\Nam1\HocKy1\MonHoc\CongNgheThongTin\BaiTapLon\Session02\BaoCaoCuoiKy\Chuong1\Hinh anh\anh 1.jpg
### 2.	Relative Path của file logo.png
- **Đường dẫn tương đối là:**
	assets/logo.png
- **Ví dụ chèn ảnh vào report.html:**
	<img src="assets/logo.png" alt="Logo dự án">
## Phần 4 — Quy tắc Đặt tên chuẩn :
- **Tên file ban đầu:**
	Báo cáo bài tập lớn IT101 (bản cuối) v2.docx
- **Tên file sau khi đổi sang kebab-case:**
	bao-cao-bai-tap-lon-it101-ban-cuoi-v2.docx
## Phần 5 — Tổ chức & Dọn dẹp Ổ đĩa
Đường dẫn cũ lồng tới 9 cấp, vi phạm nghiêm trọng "Quy tắc 3 cấp".

**Quy tắc 4 Trụ Cột & 3 Cấp:**
D:\01_HocTap\IT101\BaiTapLon\anh-1.jpg
-	Cấp 1 (Trụ cột): 01_HocTap
-	Cấp 2 (Môn): IT101
-	Cấp 3 (Nội dung): BaiTapLon
## Phần 6 — Đuôi file & File ẩn
**Cạm bẫy:** Đây là thủ đoạn giả mạo phần mở rộng kép của hacker. Vì máy đang tắt tính năng hiện đuôi file, bạn chỉ nhìn thấy phần tên do hacker cố tình đặt là de-thi-dap-an.pdf, khiến bạn tưởng đây là file tài liệu an toàn.

**Tên file thật có khả năng là:** de-thi-dap-an.pdf.exe

**Thao tác phát hiện sự thật:**
-	Mở File Explorer.
-	Chuyển sang tab View.
-	Đánh dấu tick vào ô File name extensions (Trên Windows 11: Chọn View > Show > File name extensions). Đuôi file thật sẽ lập tức hiện nguyên hình.
