# 📚 NHẮC NHỞ MỤC ĐÍCH HỌC TẬP - AIRGEDDON

> **Công cụ này được thiết kế cho mục đích giáo dục và nghiên cứu bảo mật hợp pháp.**

---

## ⚖️ CAM KẾT SỬ DỤNG HỢP PHÁP

```
╔════════════════════════════════════════════════════════════════════════╗
║                                                                      ║
║   TRƯỚC KHI SỬ DỤNG AIRGEDDON, BẠN PHẢI CAM KẾT:                  ║
║                                                                      ║
║   ✅ Chỉ test trên mạng WiFi bạn SỞ HỮU hoặc được ỦY QUYỀN         ║
║   ✅ Luôn có sự đồng ý bằng văn bản từ chủ sở hữu                   ║
║   ✅ Sử dụng trong môi trường lab/đào tạo được kiểm soát             ║
║   ✅ Tuân thủ pháp luật Việt Nam và quốc tế                         ║
║                                                                      ║
║   ❌ KHÔNG tấn công mạng người khác                                  ║
║   ❌ KHÔNG đánh cắp thông tin cá nhân                                ║
║   ❌ KHÔNG gây hại cho hệ thống                                       ║
║   ❌ KHÔNG sử dụng cho mục đích thương mại trái phép                 ║
║                                                                      ║
╚════════════════════════════════════════════════════════════════════════╝
```

---

## 🎯 MỤC ĐÍCH SỬ DỤNG HỢP PHÁP

### 1. Học tập và Nghiên cứu
```
📚 Hiểu cách thức hoạt động của WiFi security
📚 Nghiên cứu các lỗ hổng bảo mật phổ biến
📚 Học cách phòng chống tấn công mạng
📚 Chuẩn bị cho chứng chỉ bảo mật (CEH, OSCP, v.v.)
```

### 2. Audit Bảo mật
```
🔍 Kiểm tra bảo mật mạng WiFi của riêng bạn
🔍 Đánh giá độ mạnh của mật khẩu
🔍 Kiểm tra cấu hình router
🔍 Phát hiện thiết bị xâm nhập trái phép
```

### 3. Môi trường Lab
```
🧪 Tạo mạng test với router cũ
🧪 Sử dụng virtual AP trên Linux
🧪 Thiết lập lab bảo mật tại nhà
🧪 Thực hành trong môi trường kiểm soát
```

### 4. Đào tạo và Chứng chỉ
```
🎓 Chuẩn bị cho CEH (Certified Ethical Hacker)
🎓 Học tập OSCP (Offensive Security)
🎓 Thực hành cho CompTIA Security+
🎓 Nghiên cứu cho尚os Certified Wireless Security Administrator
```

---

## 🚫 CÁC HÀNH ĐỘNG BỊ CẤM

### Tấn công bất hợp pháp
```
⛔ Tấn công mạng WiFi của người khác
⛔ Đánh cắp mật khẩu trái phép
⛔ Giả mạo AP để lừa đảo
⛔ Gây hại cho hệ thống mạng
```

### Sử dụng trái phép
```
⛔ Thương mại hóa mà không có giấy phép
⛔ Chia sẻ kết quả tấn công bất hợp pháp
⛔ Sử dụng trong các hoạt động tội phạm
⛔ Vi phạm quyền riêng tư
```

---

## 📖 HƯỚNG DẪN THỰC HÀNH AN TOÀN

### Bước 1: Thiết lập môi trường Lab
```bash
# Chuẩn bị:
- 1 router WiFi cũ (không kết nối internet)
- 1 máy tính Linux hoặc Kali VM
- 1 card WiFi hỗ trợ monitor mode

# Thiết lập:
1. Reset router về factory settings
2. Tạo mạng WiFi test với tên rõ ràng (VD: "TEST-LAB-01")
3. Đặt mật khẩu đơn giản để thực hành crack
4. Không kết nối router với internet
```

### Bước 2: Thực hành Quét mạng
```bash
# Khởi động airgeddon
sudo bash airgeddon.sh

# Chọn giao diện WiFi
# Bật chế độ monitor
# Quét và xem kết quả

# Học cách đọc:
- BSSID: MAC address của AP
- ESSID: Tên mạng WiFi
- Channel: Kênh hoạt động
- Encryption: Loại mã hóa (WPA2, WEP, v.v.)
- Signal: Độ mạnh tín hiệu
```

### Bước 3: Thực hành Bắt Handshake
```bash
# Chọn mạng test
# Chọn "Capture handshake"
# Chọn "Deauth attack"
# Chờ client kết nối lại
# Bắt gói tin handshake

# Học về:
- 4-way handshake trong WPA2
- Tại sao cần bắt handshake
- Cách lưu và kiểm tra handshake
```

