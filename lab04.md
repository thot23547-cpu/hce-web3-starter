# Báo cáo Lab 4 - Nhận diện hợp đồng có rủi ro

## Bảng phân tích rủi ro hợp đồng
| Hợp đồng | Tên hàm | Số dòng | Rủi ro cho người nắm giữ token |
| :--- | :--- | :--- | :--- |
| **ClubTokenB** | `mint` | Dòng 16-18 | Chủ sở hữu có thể tùy ý phát hành thêm vô hạn token bất cứ lúc nào, gây rủi ro lạm phát và làm mất giá trị tài sản của người nắm giữ[cite: 8]. |
| **ClubTokenC** | `setRestricted` / `_update` | Dòng 22-35 | Chủ sở hữu có quyền đưa bất kỳ địa chỉ ví nào vào danh sách hạn chế (`restricted`), khiến người nắm giữ không thể chuyển nhượng tài sản[cite: 8]. |