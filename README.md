# SubYoutube

> Lấy phụ đề, bình luận YouTube tích hợp Prompt tóm tắt.

**SubYoutube** là extension Manifest V3 dành cho Microsoft Edge, giúp bạn lấy transcript/phụ đề và bình luận từ video YouTube đang mở, sau đó sao chép nội dung hoặc tạo prompt có cấu trúc để sử dụng với các công cụ AI.

## Cài đặt

| Nền tảng | Liên kết |
|---|---|
| Microsoft Edge Add-ons | **Sắp cập nhật sau khi extension được duyệt** |
| Chrome Web Store | **Sắp cập nhật** |

Liên kết cài đặt chính thức sẽ được bổ sung ngay sau khi Microsoft Edge Add-ons cấp URL sản phẩm. Trong thời gian chờ duyệt, bạn có thể cài bản thử nghiệm bằng cách dùng **Load unpacked** trong Edge Developer mode với thư mục chứa `manifest.json`.

## Tính năng chính

SubYoutube đọc transcript theo track phụ đề mà người dùng đang chọn trên YouTube. Transcript và bình luận được hiển thị trong hai khu vực riêng biệt để có thể sao chép độc lập.

Extension có thể thu thập tối đa 500 mục bình luận, bao gồm bình luận chính và các phản hồi đã mở rộng. Cấu trúc phản hồi được thể hiện bằng ký hiệu `↳`, `↳ ↳` và các cấp tương ứng để dễ theo dõi mạch thảo luận.

Bạn có thể sao chép riêng transcript, bình luận, prompt transcript, prompt bình luận hoặc prompt tổng hợp. Prompt được tạo bằng tiếng Việt hoặc tiếng Anh tùy ngôn ngữ giao diện đã chọn.

Transcript có timestamp có thể được xuất thành file phụ đề `.SRT`. Kết quả quét được lưu tạm theo từng video để đóng và mở lại popup không phải quét lại ngay từ đầu; dữ liệu quá 24 giờ sẽ tự động được dọn dẹp và chỉ tối đa 10 video gần nhất được giữ lại.

## Ngôn ngữ và dữ liệu

Giao diện hỗ trợ **tiếng Việt và English**. Nút VI/EN chỉ thay đổi ngôn ngữ giao diện và prompt; extension không tự động dịch transcript hoặc bình luận. Nội dung vẫn giữ nguyên theo track phụ đề và dữ liệu YouTube mà người dùng chọn.

SubYoutube chỉ hoạt động khi người dùng chủ động mở extension trên một trang video YouTube. Extension đọc transcript/phụ đề, bình luận, URL và tiêu đề video để hiển thị, tạo prompt, lưu tạm theo video và xuất SRT. Dữ liệu được xử lý trong trình duyệt và không tự động gửi đến máy chủ SubYoutube hoặc nhà cung cấp AI bên ngoài. Người dùng tự quyết định việc sao chép dữ liệu sang ứng dụng khác.

Xem [Chính sách quyền riêng tư](PRIVACY.md) để biết thêm chi tiết.

## Cài bản thử nghiệm trên Microsoft Edge

1. Tải hoặc giải nén package phát hành.
2. Mở `edge://extensions`.
3. Bật **Developer mode / Chế độ nhà phát triển**.
4. Chọn **Load unpacked / Tải giải nén**.
5. Chọn thư mục có `manifest.json` ở ngay cấp bên trong.
6. Mở một video YouTube, tải lại trang bằng `Ctrl + R`, sau đó mở SubYoutube.

Bản phát hành chính thức sẽ được cài trực tiếp từ liên kết Microsoft Edge Add-ons sau khi được xét duyệt.

## Quyền extension

SubYoutube sử dụng các quyền cần thiết để hoạt động trên video YouTube do người dùng chủ động mở:

| Quyền | Mục đích |
|---|---|
| `activeTab` | Truy cập tab hiện tại sau khi người dùng mở popup và yêu cầu quét. |
| `scripting` | Đọc transcript và bình luận trong trang YouTube hiện tại. |
| `tabs` | Đọc URL và tiêu đề video để xác định và lưu trạng thái theo video. |
| `storage` | Lưu tạm transcript, bình luận, prompt và timestamp trong trình duyệt. |
| YouTube host permissions | Giới hạn hoạt động trên các miền YouTube cần thiết. |

Extension không sử dụng mã JavaScript từ xa và không tự động gửi nội dung sang dịch vụ AI.

## Đóng góp và phản hồi

Nếu bạn phát hiện lỗi hoặc muốn đề xuất tính năng, hãy mở một [Issue](https://github.com/Tungronoro/SubYoutube/issues). Khi báo lỗi transcript, nên ghi rõ ngôn ngữ phụ đề đang chọn trên YouTube và phiên bản Edge đang sử dụng; không đăng thông tin tài khoản, mã xác minh hoặc dữ liệu riêng tư.

## Trạng thái dự án

- Phiên bản hiện tại: **4.7.0**
- Manifest: **V3**
- Nền tảng thử nghiệm: **Microsoft Edge Chromium**
- Trạng thái cửa hàng: **Đang chờ đăng và xét duyệt**

## License

License sẽ được bổ sung cùng chính sách phát hành chính thức.