### Bước 4: Thực hành Cracking
```bash
# Sử dụng aircrack-ng
aircrack-ng -w /usr/share/wordlists/rockyou.txt handshake.cap

# Sử dụng hashcat (nhanh hơn)
hashcat -m 22000 handshake.hc22000 rockyou.txt

# Học về:
- Brute force vs Dictionary attack
- Rainbow table
- GPU acceleration
- Tại sao mật khẩu mạnh quan trọng
```

### Bước 5: Phân tích Kết quả
```
📊 Đánh giá:
- Mất bao lâu để crack?
- Tại sao mật khẩu yếu/mạnh?
- Cách cải thiện bảo mật?
- Bài học rút ra?
```

---

## 🔐 BÀI HỌC VỀ BẢO MẬT WiFi

### Mật khẩu Mạnh
```
✅ 12+ ký tự
✅ Kết hợp: HOA, thường, số, ký tự đặc biệt
✅ Không dùng thông tin cá nhân
✅ Đổi mật khẩu định kỳ
✅ Sử dụng WPA3 nếu có thể
```

### Cấu Hình Router
```
✅ Đổi tên admin mặc định
✅ Cập nhật firmware thường xuyên
✅ Tắt WPS nếu không cần
✅ Bật firewall
✅ Giới hạn địa chỉ MAC (không phải bảo mật tuyệt đối)
```

### Phát Hiện Xâm Nhập
```
🔍 Kiểm tra danh sách client kết nối
🔍 Theo dõi lưu lượng bất thường
🔍 Sử dụng IDS/IPS
🔍 Báo cáo sự cố
```

---

## 📚 TÀI LIỆU THAM KHẢO

### Official
- [Airgeddon GitHub Wiki](https://github.com/v1s1t0r1sh3r3/airgeddon/wiki)
- [Airgeddon Documentation](https://airgeddon.pro/)

### Bảo mật
- [OWASP WiFi Security Testing Guide](https://owasp.org/)
- [NIST WiFi Security Guidelines](https://csrc.nist.gov/)
- [WiFi Alliance Security](https://www.wi-fi.org/discover-wi-fi/security)

### Chứng chỉ
- [CEH Certification](https://www.eccouncil.org/programs/certified-ethical-hacker-ceh/)
- [OSCP Certification](https://www.offensive-security.com/pwk-oscp/)
- [CompTIA Security+](https://www.comptia.org/certifications/security)

### Tại Việt Nam
- [Nhà nước về An toàn thông tin](https://nstic.vn/)
- [Bộ TT&TT - An toàn thông tin](https://mic.gov.vn/)

---

## 🛡️ NGUYÊN TẮC ĐẠO ĐỨC HACKER

```
1. LUÔN được phép trước khi test
2. KHÔNG gây hại cho hệ thống
3. BÁO cáo lỗ hổng cho chủ sở hữu
4. KHÔNG chia sẻ thông tin trái phép
5. TUÂN thủ pháp luật
6. SỬ DỤNG kỹ năng vào mục đích tốt
7. TÔN TRỌNG quyền riêng tư
8. HỌC TẬP liên tục
```

---

## 📞 BÁO CÁO LỖ HỔNG

Nếu phát hiện lỗ hổng bảo mật:
```
1. KHÔNG exploit hoặc lạm dụng
2. Liên hệ chủ sở hữu hệ thống
3. Cung cấp thông tin chi tiết
4. Đợi xác nhận trước khi công bố
5. Tuân thủ Responsible Disclosure
```

---

## ✅ CHECKLIST TRƯỚC KHI SỬ DỤNG

```
□ Tôi hiểu đây là công cụ EDUCATIONAL
□ Tôi sẽ chỉ test trên mạng của riêng mình
□ Tôi có sự đồng ý từ chủ sở hữu (nếu test mạng khác)
□ Tôi tuân thủ pháp luật Việt Nam
□ Tôi sẽ không gây hại cho hệ thống
□ Tôi sẽ lưu trữ kết quả an toàn
□ Tôi sẽ xóa dữ liệu sau khi hoàn thành
□ Tôi hiểu hậu quả pháp lý nếu lạm dụng
```

---

**📝 Ghi chú: Sử dụng có trách nhiệm. Học hỏi và chia sẻ kiến thức để xây dựng cộng đồng mạng an toàn hơn.**

**🌐 Phiên bản tiếng Việt | Cập nhật: Tháng 9, 2026**
