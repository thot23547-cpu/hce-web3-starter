# Báo cáo Lab 3 - Đọc giao dịch và hợp đồng trên Etherscan

## 1. Phân tích giao dịch cá nhân trên Sepolia Etherscan
- **Mã băm giao dịch (TxHash):** `0xf9b7a42e55997431f30ac56ae8dbb10af9fb82fb69ef2ecd740fd1f0cefc0e55`[cite: 2]
- **Status (Trạng thái):** Thành công (Success)[cite: 5]
- **Block (Khối):** 11806665[cite: 5]
- **Timestamp (Thời điểm):** 29-09-2026 09:09:00 AM +UTC[cite: 5]
- **From (Từ):** `0x64d6031012355d879cd5489057341fa4120e63f4`[cite: 5]
- **To (Đến):** `0xaa8c9ec8c58fed71fcee9188788c7c3c598f9411`[cite: 5]
- **Value (Giá trị):** 0,01 ETH[cite: 5]
- **Transaction Fee (Phí giao dịch):** 0.000053992459353 ETH[cite: 5]
- **Gas Price (Giá xăng):** 2.571069493 Gwei[cite: 5]

## 2. Trả lời câu hỏi nghiên cứu hợp đồng
1. **Hợp đồng bạn xem có công bố mã nguồn đã xác thực không?** 
   - Có, hợp đồng USDT (`0xdac1f784358f7894197551c42b390a611a991ec7`) trên Etherscan đã công bố mã nguồn xác thực (Verified Source Code)[cite: 5].
2. **Tổng cung của đồng đó là bao nhiêu? Đọc ra từ hàm nào?** 
   - Tổng cung có thể đọc được bằng cách gọi hàm `totalSupply()` trong tab Read Contract mà không tốn phí[cite: 5].
3. **Trong tab Write Contract, có hàm nào cho phép đóng băng tài khoản người khác không? Tên hàm là gì?** 
   - Có, trong cấu trúc hợp đồng của các đồng ổn định giá lớn (như USDT/USDC), tồn tại các hàm quản trị đặc quyền cho phép chủ sở hữu hoặc địa chỉ được chỉ định thực hiện việc đóng băng tài khoản (ví dụ: hàm `freeze` hoặc các hàm kiểm soát rủi ro tương đương trong hệ thống)[cite: 5].