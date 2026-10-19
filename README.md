# LHULearnTrack

LHULearnTrack là website frontend tĩnh hỗ trợ sinh viên theo dõi tiến độ học tập, lộ trình phát triển kỹ năng và kết quả theo từng môn học. Website được xây dựng theo hướng trực quan, responsive và ưu tiên khả năng đọc trên máy tính, máy tính bảng và điện thoại.

## 1. Tổng quan website

Website gồm bốn trang chính:

| Trang | Tệp | Nội dung |
| --- | --- | --- |
| Trang chủ | `index.html` | Giới thiệu sản phẩm, các tính năng chính và liên kết nhanh đến dashboard |
| Dashboard cá nhân | `dashboard.html` | Lời chào, tổng quan tiến độ, hoạt động gần đây, khóa học, lộ trình và thông tin nhanh |
| Lộ trình học tập | `learning-path.html` | Timeline bốn giai đoạn: Cơ bản, Thực hành, Dự án và Nâng cao |
| Thống kê điểm số | `statistics.html` | Tổng quan điểm, chỉ báo tăng/giảm, biểu đồ kết quả theo môn và gợi ý học tập |

## 2. Cấu trúc thư mục

```text
.
├── index.html
├── dashboard.html
├── learning-path.html
├── statistics.html
├── style.css
├── PROMPT_LOG.md
├── README.md
└── assets/
    ├── study-workspace.webp
    ├── html5.webp
    ├── css3.webp
    ├── javascript.webp
    ├── github.webp
    └── react.webp
```

## 3. Phân tích kỹ thuật

### Semantic HTML5

Các trang sử dụng các phần tử semantic phù hợp:

- `header`: thương hiệu, navigation và menu tài khoản.
- `nav`: điều hướng chính và liên kết hỗ trợ ở footer.
- `main`: vùng nội dung chính, chỉ sử dụng một `main` trên mỗi trang.
- `section`: nhóm nội dung lớn như tổng quan, khóa học, lộ trình và biểu đồ.
- `article`: từng thẻ khóa học, giai đoạn học tập và thẻ thống kê.
- `aside`: khu vực thông tin nhanh trên dashboard.
- `footer`: thông tin liên hệ, liên kết và bản quyền.

Các tiêu đề được liên kết bằng `aria-labelledby`; các thanh tiến độ và biểu đồ có nhãn ARIA để hỗ trợ trình đọc màn hình.

### CSS và responsive layout

Toàn bộ giao diện dùng [style.css](./style.css), không sử dụng framework CSS. Các đặc điểm chính:

- CSS Variables trong `:root` cho màu sắc, font, khoảng cách, bo góc, shadow và transition.
- CSS Grid cho overview, danh sách khóa học, dashboard và biểu đồ.
- Flexbox cho header, navigation, footer, progress label và các nhóm liên kết.
- Breakpoint tại desktop, tablet và mobile.
- Menu mobile sử dụng checkbox và CSS, không cần JavaScript.
- Biểu đồ cột được dựng bằng CSS thuần.
- Footer full width, không viền, có thông tin địa chỉ, điện thoại, email và liên kết.

### Animation và tương tác

- Animate.css được liên kết để tạo hiệu ứng cho tiêu đề, hero, CTA và thẻ thống kê.
- Các phần tử có `data-aos` để thể hiện ý định hiệu ứng cuộn. Website không thêm JavaScript và không gọi `AOS.init()`, vì vậy nội dung vẫn hiển thị bình thường khi JavaScript bị tắt.
- Hover, focus-visible và active được viết bằng CSS.
- Focus keyboard có outline màu tương phản.
- Hiệu ứng hover chỉ dịch chuyển nhẹ, không làm thay đổi mạnh bố cục.
- Có hỗ trợ `prefers-reduced-motion` để giảm chuyển động khi người dùng bật tùy chọn hệ điều hành.

## 4. Tài nguyên hình ảnh

- `study-workspace.webp` là ảnh chụp thực tế góc học tập, được dùng làm background cho khu vực chào mừng của dashboard.
- Các tệp `html5.webp`, `css3.webp`, `javascript.webp`, `github.webp` và `react.webp` là icon công nghệ dùng trong các thẻ khóa học.
- Tất cả tài nguyên trong thư mục `assets/` đã được lưu dưới định dạng WebP để giảm dung lượng và sử dụng cục bộ trong website.
- Ảnh background có lớp phủ gradient nhằm duy trì độ tương phản giữa chữ và hình nền.

## 5. Cách chạy

Đây là website tĩnh nên không cần backend hoặc bước build:

1. Mở trực tiếp `index.html` bằng trình duyệt; hoặc
2. Mở thư mục dự án trong VS Code và chạy bằng một static server nếu muốn kiểm tra navigation qua HTTP.

Các thư viện Animate.css và AOS hiện được tham chiếu qua CDN trong những trang có animation. Nếu chạy khi không có Internet, phần nội dung và CSS chính vẫn hiển thị; chỉ các stylesheet CDN mới không tải được.

## 6. Giới hạn hiện tại

- Dữ liệu khóa học, điểm số và hoạt động đang là dữ liệu mẫu tĩnh.
- Chưa có backend, tài khoản thật, cơ sở dữ liệu hoặc chức năng lưu tiến độ.
- Menu tài khoản và các liên kết hồ sơ/cài đặt hiện phục vụ mục đích minh họa giao diện.
- Biểu đồ là bản trình bày CSS, chưa kết nối với dữ liệu động.
- Không sử dụng JavaScript tùy chỉnh theo yêu cầu của dự án.

## 7. Nhật ký phát triển

Quá trình xây dựng, các prompt và các lần tinh chỉnh được ghi trong [PROMPT_LOG.md](./PROMPT_LOG.md).

