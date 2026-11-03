1. Vấn đề là gì?
Trang mất 20 giây để tải; ảnh bản đồ có thể bị 404 nên không hiện, còn ảnh dung lượng lớn có thể làm trang tải chậm. Cần xem Waterfall để xác định gói tin nào thực sự gây chậm
2. Yêu cầu đề bài
Dùng Network để tìm lỗi 404 và tài nguyên tải lâu; sửa đường dẫn, nén ảnh, bật Browser Cache. Kiểm tra CSS và JavaScript quan trọng tải thành công trước khi giao diện hiển thị
3. Cách làm
1. Mở F12 tìm Network tìm Disable cache, tải lại trang. Xem cột Status, Size, Time và biểu đồ Waterfall để tìm request 404 hoặc ảnh tải lâu nhất
2. Sửa link 404, nén ảnh bản đồ và bật cache cho ảnh, CSS, JavaScript tĩnh. Kiểm tra CSS/JavaScript quan trọng trả 200 OK ở lần tải đầu
3. Bỏ chọn Disable cache rồi tải lại. Mã 304 Not Modified là tín hiệu tốt: trình duyệt dùng lại file đã lưu, máy chủ không phải gửi lại toàn bộ nội dung, nên tiết kiệm băng thông
