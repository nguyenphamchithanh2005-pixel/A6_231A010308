NC2: Đếm số buổi đã chọn và hiện ngay dưới nhóm CheckBox.

Bổ sung TextView (tvSoBuoiDaChon) phía dưới các CheckBox trong file layout.

Khai báo một OnCheckedChangeListener dùng chung cho cả 3 CheckBox (cbSang, cbChieu, cbToi).

Viết hàm demSoBuoi() để đếm tổng số CheckBox đang được chọn (isChecked() == true) và cập nhật văn bản lên TextView theo thời gian thực. Gọi lại hàm này trong sự kiện nút Làm lại để reset số đếm về 0.

Kết quả test: Khi chọn/bỏ chọn từng buổi, TextView tự động cập nhật số lượng (0 -> 1 -> 2 ->  3) chính xác. Bấm Làm lại số đếm quay về 0.


NC3:SThêm MaterialSwitch (swDarkMode) vào giao diện XML.

Bắt sự kiện setOnCheckedChangeListener cho công tắc swDarkMode.

Sử dụng hàm AppCompatDelegate.setDefaultNightMode() truyền tham số MODE_NIGHT_YES (nếu bật) hoặc MODE_NIGHT_NO (nếu tắt) để chuyển đổi giao diện sáng/tối ngay lập tức.

Kết quả test: Khi gạt công tắc swDarkMode, toàn bộ nền và màu sắc ứng dụng chuyển sang Chế độ tối (Dark Mode) hoặc quay về Chế độ sáng mượt mà, không bị giật lag.witch "Chế độ tối" đổi nền màn hình ngay lập tức.
