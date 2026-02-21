# TuTien Advanced Skript (Full)

Bản này là phiên bản **nâng cấp full** theo yêu cầu, gồm:

- Hệ thống tu tiên cốt lõi (`/tutien`, `/dotpha`, thiền tọa, cảnh giới)
- Tích hợp **ImmortalCultivation** bằng hook command cấu hình được
- Hệ thống **/tuluyen** ngồi nhập định và cộng linh lực theo chu kỳ
- Hệ thống **Aura + GUI** (`/aura gui`)
- Hệ thống **Đạo lữ** (`/marry`, `/divorce`, chat riêng đạo lữ)
- Lệnh **admin** (`/tutien-admin`, `/tutien-reset`)
- PlaceholderAPI cho `exp`, `maxexp`, `realm`, `daolu`

## Cài đặt

1. Cài plugin Skript (và addon cần thiết nếu bạn dùng particle nâng cao/nbt/placeholderapi).
2. (Tuỳ chọn) Cài plugin ImmortalCultivation.
3. Copy file `skript-plugin/basic_plugin.sk` vào:
   - `plugins/Skript/scripts/`
4. Reload:
   - `/sk reload basic_plugin`

## Các lệnh chính

- `/tutien thongtin|thientoa|dotpha|dongbo|top`
- `/dotpha`
- `/tuluyen`
- `/aura gui|smoke|flame|cloud|water|snow|clear`
- `/marry ask|accept|decline|chat`
- `/divorce`
- `/tutien-admin ...` (admin)
- `/tutien-reset <player>` (admin)

## ImmortalCultivation hook

Trong `options`:

- `ic-enabled`
- `ic-on-join-cmd`
- `ic-on-meditate-cmd`
- `ic-on-breakthrough-cmd`

Placeholder trong command hook:

- `%player%`
- `%realm%`
- `%power%`

> Nếu command IC của server bạn khác, chỉ cần sửa 3 dòng `ic-on-...-cmd`.
