# Dev Quest

App theo dõi việc tự học lập trình: lịch trong ngày có bộ đếm giờ, phiên học tính điểm theo phút, chuỗi ngày, cửa hàng game. Chạy hoàn toàn trên trình duyệt (PWA), không cần server.

## Chạy thử
Mở `index.html` bằng trình duyệt, hoặc chạy `python3 -m http.server` trong thư mục này rồi vào http://localhost:8000.

## Đưa lên GitHub và dùng trên điện thoại
1. Tạo repo mới, commit toàn bộ file trong thư mục này.
2. Vào Settings → Pages → chọn nhánh `main`, thư mục `/ (root)`.
3. Mở đường link GitHub Pages trên điện thoại, chọn "Thêm vào màn hình chính".

## Chuyển dữ liệu từ trang Claude
1. Ở trang Claude cũ, bấm "Xuất", sao chép JSON.
2. Ở app này, dán vào ô "Xuất / nhập dữ liệu" rồi bấm "Nhập" (hoặc chọn file .json).

## Lưu ý
- Dữ liệu lưu trong localStorage của từng trình duyệt. Điện thoại và PC chưa tự đồng bộ: dùng Xuất/Nhập để chuyển.
- Phiên học đang là chế độ tự giác (đồng hồ). Chưa có kiểm tra bằng AI.

## Hướng phát triển
- Extension VS Code và trình duyệt gửi "nhịp tim" hoạt động (chỉ tính phút có gõ phím hoặc thao tác thật, bỏ qua lúc AFK).
- Backend nhỏ (Supabase hoặc Firebase) để PC và điện thoại tự đồng bộ.
- Tùy chọn: kiểm tra bằng AI qua API key đặt ở server.
