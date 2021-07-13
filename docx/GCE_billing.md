# Chi phí dịch vụ GCE
- Chi phí sử dụng Google Compute Engine được gửi vào cuối mỗi chu kì thanh toán (đơn vị thanh toán: $ - Đô la Mỹ)
- Đối với Google Compute Engine: kích thước ổ đĩa (disk size), bộ nhớ (memory) và mức sử dụng mạng (network usage) được sử dụng đơn vị gigabyte (GB).
  - Note:  1 GB thường được định nghĩa là 1.000.000.000 byte.  GiB (Gibibytes) là một đơn vị tiêu chuẩn được sử dụng trong lĩnh vực xử lý và truyền dữ liệu và được định nghĩa là cơ sở 1024 chứ không phải cơ sở 1000. Ví dụ: 1 GB được định nghĩa là 1000^3 byte, trong khi 1 GiB được định nghĩa là 1024^3 byte.

Chi phí dịch vụ sẽ bao gồm các chi phí dành cho

  - Chi phí Instance
  - Chi phí Disk và Image
  - Chi phí Network
  - Chi phí GPU

## Các cách tra cứu thông tin chi phí giá dịch vụ GCE

1. Xem chi phí ước tính cho các phiên bản và tài nguyên Compute Engine trực tiếp trong khi tạo Instance trong Google Cloud Console.
2. Ước tính tổng chi phí dự án dựa trên các phiên bản và tài nguyên cần thiết thông qua công cụ tính toán của Google.
Ngoài 2 cách phổ biến trên thì còn có thể xem và tải xuống từ Bảng giá trong Google Cloud Console hoặc nhận thông tin về giá thông qua API.
Sử dụng các công cụ tuỳ theo nhu cầu của người dùng:

  - Sử dụng xem chi phí trong Google Cloud Console để nắm được chi phí của hệ thống đang xây dựng kèm theo các chính sách giảm giá cho từng instance.
  - Sử dụng Công cụ tính toán của google và bảng giá để có thể tính toán chi phí trước khi xây dựng hệ thống theo kiến trúc, cấu hình định trước.
  - Sử dụng bảng giá thông qua API phục vụ cho các bài toán xây dựng hệ thống billing, tích hợp với các ứng dụng khác theo nhu cầu.
- Google luôn có chính sách giảm giá cho người dùng sử dụng liên tục (càng sử dụng nhiều trong 1 tháng thì càng được chiết khẩu nhiều hơn) hoặc cam kết sử dụng 1 năm, 3 năm. Chi phí sử dụng dịch vụ có thể giảm tới 57% (cam kết sử dụng 3 năm) so với sử dụng theo giờ (theo nhu cầu).

# Tham khảo
- https://cloud.google.com/compute/vm-instance-pricing