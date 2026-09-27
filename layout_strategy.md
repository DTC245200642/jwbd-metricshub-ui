# Báo cáo Giải trình Kiến trúc Layout - MetricsHub

1. **Navbar (Flexbox):** Chuyển từ Grid cứng nhắc sang Flexbox giúp các mục menu tự động co giãn linh hoạt theo chiều ngang (content-first), giải quyết triệt để lỗi tràn chữ khi đổi sang ngôn ngữ dài (tiếng Đức).
2. **Dashboard (CSS Grid):** Loại bỏ hoàn toàn cấu trúc "Div Soup" và các thẻ cột trung gian thừa thãi. Sử dụng CSS Grid trực tiếp với thuộc tính `span` giúp kiểm soát bố cục Bento Box 2 chiều (hàng và cột) trực quan, gọn gàng.
3. **Pricing (Bootstrap 5):** Tận dụng hệ thống Grid 12 cột sẵn có (`row`, `col-12`, `col-md-4`) của Bootstrap 5, loại bỏ hoàn toàn các đoạn code Media Queries thủ công và lệnh `float` lỗi thời.

*Kết luận:* **CSS Grid sinh ra để làm Layout tổng thể (2D), Flexbox sinh ra để làm Component chi tiết và căn chỉnh linh hoạt (1D).**