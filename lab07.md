# BÁO CÁO PHÂN QUYỀN & QUẢN LÝ TRẠNG THÁI TRONG SMART CONTRACT (LAB 7)

## 1. Thông tin Triển khai Hợp đồng

- **Tên Hợp đồng:** `AccessControl.sol`
- **Địa chỉ Hợp đồng (Contract Address):** `0xd7a766388bdb6319e364266481caadc88ab2771b` *(Dán địa chỉ hợp đồng thu được ở Bước 3)*
- **Mã băm giao dịch triển khai (Deploy TxHash):** `0xc685890ad5d5ecac892ca55fe3399afd680e63c72ef430b7e953209d9eb29916` *(Dán mã TxHash thu được ở Bước 3)*
- **Mạng thử nghiệm:** Sepolia Testnet

## 2. Kết quả Kiểm thử Phân quyền (Access Control)

| Trường hợp | Ví thực thi | Hàm gọi | Kết quả kỳ vọng | Kết quả thực tế |
| :--- | :--- | :--- | :--- | :--- |
| **Trường hợp 1** | Ví Owner (Chủ hợp đồng) | `setSystemStatus("Bao tri")` | Thành công, trạng thái cập nhật | **Thành công** (Đã phát event `StatusUpdated`) |
| **Trường hợp 2** | Ví khác (Không phải Owner) | `setSystemStatus("Thay doi")` | Bị từ chối (Revert) | **Thành công** (Giao dịch bị chặn với lỗi "Chi Owner moi co quyen") |

## 3. Trả lời câu hỏi thu hoạch

**Câu hỏi 1:** Tại sao cần sử dụng `modifier` thay vì viết lệnh `require` lặp đi lặp lại trong từng hàm?  
**Trả lời:** Việc sử dụng `modifier` (như `onlyOwner`) giúp tái sử dụng mã nguồn, giảm nguy cơ sót lỗi phân quyền, làm code gọn gàng, dễ bảo trì và tiết kiệm phí Gas khi biên dịch.

**Câu hỏi 2:** Sự kiện (`event`) trong Solidity có vai trò gì đối với ứng dụng Web3 Front-end?  
**Trả lời:** `Event` cho phép ghi dữ liệu vết lên nhật ký của Blockchain (Logs). Các ứng dụng Front-end (Web3/React) dựa vào `Event` để lắng nghe (listen) và cập nhật giao diện người dùng theo thời gian thực mà không cần phải liên tục truy vấn Blockchain.