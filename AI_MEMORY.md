# 🧠 AI Context & Memory: Yoga Hoa Đào Project

*Tài liệu này lưu trữ toàn bộ bối cảnh, yêu cầu thiết kế và kiến trúc của dự án "Yoga Hoa Đào" để AI trong các phiên làm việc tiếp theo có thể nắm bắt và tiếp tục công việc ngay lập tức mà không cần hỏi lại người dùng.*

---

## 1. Thông Tin Thương Hiệu (Brand Identity)
- **Tên cơ sở:** Phòng tập Yoga Hoa Đào
- **Địa chỉ:** Số 54, Ngô Gia Khảm, phường Phan Rang, tỉnh Khánh Hòa
- **Người liên hệ:** 0985 787 579 (Gặp Dần)
- **Triết lý cốt lõi:** "Thân ở đâu, tâm ở đó. Nhờ hơi thở dẫn lối." - Đánh thức năng lượng, cân bằng Thân - Tâm - Trí, sự tĩnh tâm và khiêm nhường.

## 2. Hệ Thống Thiết Kế (Design System)
- **Phong cách:** Soft UI / Modern Minimalist (Nhẹ nhàng, thư giãn, hiện đại). **Tuyệt đối không dùng Dark Mode.**
- **Màu sắc chủ đạo:** 
  - Màu nền (Background): Hồng nhạt tĩnh tâm (`#FDF2F8`).
  - Màu nhấn (Primary): Hồng phấn (`#EC4899`, `#BE185D`, `#F9A8D4`).
  - Nút kêu gọi hành động (CTA): Tím hiện đại (`#8B5CF6`, `#7C3AED`) để tạo độ tương phản thu hút.
  - Văn bản: Đỏ rượu/Hồng sậm (`#831843`, `#9D174D`) tạo cảm giác ấm áp thay vì dùng màu đen thông thường.
- **Typography (Phông chữ):** 
  - Tiêu đề (Headings): `Lora` (cổ điển, tinh tế, phù hợp với Yoga).
  - Văn bản (Body): `Raleway` (hiện đại, dễ đọc, thanh thoát).

## 3. Cấu Trúc Mã Nguồn & Kỹ Thuật (Architecture)
- **Cấu trúc file:** Dự án là một Landing Page siêu nhẹ, sử dụng cấu trúc **Single-file (`index.html`)** với HTML, CSS thuần (trong thẻ `<style>`) và JS nội tuyến (Vanilla JS) để đạt hiệu năng tối đa. Không sử dụng Framework phức tạp (tránh React/Next.js cho dự án này trừ khi có yêu cầu mới).
- **Tài nguyên (Assets):** Hình ảnh thực tế của phòng tập được lưu trữ trực tiếp trong thư mục `Anh/` (`01.jpg` đến `15.jpg`, `Logo.jpg` và `Banner.jpg`).
- **Icon:** Sử dụng Inline SVG nguyên bản với nét mỏng (stroke-width: 2) để đảm bảo độ sắc nét và đồng nhất với phong cách Minimalist (ví dụ: các icon ở mục Pain Points).
- **Tối ưu hóa Di động (Mobile-first):**
  - Có Menu Hamburger trượt mượt mà.
  - Sử dụng Nút liên hệ Nổi (Floating Action Button - FAB) ghim ở đáy màn hình điện thoại (`href="tel:0985787579"`).
  - Tỉ lệ hình ảnh động (`aspect-ratio: 4/3` trên mobile).

## 4. Bố Cục Trang Web (Layout Structure)
1. **Header:** Logo + Navigation + CTA.
2. **Top Banner (NEW):** Bức ảnh Banner ngang cực lớn (`Anh/Banner.jpg`) được đặt ngay đầu `<main>` (rộng toàn màn hình - 100% width) để truyền tải thông điệp chính ngay khi tải trang.
3. **Hero Section:** Tiêu đề mạnh mẽ + Nút hành động.
4. **Vấn Đề (Pain Points - NEW):** 4 thẻ (card) vấn đề khách quan (Đau mỏi, Mất ngủ, Thiếu năng lượng, Vóc dáng) kết hợp với icon SVG mỏng, giúp đánh trúng tâm lý người tập trước khi nói về giải pháp.
5. **Triết Lý (Philosophy):** Thông điệp về Thân-Tâm-Trí và Namaste.
6. **Kiến Thức (Poses):** Chi tiết về lợi ích của 3 tư thế trọng tâm: *Bánh xe, Camatkarasana, Puppy Pose*.
7. **Lịch Tập (Schedule):** Chi tiết lịch tập buổi sáng và chiều/tối (dành cho người lớn tuổi và cộng đồng).
8. **Không Gian (Gallery):** CSS Grid (9 ảnh đan xen lớn nhỏ) hiển thị không gian và học viên.
9. **Liên Hệ (Contact):** Thông tin địa chỉ và SĐT.
10. **Footer.**

## 5. Trạng Thái Triển Khai (Deployment)
- **Kho lưu trữ (Repository):** GitHub (`https://github.com/hungniwaco-stack/yoga-hoa-dao`)
- **Tên nhánh chính:** `master`
- **Môi trường Live (Production):** Vercel (`https://yoga-hoa-dao.vercel.app`)
- **Workflow:** Push code lên GitHub master branch sẽ tự động trigger Vercel build & deploy.

---
*Ghi chú cho AI: Bất cứ khi nào người dùng yêu cầu chỉnh sửa dự án này, hãy tuân thủ nghiêm ngặt các quy tắc thiết kế (màu sắc, font chữ) ở trên. Nếu cần bổ sung ảnh, hãy kiểm tra thư mục `Anh/` trước.*
