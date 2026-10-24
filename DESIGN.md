# Thiết kế giao diện landing page — Váy cưới Mẫn Nhi (TEC-24)

> Thuộc Epic TEC-23, project Linear `m-software-vay-cuoi-man-nhi`.
> Bản thiết kế này đủ để Dev dựng trang mà không cần hỏi thêm:
> mọi section đều có bố cục, màu sắc, nội dung từng khối và ghi chú kỹ thuật.
> Nội dung là nội dung gốc do M-Software soạn; hình ảnh dùng ảnh minh họa
> chung (ảnh mẫu váy cưới, hoa, không gian tiệm) — KHÔNG dùng hình ảnh
> hay thương hiệu của bất kỳ trang tham khảo nào.

## 1. Tổng quan

- **Mục đích:** giới thiệu dịch vụ **cho thuê váy cưới** và dẫn khách đặt lịch thử váy.
- **Đối tượng:** cô dâu chuẩn bị cưới, người thân đi cùng; xem chủ yếu trên điện thoại.
- **Hành động chính (CTA chính):** nút **“Đặt lịch thử váy”** — xuất hiện ở hero,
  cuối mỗi section lớn và thanh CTA cố định cuối trang trên mobile.
- **Cấu trúc trang (từ trên xuống):**
  1. Header cố định → 2. Hero → 3. Danh mục váy cưới → 4. Bảng giá thuê →
  5. Quy trình thuê → 6. Đánh giá khách hàng → 7. Form liên hệ / đặt lịch →
  8. Footer.
- **Ngôn ngữ / giọng văn:** ấm áp, trang trọng, gần gũi; xưng “Mẫn Nhi”,
  gọi khách là “cô dâu” hoặc “bạn”.

## 2. Hệ màu — chủ đạo đỏ hỷ

| Vai trò | Màu | Mã | Ghi chú |
|---|---|---|---|
| Chủ đạo (đỏ hỷ) | Đỏ hỷ | `#B91C2E` | Nút CTA, tiêu đề điểm nhấn, viền, icon |
| Đỏ đậm | Đỏ rượu | `#7F1220` | Header khi cuộn, footer, hover nút |
| Nền sáng | Kem | `#FDF8F3` | Nền toàn trang |
| Nền phụ | Hồng nhạt | `#FBEAEA` | Nền xen kẽ section chẵn |
| Nền tối | Đen ấm | `#1F1718` | Footer, chữ trên ảnh tối |
| Chữ chính | Đen ấm | `#2B2122` | Tiêu đề, nội dung |
| Chữ phụ | Xám ấm | `#6E5F60` | Mô tả, chú thích |
| Viền / chia khối | Hồng xám | `#E8D5D5` | Card, bảng giá |
| Điểm nhấn | Vàng đồng | `#C9A227` | Giá, sao đánh giá, họa tiết trang trí |

- Tương phản: chữ trên nền đỏ hỷ dùng trắng `#FFFFFF`; chữ vàng đồng
  chỉ dùng cho số liệu/điểm nhấn, không dùng làm chữ nội dung dài.
- Ảnh: tông ấm, sáng, váy trắng/nude nổi trên nền kem; không dùng ảnh tối,
  ảnh có logo thương hiệu khác.

## 3. Kiểu chữ & lưới bố cục

- **Tiêu đề:** font serif trang trọng (ví dụ Playfair Display hoặc serif hệ thống),
  cỡ 40px desktop / 30px mobile, đậm vừa, màu đen ấm, từ khóa điểm nhấn màu đỏ hỷ.
- **Nội dung:** font sans-serif dễ đọc (ví dụ Inter hoặc sans hệ thống),
  cỡ 16px desktop / 15px mobile, giãn dòng 1,6.
- **Nút:** bo tròn 999px (dạng viên nang), nút chính nền đỏ hỷ chữ trắng,
  nút phụ viền đỏ hỷ chữ đỏ hỷ; hover nút chính chuyển đỏ rượu.
- **Lưới:** tối đa 1200px, căn giữa, padding hai bên 24px (mobile 16px).
  Desktop 3–4 cột cho card, tablet 2 cột, mobile 1 cột, xếp dọc.
- **Khoảng cách section:** 80px desktop / 56px mobile; tiêu đề section luôn có
  dòng phụ nhỏ màu đỏ hỷ phía trên (eyebrow) và đường gạch vàng đồng ngắn bên dưới.

