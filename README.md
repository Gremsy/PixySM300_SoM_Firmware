# PixySM300_SoM_Firmware
## Cách sử dụng firmware cho Pixy-SM prototype 1:
### Chuẩn bị trước:
- Một thiết bị USB-TTL để đọc console của SoM 
- Thẻ nhớ chứa file firmware.

### Thao tác thực hiện: 
 * Sử dụng phần mềm nạp GremsyTool
  - Có hướng dẫn ở trong file Download của GremsyTool
 * Cài đặt bằng lệnh
  - Nối USB-TTL với 3 dây console của SoM. Bất nguồn M300 -> Màn hình làm việc -> Đăng nhập.
  - Giải nén file tải về, copy file upgrade.7z vào trong thẻ nhớ 
  - Bỏ thẻ nhớ vào khe SD của Pixy-SM300.
  - Check tình trạng của SoM đủ điều khiển để nạp.
	    tek_ota --status
  -> SoM ở trạng thái nạp được sẽ hiện dòng:
	  Current OTA state: Booted into normal mode 
  - Sử dụng lệnh dưới để flash firmware trong thẻ nhớ.
	  tek_ota --upgrade <path_to_file_upgrade.7z>
  - Sau khi nạp xong vô màn hình làm việc. Sử dụng dòng lệnh sau để kết thúc flashing.
	  tek_ota --success
  - Nhấn lệnh sau để SoM bắt đầu chạy payload tự động.
	  systemctl start gremsy-payload.service
	  systemctl enable gremsy-payload.service
	
