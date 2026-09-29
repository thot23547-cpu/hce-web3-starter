# Báo cáo Lab 2 - Ví và giao dịch đầu tiên

## 1. Giao dịch thành công trên Sepolia
- **Mã băm giao dịch (TxHash):** `0xf9b7a42e55997431f30ac56ae8dbb10af9fb82fb69ef2ecd740fd1f0cefc0e55`
- **Số lượng chuyển:** 0.01 Sepolia ETH
- **Trạng thái:** Thành công (Confirmed)

## 2. Thử nghiệm thay đổi địa chỉ ví nhận và bài học rút ra
- **Thực tế thử nghiệm:** Khi thử thay đổi ký tự trong địa chỉ ví nhận, nếu chuỗi ký tự vẫn thỏa mãn định dạng hợp lệ, giao dịch vẫn có thể được thực thi và chuyển tiền đi.
- **Bài học rút ra:** Các giao dịch trên blockchain có tính bất biến và không có cơ quan trung gian hay tổng đài nào hỗ trợ lấy lại tiền nếu chuyển nhầm. Do đó, việc kiểm tra kỹ lưỡng từng ký tự của địa chỉ ví trước khi bấm gửi là bắt buộc để tránh mất tài sản.