## 4. Header (cố định)

- Bên trái: tên **“Váy cưới Mẫn Nhi”** (chữ serif, đỏ hỷ) + dòng nhỏ
  “Cho thuê váy cưới”.
- Giữa (desktop): menu neo tới các section: Váy cưới · Bảng giá · Quy trình ·
  Đánh giá · Liên hệ.
- Bên phải: nút **“Đặt lịch thử váy”** (đỏ hỷ).
- Mobile: menu thu gọn (hamburger); nút CTA giữ lại dạng icon + chữ ngắn.
- Khi cuộn xuống: header thêm nền trắng + bóng mờ nhẹ, không che nội dung.

## 5. Section 1 — Hero

- **Bố cục:** 2 cột desktop (trái chữ, phải ảnh), mobile xếp dọc (ảnh sau chữ).
- **Trái:**
  - Eyebrow: “Cho thuê váy cưới — Mẫn Nhi”.
  - Tiêu đề lớn: “Ngày cưới rạng rỡ, bắt đầu từ chiếc váy trong mơ.”
    (“trong mơ” tô màu đỏ hỷ.)
  - Mô tả 2 câu: hơn 200 mẫu váy cưới cho thuê, từ dáng công chúa,
    đuôi cá đến cổ điển; thử váy miễn phí buổi đầu, tư vấn chọn dáng theo
    vóc dáng và ngân sách.
  - 2 nút: chính “Đặt lịch thử váy” (nhảy tới form cuối trang),
    phụ “Xem mẫu váy” (nhảy tới danh mục).
  - Dòng tin cậy nhỏ: ★ 4,9/5 · 300+ cô dâu đã thuê · Thử váy miễn phí buổi đầu.
- **Phải:** ảnh minh họa lớn (cô dâu mặc váy cưới trắng, phông sáng),
  bo góc 24px, góc dưới chèn thẻ nổi nhỏ: “Thuê từ 2.500.000đ / váy”.
- **Trang trí:** họa tiết hoa nhẹ góc ảnh, không rối, không che mặt mẫu.

## 6. Section 2 — Danh mục váy cưới

- **Tiêu đề:** “Chọn dáng váy của riêng bạn” — phụ đề:
  “Mỗi dáng váy một vẻ đẹp riêng; bấm vào từng nhóm để xem gợi ý.”
- **Bố cục:** lưới 4 card desktop / 2 tablet / 1 mobile. Mỗi card gồm:
  ảnh minh họa dáng váy, tên nhóm, 1 câu mô tả, khoảng giá thuê, nút “Xem mẫu”.
- **4 nhóm (nội dung gốc):**

| Nhóm | Mô tả | Hợp với | Giá thuê tham khảo |
|---|---|---|---|
| Công chúa bồng xòe | Chân váy nhiều lớp, thắt eo, lộng lẫy như cổ tích | Tiệc lớn, sân khấu | 4.000.000 – 8.000.000đ |
| Đuôi cá ôm dáng | Ôm sát thân trên, xòe nhẹ từ gối xuống, tôn dáng | Cô dâu dáng cân đối, tiệc tối | 3.500.000 – 7.000.000đ |
| Chữ A thanh lịch | Xòe nhẹ từ eo, gọn gàng, dễ di chuyển | Mọi vóc dáng, tiệc ngoài trời | 2.500.000 – 5.000.000đ |
| Cổ điển / ren tay dài | Ren tinh tế, tay dài kín đáo, sang trọng | Lễ nhà thờ, tiệc trang trọng | 3.000.000 – 6.500.000đ |

- **Ghi chú dưới lưới:** “Giá là giá thuê trọn gói theo ngày cưới (xem chi tiết
  ở Bảng giá). Mẫu mới về mỗi tháng — đặt lịch thử để xem mẫu mới nhất.”
- **Ghi chú cho Dev:** card dùng ảnh placeholder chung, tên file gợi ý
  `assets/vay-cong-chua.jpg`, `vay-duoi-ca.jpg`, `vay-chu-a.jpg`,
  `vay-co-dien.jpg`; khi có ảnh thật chỉ cần thay file, không đổi bố cục.

## 7. Section 3 — Bảng giá thuê

- **Tiêu đề:** “Bảng giá thuê minh bạch” — phụ đề:
  “Giá đã gồm giặt ủi, chỉnh sửa cơ bản và phụ kiện đi kèm ghi rõ từng gói.”
