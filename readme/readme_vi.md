# Pinterest Media Analyzer (Công cụ phân tích phương tiện Pinterest)

> 🔍 Công cụ frontend nhẹ phục vụ mục đích học tập và nghiên cứu, hỗ trợ trích xuất siêu dữ liệu từ nội dung công khai trên Pinterest

🌐 Trải nghiệm trực tuyến: [https://twittervideodownloaderx.com/pinterest_downloader_vi](https://twittervideodownloaderx.com/pinterest_downloader_vi)

---

## 📋 Giới thiệu dự án

Dự án này được phát triển với mục đích học tập và nghiên cứu kỹ thuật, là một công cụ frontend nhẹ giúp hỗ trợ trích xuất thông tin meta của các tài nguyên đa phương tiện như video và hình ảnh từ các trang công khai của Pinterest, sử dụng dữ liệu từ OEmbed Interface và Structured Data (Schema.org / Open Graph) mà nền tảng cung cấp.

> 🎯 Các trường hợp sử dụng được khuyến nghị:
> - Sắp xếp tài liệu học tập cá nhân và thu thập ý tưởng
> - Nghiên cứu và phát triển kỹ thuật trích xuất dữ liệu web (Frontend Development)
> - Học tập về cấu trúc siêu dữ liệu đa phương tiện
> - Hỗ trợ lưu trữ nội dung đã được chủ sở hữu bản quyền cho phép

⚠️ **Lưu ý quan trọng**: Công cụ này chỉ hỗ trợ 'thông tin đã được công khai', không thể phân tích nội dung yêu cầu đăng nhập / trả phí / cài đặt ở chế độ riêng tư.

---

## ✨ Tính năng chính

- 🔗 **Hệ thống nhận diện liên kết tự động**: Hỗ trợ định dạng liên kết chuẩn / liên kết rút gọn / liên kết di động từ trang công khai của Pinterest
- 🎬 **Hỗ trợ đa định dạng**: Trích xuất thông tin tài nguyên video MP4, ảnh động WebM, ảnh tĩnh JPG/PNG, v.v.
- 📐 **Hiển thị thông tin độ phân giải**: Hiển thị danh sách độ phân giải và định dạng tệp khả dụng, cho phép người dùng lựa chọn theo nhu cầu
- 📱 **Thiết kế đáp ứng mọi thiết bị**: Trải nghiệm sử dụng mượt mà trên PC / máy tính bảng / điện thoại thông minh
- ⚡ **Kiến trúc ưu tiên phía client**: Xử lý chính trên trình duyệt, giảm tải cho máy chủ và phản hồi nhanh chóng
- 🔐 **Thiết kế tôn trọng quyền riêng tư**: Không ghi lại liên kết người dùng gửi / Không lưu kết quả phân tích / Không thu thập bất kỳ dữ liệu cá nhân nào

---

## 🚀 Hướng dẫn sử dụng nhanh

1. Mở ứng dụng hoặc website Pinterest, tìm **nội dung công khai** mà bạn muốn tham khảo
2. Sao chép URL của trang đó (ví dụ: `https://www.pinterest.com/pin/1234567890/`)
3. Dán liên kết vào ô nhập liệu của công cụ này, sau đó nhấp nút "Phân tích"
4. Hệ thống sẽ trích xuất siêu dữ liệu công khai và hiển thị danh sách tài nguyên khả dụng
5. Chọn định dạng / độ phân giải mong muốn, nhấp chuột phải → "Lưu thành" để lưu vào thiết bị của bạn

> 💡 Mẹo sử dụng:
> - Vui lòng xác nhận nội dung mục tiêu đang ở chế độ "Công khai"
> - Nếu phân tích thất bại, hãy thử làm mới trang hoặc kiểm tra kết nối mạng
> - Đối với người quan tâm học tập kỹ thuật, khuyến nghị sử dụng kết hợp Developer Tools của trình duyệt (F12 → Network → Fetch/XHR)

---

## ⚠️ Điều khoản sử dụng và Tuyên bố miễn trừ trách nhiệm (Vui lòng đọc kỹ)

Dự án này tuân thủ nguyên tắc "tính trung lập về kỹ thuật" và "tuân thủ pháp luật" làm nền tảng. Vui lòng hiểu rõ các nội dung sau trước khi sử dụng:

### ✅ Hành vi được khuyến khích
- Chỉ phân tích **nội dung công khai** mà bạn có quyền truy cập
- Sử dụng tài nguyên đã trích xuất cho mục đích **học tập cá nhân / nghiên cứu / sử dụng cá nhân**
- Nếu muốn đăng tải lại / tạo tác phẩm phái sinh / sử dụng thương mại, phải xin phép chủ sở hữu bản quyền trước
- Ghi rõ nguồn và tên người sáng tạo trong tác phẩm của bạn, tôn trọng quyền của creator

### ❌ Hành vi bị nghiêm cấm
- Cố gắng phân tích nội dung yêu cầu đăng nhập / trả phí / cài đặt riêng tư
- Sử dụng công cụ cho mục đích scrape thương mại / dịch vụ tổng hợp dữ liệu / kiếm tiền từ quảng cáo
- Gửi lượng lớn yêu cầu trong thời gian ngắn / sử dụng công cụ tự động / tấn công gây quá tải cho nền tảng
- Sửa đổi / xóa / che giấu watermark / thông tin bản quyền / metadata của tài nguyên

> 📜 Cơ sở pháp lý:
> Việc sử dụng công cụ này phải tuân thủ "Luật Sở hữu trí tuệ" "Luật An ninh mạng" của Việt Nam, cũng như "Community Guidelines" và "Developer Policy" của Pinterest.
> Nhà phát triển không chịu bất kỳ trách nhiệm nào đối với thiệt hại hoặc trách nhiệm pháp lý phát sinh từ việc sử dụng không phù hợp của người dùng.

---

## 🛠 Thông tin kỹ thuật tham khảo (Dành cho nhà phát triển)

> Người dùng phổ thông có thể bỏ qua phần này

### Tổng quan kiến trúc
```
Trình duyệt người dùng → Module phân tích phía client → Pinterest Public API / OEmbed → Phân tích dữ liệu có cấu trúc → Hiển thị kết quả
```

### Điểm nổi bật về kỹ thuật
- Sử dụng `fetch` API kết hợp với cấu hình CORS Proxy phù hợp để lấy metadata từ trang công khai
- Phân tích dữ liệu có cấu trúc Schema.org từ `<script type="application/ld+json">`
- Sử dụng Open Graph Tags (`og:video` / `og:image` / `og:title` v.v.) để bổ sung thông tin tài nguyên
- Áp dụng xác thực hai lớp bằng Regular Expression + DOM Parsing để tăng độ ổn định khi nhận diện liên kết

### Hướng dẫn triển khai trên máy chủ cá nhân (Tham khảo)
```bash
# 1. Clone repository (ví dụ)
git clone https://github.com/yourname/pinterest-downloader-vi.git

# 2. Host file tĩnh (khuyến nghị sử dụng HTTPS)
#    - Vercel / Netlify / Cloudflare Pages (khuyến nghị cho người mới)
#    - Nginx + Chứng chỉ Let's Encrypt (cho máy chủ tự xây dựng)

# 3. Ví dụ cấu hình Security Headers (Nginx)
add_header Content-Security-Policy "default-src 'self'; script-src 'self' 'unsafe-inline';";
add_header X-Content-Type-Options "nosniff";
add_header Referrer-Policy "strict-origin-when-cross-origin";
```

> 🔐 Lưu ý khi triển khai môi trường thực tế:
> - Bắt buộc bật HTTPS để ngăn chặn tấn công Man-in-the-Middle
> - Khuyến nghị cấu hình Rate Limiting để hạn chế yêu cầu quá mức
> - Cần thận trọng khi công khai logic phân tích quá chi tiết, nhằm giảm nguy cơ bị lợi dụng cho mục đích xấu

---

## 🤝 Đóng góp cho dự án

Chúng tôi hoan nghênh tất cả mọi người quan tâm cùng tham gia phát triển và cải thiện dự án!

| Loại đóng góp | Ví dụ nội dung |
|--------------|----------------|
| 🐛 Báo cáo lỗi | Tạo Issue thông báo lỗi phân tích / hiển thị (kèm URL + thông tin trình duyệt + các bước tái hiện) |
| 💡 Đề xuất tính năng | Chia sẻ ý tưởng sáng tạo để cải thiện UX / hỗ trợ đa ngôn ngữ / khả năng tiếp cận tốt hơn |
| 🌍 Hỗ trợ dịch thuật | Hỗ trợ dịch và hiệu đính nội dung cho các ngôn ngữ khác (Trung / Anh / Nhật v.v.) |
| 📚 Phát triển tài liệu | Bổ sung ví dụ sử dụng / tạo sơ đồ giải thích nguyên lý hoạt động / tăng cường hướng dẫn tuân thủ quy định |

> Dự án này được phát hành theo [Giấy phép MIT](./LICENSE). Chúng tôi hoan nghênh việc sử dụng / chỉnh sửa vì mục đích học tập và nghiên cứu. Nếu cần tùy chỉnh cho mục đích thương mại, vui lòng liên hệ qua kênh riêng.

---

## ❓ Câu hỏi thường gặp (FAQ)

**Q: Xuất hiện thông báo "Không thể lấy nội dung", nguyên nhân do đâu?**  
A: Nguyên nhân có thể: ① Liên kết đích là nội dung riêng tư / đã bị xóa ② Pinterest tạm thời thay đổi cấu trúc trang ③ Hạn chế mạng / vấn đề CORS. Cách xử lý: Xác nhận cài đặt công khai → Thử dùng mạng khác → Đợi một lát rồi thử lại.

**Q: Video trích xuất có watermark, điều này có bình thường không?**  
A: Công cụ này chỉ trả về liên kết tài nguyên gốc do Pinterest cung cấp chính thức. Việc có hay không có watermark phụ thuộc vào cài đặt khi tải lên của người sáng tạo nội dung. Công cụ này không thực hiện bất kỳ thao tác thêm / xóa / sửa đổi nào.

**Q: Có hỗ trợ phân tích hàng loạt cho album hoặc board không?**  
A: Phiên bản hiện tại tập trung vào phân tích pin đơn lẻ, nhằm ưu tiên tính ổn định và tuân thủ quy định. Đối với yêu cầu xử lý hàng loạt, vui lòng tự kiểm tra tính phù hợp với "Developer Policy" của Pinterest trước.

**Q: Công cụ này có thu thập lịch sử sử dụng hoặc dữ liệu cá nhân không?**  
A: Không. Dự án này là trang web tĩnh phía client thuần túy, không có backend ghi log / script phân tích / hoặc hệ thống theo dõi qua cookie. Toàn bộ quá trình xử lý đều diễn ra cục bộ trong trình duyệt của bạn.

---

## 🌱 Triết lý và tầm nhìn của chúng tôi

> Bản thân công nghệ không có thiện hay ác. Điều quan trọng là 'mục đích' và 'trách nhiệm' của người sử dụng.

Chúng tôi mong mời các nhà phát triển và người dùng cùng tuân thủ các giá trị sau:

- 🔬 Lấy học tập và sự tò mò làm động lực, để hiểu sâu sắc nguyên lý của công nghệ web
- 🤲 Tôn trọng quyền của creator, xây dựng thói quen ghi nguồn và xin phép phù hợp
- 🌍 Góp phần thúc đẩy sự lưu thông lành mạnh của nội dung số và bảo tồn sự đa dạng văn hóa

Cùng nhau xây dựng vòng tuần hoàn tích cực của sáng tạo và chia sẻ, thông qua việc sử dụng đúng đắn và có trách nhiệm ✨

---

## 📄 Giấy phép

Dự án này được phát hành theo [Giấy phép MIT](./LICENSE).  
Nếu muốn sử dụng thương mại hoặc phân phối lại, vui lòng tuân thủ các điều khoản của giấy phép và ghi rõ nguồn gốc.

```


Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---


*🔖 Phiên bản: v1.2.0-vi (Tối ưu hiệu suất phía client / Tăng cường hỗ trợ đa ngôn ngữ / Bổ sung chi tiết điều khoản sử dụng)*