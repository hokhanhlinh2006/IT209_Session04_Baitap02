# Báo cáo: Giải quyết xung đột (Merge Conflict)

## Bối cảnh
- Được yêu cầu tạo xung đột khi gộp nhánh `feature-update` vào nhánh `main`.
- Xung đột xảy ra tại file `README.md`.

## Các bước giải quyết xung đột thủ công
1. Mở file `README.md` bị lỗi xung đột (conflict).
2. Tìm đến các dòng đánh dấu xung đột (`<<<<<<< HEAD`, `=======`, `>>>>>>> feature-update`).
3. Xác định nội dung cần giữ lại từ cả hai nhánh, hoặc chỉnh sửa gộp chung.
4. Xóa bỏ các ký hiệu đánh dấu xung đột của Git.
5. Lưu file `README.md`.
6. Thực hiện lệnh `git add homework/session_04/ex2/README.md` để đánh dấu file đã được giải quyết xung đột.
7. Thực hiện lệnh `git commit -m "Merge branch 'feature-update'"` để hoàn thành 3-way merge.

## Hình ảnh lịch sử commit
Dưới đây là kết quả của lệnh `git log --graph --oneline`:

```text
*   104950d Merge branch 'feature-update'
|\  
| * 87d78dc Add feature update to README
* | 5eb8fea Update README in main
|/  
* cfec6b5 Initial commit
```