- **Bố cục:** 3 cột desktop (gói giữa nổi bật), mobile xếp dọc.
  Gói giữa có viền đỏ hỷ dày hơn, nhãn “Được chọn nhiều nhất” màu đỏ hỷ.

| Gói | Giá | Gồm những gì | Phù hợp |
|---|---|---|---|
| Cơ bản | 2.500.000đ / váy | Váy thuê 1 ngày cưới; chỉnh sửa cơ bản (eo, lai); giặt ủi sau tiệc | Tiệc nhỏ, ngân sách gọn |
| Tiêu chuẩn ★ | 4.500.000đ / váy | Mọi quyền lợi gói Cơ bản + voan + vương miện; thử váy 2 buổi; giao nhận tận nơi trong nội thành | Đa số cô dâu — gói khuyên dùng |
| Cao cấp | 7.500.000đ / váy | Mọi quyền lợi gói Tiêu chuẩn + váy thiết kế riêng theo số đo; trang điểm thử 1 buổi; hỗ trợ suốt ngày cưới | Tiệc lớn, muốn riêng biệt |

- **Dưới bảng:** 3 lưu ý ngắn, mỗi lưu ý 1 dòng có icon:
  1. Đặt cọc 30% khi giữ váy; thanh toán phần còn lại khi nhận váy.
  2. Hủy lịch trước 14 ngày được hoàn cọc; trong 14 ngày giữ cọc cho lần sau.
  3. Hư hỏng nhẹ do sử dụng bình thường không tính phí; hư hỏng nặng báo giá
     sửa trước khi thu phí.
- **CTA cuối section:** nút “Đặt lịch thử váy — giữ gói Tiêu chuẩn”.

## 8. Section 4 — Quy trình thuê (5 bước)

- **Tiêu đề:** “Thuê váy chỉ với 5 bước” — phụ đề:
  “Từ lần thử đầu tiên đến ngày trả váy, Mẫn Nhi đồng hành cùng bạn.”
- **Bố cục:** hàng ngang 5 bước có mũi tên nối (desktop), dọc có đường nối
  (mobile). Mỗi bước: số tròn nền đỏ hỷ, tên bước, mô tả 1–2 câu.

| Bước | Tên | Nội dung |
|---|---|---|
| 1 | Đặt lịch thử váy | Điền form cuối trang hoặc nhắn tin; Mẫn Nhi xác nhận lịch trong ngày. |
| 2 | Thử váy tại tiệm | Thử tối đa 5 mẫu/buổi, tư vấn viên gợi ý dáng theo vóc dáng và ngân sách. |
| 3 | Chốt váy & đặt cọc | Giữ váy bằng cọc 30%; hẹn ngày chỉnh sửa và ngày nhận váy. |
| 4 | Nhận váy ngày cưới | Nhận váy đã giặt ủi, chỉnh sửa vừa vặn; kiểm tra cùng nhau trước khi mang về. |
| 5 | Trả váy sau tiệc | Trả trong 2 ngày sau cưới; Mẫn Nhi lo giặt ủi, bạn không cần giặt trước. |

- **Ghi chú cho Dev:** bước hiện tại của khách không cần trạng thái động ở
  bản landing đầu tiên — hiển thị tĩnh toàn bộ 5 bước.

## 9. Section 5 — Đánh giá khách hàng

- **Tiêu đề:** “Cô dâu nói gì về Mẫn Nhi” — phụ đề: “★ 4,9/5 từ 300+ lượt thuê”.
- **Bố cục:** 3 card đánh giá (desktop), trượt ngang trên mobile. Mỗi card:
  5 sao vàng đồng, 1 đoạn trích 2–3 câu, tên cô dâu (chỉ tên, không họ đầy đủ),
  tháng/năm thuê, gói đã thuê.
- **Nội dung mẫu (gốc, để Dev dựng khung; thay bằng đánh giá thật khi có):**
  1. “Váy vừa như may đo, nhân viên tư vấn rất có tâm. Ngày cưới mình nhận
     được bao nhiêu lời khen!” — Lan Anh, 09/2026, gói Tiêu chuẩn.
  2. “Thử 4 mẫu mới chọn được chiếc ưng ý, không hề bị ép chốt nhanh.
     Giá rõ ràng từ đầu, không phát sinh.” — Thu Hà, 08/2026, gói Cơ bản.
  3. “Mình ở xa nên được giao váy tận nơi, váy sạch thơm, đóng gói cẩn thận.
     Sẽ giới thiệu bạn bè.” — Phương Linh, 07/2026, gói Cao cấp.
