# Skript Tu Tiên + ImmortalCultivation

Repository này cung cấp một script **Skript chủ đề tu tiên** cho server Minecraft (Spigot/Paper), có thể **kết hợp với plugin ImmortalCultivation** thông qua các command hook.

## Tính năng

File `skript-plugin/basic_plugin.sk` bao gồm:

- Hệ thống **cảnh giới**: `Phàm Nhân -> Luyện Khí -> Trúc Cơ -> Kim Đan -> Nguyên Anh`
- Biến **linh lực** theo từng người chơi
- Lệnh `/tutien thongtin`: xem trạng thái tu luyện
- Lệnh `/tutien thientoa`: thiền tọa nhận linh lực (có cooldown)
- Lệnh `/tutien dotpha`: đột phá cảnh giới (tỉ lệ thành công 70%)
- Lệnh `/tutien dongbo`: đồng bộ tay sang ImmortalCultivation

## Kết hợp với ImmortalCultivation

Trong `options` của script có các dòng:

- `ic-enabled`: bật/tắt tích hợp (`true/false`)
- `ic-on-join-cmd`: command chạy khi người chơi vào server
- `ic-on-meditate-cmd`: command chạy khi thiền tọa
- `ic-on-breakthrough-cmd`: command chạy khi đột phá thành công hoặc đồng bộ tay

Placeholder hỗ trợ trong command hook:

- `%player%`: tên người chơi
- `%realm%`: cảnh giới
- `%power%`: linh lực hiện tại

> Lưu ý: mỗi bản ImmortalCultivation có thể khác command. Hãy đổi các dòng `ic-on-...-cmd` cho đúng command plugin bạn đang dùng.

## Cài đặt

1. Cài plugin Skript trên server.
2. (Khuyến nghị) Cài plugin ImmortalCultivation.
3. Copy file `skript-plugin/basic_plugin.sk` vào thư mục:
   - `plugins/Skript/scripts/`
4. Reload script bằng lệnh:
   - `/sk reload basic_plugin`
