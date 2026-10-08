# Hệ thống chấm điểm Ngân hàng số

Dự án này xây dựng một quy trình có thể tái lập để trích xuất, lọc và tổng hợp bằng chứng phục vụ đánh giá mức độ chuyển đổi số của một số ngân hàng thương mại Việt Nam dựa trên các tài liệu công khai như Báo cáo thường niên và Báo cáo phát triển bền vững.

Quy trình tập trung vào việc tìm bằng chứng theo 16 tiêu chí ngân hàng số, lọc bằng chứng theo hai tầng và tổng hợp kết quả thành file Excel cuối cùng để phục vụ bước chấm điểm và xếp hạng sau đó.

## Các ngân hàng được phân tích

Dữ liệu hiện tại gồm 5 ngân hàng:

- BIDV
- Vietcombank (VCB)
- OCB
- MB
- VietinBank

## Nguồn báo cáo

Dự án sử dụng Báo cáo thường niên và Báo cáo phát triển bền vững năm 2025 khi có sẵn.

Nguồn dữ liệu hiện tại gồm:

- Vietcombank: Báo cáo thường niên 2025 và Báo cáo phát triển bền vững 2025
- OCB: Báo cáo thường niên 2025 và Báo cáo phát triển bền vững 2025
- MB: Báo cáo thường niên 2025
- VietinBank: Báo cáo thường niên 2025 và Báo cáo phát triển bền vững 2025
- BIDV: Báo cáo thường niên 2025 và Báo cáo phát triển bền vững 2025

## Khung đánh giá

Hệ thống sử dụng 16 tiêu chí, chia thành 4 nhóm chính.

### A. Chiến lược và nguồn lực số

- A1 – Chiến lược chuyển đổi số
- A2 – Đầu tư CNTT / chuyển đổi số
- A3 – Quản trị chuyển đổi số
- A4 – Nhân lực số

### B. Sản phẩm số và trải nghiệm khách hàng

- B1 – eKYC
- B2 – Mobile / Digital Banking
- B3 – QR / Digital Payment
- B4 – Thẻ số / thẻ ảo

### C. Công nghệ và dữ liệu

- C1 – Trí tuệ nhân tạo (AI)
- C2 – Điện toán đám mây (Cloud)
- C3 – API / Open Banking
- C4 – Big Data / Data Platform

### D. Vận hành số và an toàn

- D1 – RPA / Automation
- D2 – Số hóa quy trình
- D3 – An ninh mạng
- D4 – Phát hiện gian lận

## Quy trình xử lý dữ liệu

Quy trình gồm 5 bước chính.

### Bước 1 – Thu thập báo cáo

Thu thập Báo cáo thường niên và Báo cáo phát triển bền vững của từng ngân hàng và lưu theo từng thư mục riêng.

Ví dụ:

```text
Data giữa kì/
│
├── BIDV/
├── MB/
├── OCB/
├── VCB/
└── VietinBank/