- **Lưu ý trung thực:** khi lên trang thật, chỉ giữ những đánh giá có thật;
  các đoạn trên là văn bản mẫu dựng khung, phải thay trước khi công bố.

## 10. Section 6 — Form liên hệ / đặt lịch thử váy

- **Tiêu đề:** “Đặt lịch thử váy miễn phí buổi đầu”.
- **Bố cục:** 2 cột desktop (trái: thông tin liên hệ + giờ mở cửa; phải: form),
  mobile xếp dọc.
- **Trái:** địa chỉ tiệm (để trống chờ PO điền địa chỉ thật — không bịa địa chỉ),
  số điện thoại (chờ PO điền), giờ mở cửa 9:00–20:00 hằng ngày,
  dòng “Mẫn Nhi trả lời trong ngày làm việc.”
- **Form — các trường:**
  1. Họ tên (bắt buộc) · 2. Số điện thoại (bắt buộc, kiểm tra 10 số) ·
  3. Ngày muốn thử (bắt buộc, chọn ngày, không cho ngày quá khứ) ·
  4. Buổi: Sáng / Chiều / Tối (chọn 1) · 5. Dáng váy quan tâm (chọn nhiều:
     Công chúa / Đuôi cá / Chữ A / Cổ điển / Chưa biết — tư vấn giúp mình) ·
  6. Ngân sách dự kiến (tùy chọn: Dưới 3 triệu / 3–5 triệu / Trên 5 triệu) ·
  7. Ghi chú thêm (tùy chọn, tối đa 500 ký tự).
- **Nút gửi:** “Gửi yêu cầu đặt lịch” (đỏ hỷ). Sau khi gửi: hiện thông báo
  “Cảm ơn bạn! Mẫn Nhi sẽ liên hệ xác nhận lịch trong ngày.”
- **Ghi chú cho Dev:** bản thiết kế này chỉ định nghĩa giao diện form;
  nơi lưu dữ liệu form (email / sheet / API) do task Dev quyết định,
  không tự chọn trong bản thiết kế để tránh đoán sai hạ tầng.

## 11. Footer

- 3 cột: (1) tên shop + câu giới thiệu 1 dòng; (2) liên kết nhanh
  (Váy cưới, Bảng giá, Quy trình, Đánh giá); (3) liên hệ (địa chỉ, điện thoại
  — chờ PO điền, giống mục 10).
- Dòng cuối: “© 2026 Váy cưới Mẫn Nhi — Thiết kế bởi M-Software (TEC-24).”

## 12. Responsive & trạng thái

- **Breakpoint:** desktop ≥ 1024px · tablet 768–1023px · mobile < 768px.
- **Mobile:** hero chữ trước ảnh sau; bảng giá gói Tiêu chuẩn lên đầu;
  CTA “Đặt lịch thử váy” cố định đáy màn hình khi cuộn qua hero.
- **Trạng thái:** nút khi bấm chuyển đỏ rượu; trường form lỗi viền đỏ +
  dòng chữ đỏ giải thích; ảnh chưa tải hiện nền hồng nhạt, không vỡ bố cục.
- **Tiếp cận:** mọi nút có chữ rõ nghĩa (không chỉ icon); tương phản chữ/nền
  đạt mức đọc thoải mái; form dùng được bằng bàn phím.

## 13. Bàn giao cho Dev

- File này là tài sản thiết kế duy nhất của TEC-24; Dev dựng trang theo đúng
  thứ tự section mục 1, bảng màu mục 2, kiểu chữ mục 3.
- Việc còn thiếu, chờ PO/Dev quyết (không bịa trong thiết kế):
  địa chỉ + số điện thoại thật của tiệm; ảnh váy thật; đánh giá thật;
  nơi lưu dữ liệu form.
- Checklist nghiệm thu theo AC: đủ 6 section (hero, danh mục, bảng giá,
  quy trình, đánh giá, form) + header/footer; mỗi section có màu, bố cục,
  nội dung từng khối như trên; nội dung gốc, không dùng thương hiệu khác.
