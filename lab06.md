# BÁO CÁO TRIỂN KHAI SMART CONTRACT TRÊN SEPOLIA (LAB 6)

## 1. Thông tin Triển khai (Deployment Info)

- **Tên Hợp đồng:** `Greeter.sol`
- **Địa chỉ Hợp đồng (Contract Address):** `0xd8bdf83465db6efe5f8d8d2cacc13d475b3f3fa8` *(Dán địa chỉ hợp đồng bạn vừa Deploy vào đây)*
- **Mã băm giao dịch triển khai (Deploy TxHash):** `0xb3ab78ac2bea5ea7f3fc05af92a8901f6081PbWWqgKDBDorh525uecKaGZD21FGSoCeR` *(Dán TxHash từ MetaMask/Etherscan vào đây)*
- **Mạng thử nghiệm:** Sepolia Testnet

## 2. Nhật ký Tương tác Hợp đồng

| Thao tác | Hàm sử dụng | Dữ liệu đầu vào | Kết quả thực thi |
| :--- | :--- | :--- | :--- |
| **Khởi tạo** | `constructor()` | `"Xin chao Hue University!"` | Triển khai thành công |
| **Đọc dữ liệu** | `greet()` | Không có | Trả về chuỗi `"Xin chao Hue University!"` |
| **Ghi dữ liệu** | `setGreeting()` | `"Lop Kinh te so Web3"` | Cập nhật câu chào mới thành công |

## 3. Bài học rút ra

- Hiểu được quy trình từ viết code Solidity -> Compile -> Deploy thông qua ví MetaMask.
- Phân biệt được hàm đọc (`view`) không tốn Gas và hàm ghi (`setGreeting`) tốn phí Gas.