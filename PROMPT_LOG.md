# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)
- **Họ và tên:** Nguyễn Duy Phúc Lộc
- **MSSV:** 125001712
- **Tên đề tài Website:** Dashboard Cá nhân & Lộ trình Học tập (The Learning Path)
- **Công cụ AI đã sử dụng:** GitHub Copilot

## 1. Quá trình xây dựng và tinh chỉnh website
### Lần 1: Đề xuất cấu trúc Dashboard Cá nhân & Lộ trình Học tập
- **Prompt đã dùng:**
Tôi đang xây dựng website với đề tài “Dashboard Cá nhân & Lộ trình Học tập”.
Hãy đề xuất cấu trúc giao diện cho một trang dashboard học tập cá nhân, gồm:

Header chứa logo/tên hệ thống và navigation.
Khu vực chào mừng người học.
Tổng quan tiến độ học tập.
Danh sách các khóa học hoặc môn học.
Lộ trình học tập theo từng giai đoạn.
Biểu đồ cột thể hiện kết quả học tập.
Sidebar hoặc aside chứa mục tiêu, lịch học và thông tin nhanh.
Footer.
Website chỉ cần là giao diện frontend tĩnh, chưa cần backend, đăng nhập hoặc AI thật. Hãy ưu tiên bố cục rõ ràng, hiện đại và phù hợp với sinh viên.
- **Kết quả AI tạo ra:** Đề xuất cấu trúc dashboard gồm header và navigation, khu vực chào mừng, các thẻ tổng quan tiến độ, danh sách khóa học, lộ trình học tập theo giai đoạn, biểu đồ cột kết quả học tập, aside chứa mục tiêu/lịch học/thông tin nhanh và footer. Giao diện được định hướng theo frontend tĩnh, hiện đại, rõ ràng và phù hợp với sinh viên.
- **Nhận xét & Tinh chỉnh của SV:** Xác định cấu trúc nội dung trước khi triển khai Semantic HTML5, CSS Variables, layout responsive và các hiệu ứng giao diện.

### Lần 2: Tạo khung xương HTML5
- **Prompt đã dùng:** Tạo cho tôi khung xương vào index.html
- **Kết quả AI tạo ra:** Đã tạo khung HTML5 semantic cho Dashboard Cá nhân & Lộ trình Học tập trong `index.html`, gồm `header`, `nav`, `main`, `section`, `article`, `aside` và `footer`. Nội dung hiện là frontend tĩnh, chưa thêm CSS hoặc JavaScript.
- **Nhận xét & Tinh chỉnh của SV:** Hoàn thiện khung nội dung và cấu trúc semantic trước khi triển khai phần giao diện.

### Lần 3: Kiểm tra và làm lại khung HTML5 theo yêu cầu semantic
- **Prompt đã dùng:**
Dựa trên cấu trúc dashboard học tập đã đề xuất, hãy tạo khung HTML5 cho trang web.

Yêu cầu bắt buộc:

- Sử dụng `header`, `nav`, `main`, `section`, `article`, `aside` và `footer` đúng ngữ nghĩa.
- Chỉ sử dụng một thẻ `main`.
- Dùng `section` cho các khu vực lớn như tổng quan, lộ trình học tập và kết quả học tập.
- Dùng `article` cho từng khóa học hoặc từng chặng học tập.
- Dùng `aside` cho mục tiêu học tập, lịch học hoặc thông tin bổ trợ.
- Bổ sung `aria-label`, `aria-labelledby` khi phù hợp.
- Nội dung bằng tiếng Việt.
Kiểm tra và làm lại với yêu cầu này
- **Kết quả AI tạo ra:** Rà soát và làm lại khung `index.html`, giữ một thẻ `main`, dùng các thẻ semantic đúng vai trò, bổ sung nhãn ARIA cho các khu vực và nội dung tiếng Việt.
- **Nhận xét & Tinh chỉnh của SV:** Ưu tiên cấu trúc HTML rõ ràng, dễ tiếp tục phát triển CSS và đáp ứng đúng checklist semantic của đề bài.

### Lần 4: Tạo CSS nền tảng cho dashboard học tập
- **Prompt đã dùng:**
Hãy viết phần CSS nền tảng cho dashboard học tập.

Yêu cầu:
CSS kiểu external (thông qua thẻ link)
Chú ý: Không thay đổi cấu trúc Semantic HTML đã có.
Khai báo toàn bộ màu sắc, font, spacing, border-radius, shadow và transition trong :root.
Sử dụng phong cách hiện đại, sáng, chuyên nghiệp, phù hợp với sản phẩm giáo dục công nghệ.
Có màu chính, màu phụ, màu thành công, cảnh báo và màu nền.
Dùng var(--...) xuyên suốt CSS, không lặp lại các giá trị màu quan trọng.
Thiết lập box-sizing, typography, reset cơ bản và trạng thái focus dễ nhìn.
- **Kết quả AI tạo ra:** Thêm liên kết external `style.css` vào `index.html` và xây dựng CSS nền tảng responsive trong `style.css`, gồm CSS Variables, reset cơ bản, typography, layout Grid/Flexbox, màu trạng thái, card, focus-visible, responsive breakpoint và hỗ trợ giảm chuyển động.
- **Nhận xét & Tinh chỉnh của SV:** Giữ nguyên cấu trúc Semantic HTML đã có; chỉ bổ sung liên kết stylesheet và phần trình bày CSS.

### Lần 5: Mở rộng từ một trang chủ thành nhiều trang
- **Prompt đã dùng:** Trông có vẻ đơn giản. Có thể từ 1 trang chủ từ đó ra nhiều trang như Dashboard cá nhân, Lộ trình học tập và Thống kê điểm số không?
- **Kết quả AI tạo ra:** Xác nhận có thể phát triển website thành mô hình nhiều trang, gồm trang chủ, Dashboard cá nhân, Lộ trình học tập và Thống kê điểm số. Các trang có thể dùng chung CSS nền tảng, header, navigation và footer; mỗi trang tập trung vào một nhóm nội dung riêng.
- **Nhận xét & Tinh chỉnh của SV:** Mở rộng phạm vi theo hướng nhiều trang nhưng vẫn giữ cấu trúc rõ ràng, không cần backend và không can thiệp sâu ngoài phạm vi cần thiết.

### Lần 6: Triển khai cấu trúc website nhiều trang
- **Prompt đã dùng:** Tuyệt, hãy thực hiện đi.
- **Kết quả AI tạo ra:** Chuyển website sang cấu trúc nhiều trang gồm trang chủ, Dashboard cá nhân, Lộ trình học tập và Thống kê điểm số; dùng chung `style.css`, header, navigation và footer.
- **Nhận xét & Tinh chỉnh của SV:** Giữ giao diện frontend tĩnh, tổ chức nội dung thành các trang riêng để website rõ ràng và dễ mở rộng.

### Lần 7: Xây dựng layout responsive bằng CSS Grid và Flexbox
- **Prompt đã dùng:**
Hãy xây dựng layout responsive cho dashboard bằng CSS Grid và Flexbox.

Yêu cầu:

Desktop có khu vực nội dung chính và sidebar.
Khu vực tổng quan hiển thị các thẻ thống kê bằng CSS Grid.
Danh sách khóa học hiển thị dạng card.
Mobile chuyển về bố cục một cột.
Không sử dụng framework CSS.
Có breakpoint hợp lý cho tablet và mobile.
Các card không bị tràn ngang ở màn hình nhỏ.
Giữ nguyên các thẻ semantic HTML5 hiện có.
- **Kết quả AI tạo ra:** Rà soát và hoàn thiện layout responsive trong `style.css` bằng CSS Grid và Flexbox, gồm khu vực nội dung chính/sidebar trên desktop, lưới card thống kê và khóa học, breakpoint tablet/mobile, cùng các quy tắc chống tràn ngang.
- **Nhận xét & Tinh chỉnh của SV:** Giữ nguyên cấu trúc Semantic HTML5 và chỉ điều chỉnh phần layout CSS.

### Lần 8: Thu gọn thanh điều hướng trên màn hình nhỏ
- **Prompt đã dùng:** Hãy làm cho thanh điều hướng tự thu lại thành menu mở ra nếu kích thước bị thay đổi (như ở trên mobile)
- **Kết quả AI tạo ra:** Bổ sung menu hamburger responsive bằng HTML/CSS cho navigation của các trang, tự động hiển thị khi màn hình nhỏ và mở/đóng danh sách liên kết bằng thao tác người dùng.
- **Nhận xét & Tinh chỉnh của SV:** Giữ navigation dùng chung, hỗ trợ mobile và không cần framework hoặc JavaScript.

### Lần 9: Mở rộng menu mobile và menu quản lý tài khoản
- **Prompt đã dùng:** Menu nên to hơn và đưa ra giữa, ngoài ra tài khoản cũng sẽ thu nhỏ lại thành khung avatar tròn, chỉ hiện 2 chũ cuối của tên và khi click vào sẽ có một menu chi tiết quản lý
- **Kết quả AI tạo ra:** Điều chỉnh menu mobile lớn hơn và căn giữa; thay khu vực tên người dùng bằng avatar tròn hiển thị `PL`; thêm menu chi tiết quản lý tài khoản có thể mở khi nhấn vào avatar bằng HTML/CSS thuần.
- **Nhận xét & Tinh chỉnh của SV:** Giữ giao diện responsive, thao tác mở menu rõ ràng và không cần JavaScript hoặc framework.

### Lần 10: Căn chỉnh logo và avatar trên mobile
- **Prompt đã dùng:** Ở kích thước nhỏ như mobile thì icon avatar sẽ vẫn ở góc phải.
Logo và tên tiêu đề Learn Track sẽ đưa ra giữa. Lược bỏ dòng mô tả dưới tiêu đề LearnTrack
- **Kết quả AI tạo ra:** Ẩn dòng mô tả dưới logo trên toàn bộ trang; căn giữa logo trên mobile và giữ avatar cố định ở góc phải của header.
- **Nhận xét & Tinh chỉnh của SV:** Ưu tiên header mobile gọn, cân đối và giữ thao tác tài khoản luôn dễ tiếp cận.

### Lần 11: Cố định header một hàng trên cùng
- **Prompt đã dùng:** Hãy cho cả thanh menu, tên trang và phần icon avatar dàn cùng 1 hàng ngang, cố định ở phía trên đỉnh trang
- **Kết quả AI tạo ra:** Điều chỉnh header dùng chung thành thanh cố định ở phía trên; logo, nút menu và avatar nằm cùng một hàng ngang. Danh sách điều hướng trên mobile mở xuống bên dưới thanh header.
- **Nhận xét & Tinh chỉnh của SV:** Giữ header dễ sử dụng khi cuộn trang và không làm thay đổi nội dung Semantic HTML hiện có.

### Lần 12: Sửa chiều rộng menu mobile
- **Prompt đã dùng:** Menu bị vỡ giao diện chữ khi mở ra. Hãy sửa lại và cho thanh menu dài vừa đủ các tính năng có trong đó
- **Kết quả AI tạo ra:** Điều chỉnh menu mobile để chiều rộng tự phù hợp với nội dung, giới hạn theo chiều rộng màn hình và giữ chữ trên một dòng, tránh bị bó hẹp hoặc vỡ giao diện.
- **Nhận xét & Tinh chỉnh của SV:** Menu cần đủ rộng để hiển thị rõ các tính năng nhưng không được gây tràn ngang trên mobile.

### Lần 13: Thu gọn và căn trái nội dung menu
- **Prompt đã dùng:** Thanh menu quá rộng, căn nội dung lề trái và kích thước menu chỉ rộng hơn một xí vừa đủ thôi
- **Kết quả AI tạo ra:** Loại bỏ chiều rộng tối thiểu cố định của menu mobile, đặt chiều rộng theo nội dung với khoảng đệm nhỏ và căn các mục menu về bên trái.
- **Nhận xét & Tinh chỉnh của SV:** Menu cần gọn, vừa đủ nội dung và không tạo cảm giác chiếm quá nhiều diện tích.

### Lần 14: Tăng kích thước chữ và menu mobile
- **Prompt đã dùng:** Cho ksch thước chữ và menu to hơn vừa đủ xem đi, nhưng vẫn giữ cấu trúc như vậy
- **Kết quả AI tạo ra:** Tăng vừa phải kích thước chữ, padding và chiều rộng tự nhiên của menu mobile, giữ nguyên cấu trúc mở menu, căn trái nội dung và không gây tràn ngang.
- **Nhận xét & Tinh chỉnh của SV:** Menu cần dễ đọc hơn nhưng vẫn gọn và giữ nguyên cách hoạt động hiện tại.

### Lần 15: Tạo thanh tiến độ học tập bằng HTML và CSS thuần
- **Prompt đã dùng:**
> Hãy tạo các thanh tiến độ học tập bằng HTML và CSS thuần.
>
> Yêu cầu:
>
>
> - Mỗi khóa học có tên, phần trăm hoàn thành và progress bar.
> - Phần trăm được truyền qua CSS Variable, ví dụ `--progress: 75%`.
> - Thanh tiến độ phải có phần nền và phần đã hoàn thành.
> - Có animation khi trang tải, từ 0% đến giá trị mục tiêu.
> - Không dùng thư viện biểu đồ hoặc canvas.
> - Có màu khác nhau cho trạng thái đang học, hoàn thành và chưa bắt đầu.
> - Đảm bảo màu sắc và nhãn phần trăm vẫn dễ đọc.
> Ví dụ hướng triển khai:
> <div class="progress-item">
>   <div class="progress-label">
>     <span>HTML & CSS</span>
>     <strong>80%</strong>
>   </div>
>   <div class="progress-bar" role="progressbar"
>        aria-valuenow="80"
>        aria-valuemin="0"
>        aria-valuemax="100"
>        style="--progress: 80%">
>     <span></span>
>   </div>
> </div>
- **Kết quả AI tạo ra:** Bổ sung progress bar HTML/CSS thuần cho từng khóa học trên dashboard, truyền giá trị qua `--progress`, thêm animation từ 0% đến giá trị mục tiêu, hỗ trợ ba trạng thái đang học/đã hoàn thành/chưa bắt đầu và bổ sung thuộc tính ARIA cho khả năng tiếp cận.
- **Nhận xét & Tinh chỉnh của SV:** Hiển thị trực quan tiến độ từng khóa học, giữ màu sắc dễ đọc và không sử dụng thư viện biểu đồ hoặc canvas.

### Lần 16: Làm rõ khung các mục thông tin nhanh
- **Prompt đã dùng:** Mục thông tin nhanh các tiêu đề kiểu "Mục tiêu tuần này", "Lịch học sắp tới" cho viền khung chi tiết hơn
- **Kết quả AI tạo ra:** Tạo khung riêng cho từng mục trong phần thông tin nhanh bằng viền, bo góc, nền nhẹ, đổ bóng và màu nhấn cạnh trái khác nhau.
- **Nhận xét & Tinh chỉnh của SV:** Các nhóm mục tiêu, lịch học và thống kê cần được phân tách rõ ràng hơn để dễ quan sát.

### Lần 17: Tạo biểu đồ cột kết quả học tập bằng HTML và CSS thuần
- **Prompt đã dùng:**
> Hãy tạo biểu đồ cột thể hiện kết quả học tập bằng HTML và CSS thuần.
>
> Yêu cầu:
>
> Không sử dụng Chart.js, canvas hoặc thư viện biểu đồ.
> Mỗi cột sử dụng CSS Variable để biểu thị chiều cao, ví dụ --bar-height: 75%.
> Có nhãn môn học ở phía dưới và điểm/phần trăm ở phía trên.
> Biểu đồ có tiêu đề và phần mô tả ngắn.
> Biểu đồ không bị tràn trên mobile; cho phép cuộn ngang nếu cần.
> Có animation khi biểu đồ xuất hiện.
> Bổ sung thông tin thay thế hoặc mô tả để người dùng screen reader vẫn hiểu dữ liệu.
> Ví dụ:
> <div class="chart-column" style="--bar-height: 82%">
>   <span class="chart-value">82%</span>
>   <div class="chart-bar" aria-hidden="true"></div>
>   <span class="chart-label">HTML</span>
> </div>
- **Kết quả AI tạo ra:** Hoàn thiện biểu đồ cột CSS thuần trên trang thống kê, sử dụng `--bar-height`, nhãn phần trăm và môn học, mô tả dữ liệu cho screen reader, vùng cuộn ngang trên mobile và animation tuần tự khi biểu đồ xuất hiện.
- **Nhận xét & Tinh chỉnh của SV:** Giữ biểu đồ nhẹ, dễ đọc, responsive và không phụ thuộc Chart.js, canvas hoặc thư viện biểu đồ.

### Lần 18: Tạo khu vực Lộ trình học tập cho dashboard
- **Prompt đã dùng:**
> Hãy tạo khu vực “Lộ trình học tập” cho dashboard.
>
> Yêu cầu:
>
> Chia lộ trình thành các giai đoạn: Cơ bản, Thực hành, Dự án và Nâng cao.
> Mỗi giai đoạn dùng một article.
> Hiển thị trạng thái: đã hoàn thành, đang học và khóa tiếp theo.
> Dùng CSS để phân biệt các trạng thái.
> Có timeline hoặc đường nối trực quan bằng CSS.
> Nội dung thể hiện rõ môn học, mục tiêu và phần trăm hoàn thành.
> Thiết kế responsive trên mobile.
> Không thêm chức năng backend.
- **Kết quả AI tạo ra:** Bổ sung khu vực Lộ trình học tập vào dashboard với bốn `article` cho các giai đoạn Cơ bản, Thực hành, Dự án và Nâng cao; thêm trạng thái, mục tiêu, phần trăm hoàn thành, đường nối timeline bằng CSS và bố cục responsive. Trang lộ trình riêng cũng được đồng bộ nội dung.
- **Nhận xét & Tinh chỉnh của SV:** Giữ dữ liệu frontend tĩnh, giúp người học nhìn rõ giai đoạn hiện tại và bước tiếp theo trên cả desktop lẫn mobile.

### Lần 19: Hoàn tác hai thay đổi timeline gần nhất
- **Prompt đã dùng:** Hoàn tác lại trước đó. 2 prompt hồi nãy xem như không tồn tại và xoá khỏi log
- **Kết quả AI tạo ra:** Hoàn tác giao diện về trạng thái trước hai prompt timeline gần nhất và xóa hai mục nhật ký tương ứng.
- **Nhận xét & Tinh chỉnh của SV:** Hai prompt timeline gần nhất không được xem là một phần của lịch sử dự án.

### Lần 20: Tích hợp Animate.css và AOS không dùng JavaScript
- **Prompt đã dùng:**
> Hãy tích hợp Animate.css và AOS vào dashboard học tập hiện có.
>
> Yêu cầu:
>
> Animate.css áp dụng cho tiêu đề chính, khu vực hero, các nút CTA và thẻ thống kê.
> AOS áp dụng cho các section, article khóa học, learning path và biểu đồ.
> Thêm thuộc tính data-aos phù hợp như fade-up, fade-right hoặc zoom-in.
> Khởi tạo AOS bằng JavaScript với cấu hình nhẹ, không gây rối mắt.
> Không lạm dụng animation.
> Người dùng vẫn có thể đọc nội dung khi JavaScript bị tắt.
> Giữ nguyên CSS hover và focus tự viết.
>
> Yêu cầu không được sử dụng JavaScript, nên những lệnh nào có js thì ko thực hiện
- **Kết quả AI tạo ra:** Tích hợp Animate.css qua stylesheet CDN cho hero, tiêu đề, CTA và thẻ thống kê; thêm stylesheet AOS và các thuộc tính `data-aos` cho section, khóa học, learning path và aside. Vì yêu cầu không sử dụng JavaScript, không thêm lệnh khởi tạo AOS; CSS fallback giúp nội dung vẫn hiển thị và có hiệu ứng nhẹ khi JavaScript bị tắt.
- **Nhận xét & Tinh chỉnh của SV:** Ưu tiên ràng buộc không JavaScript và khả năng đọc nội dung; giữ nguyên các hiệu ứng hover/focus CSS hiện có.

### Lần 21: Sửa lỗi dashboard không hiển thị nội dung
- **Prompt đã dùng:** Dashboard không thấy gì cả
- **Kết quả AI tạo ra:** Sửa CSS fallback để các phần tử có `data-aos` kết thúc ở trạng thái hiển thị đầy đủ (`opacity: 1`, `transform: none`), tránh stylesheet AOS giữ nội dung ở trạng thái ẩn khi không có JavaScript khởi tạo.
- **Nhận xét & Tinh chỉnh của SV:** Dashboard phải luôn đọc được nội dung dù không sử dụng JavaScript.

### Lần 22: Thêm hiệu ứng cho trang lộ trình và thống kê
- **Prompt đã dùng:** Thêm hiệu ứng khi chuyển trang như vậy cho 2 trang lộ trình và thống kê đi
- **Kết quả AI tạo ra:** Đồng bộ Animate.css, thuộc tính `data-aos` và CSS fallback cho trang Lộ trình học tập và Thống kê điểm số; áp dụng hiệu ứng cho phần giới thiệu, card tổng quan, article lộ trình và các cột biểu đồ mà không thêm JavaScript.
- **Nhận xét & Tinh chỉnh của SV:** Hai trang cần có trải nghiệm chuyển đến đồng nhất với dashboard nhưng vẫn hiển thị nội dung khi JavaScript bị tắt.

### Lần 23: Đưa hoạt động gần đây lên đầu
- **Prompt đã dùng:** Đưa phần hoạt động gần đây lên đầu
- **Kết quả AI tạo ra:** Di chuyển section “Hoạt động gần đây” lên đầu khu vực nội dung dashboard, trước danh sách tiến độ khóa học; giữ nguyên nội dung, hiệu ứng và bố cục responsive.
- **Nhận xét & Tinh chỉnh của SV:** Ưu tiên hiển thị các cập nhật mới nhất trước khi người học xem danh sách khóa học.

### Lần 24: Rà soát và bổ sung hiệu ứng tương tác cho dashboard
- **Prompt đã dùng:**
> Hãy rà soát và bổ sung hiệu ứng tương tác cho dashboard.
>
> Yêu cầu:
>
> Card khóa học có hiệu ứng hover nhẹ.
> Button và link có hover, focus-visible và active rõ ràng.
> Không chỉ dùng màu để biểu thị trạng thái.
> Có outline dễ nhìn khi điều hướng bằng bàn phím.
> Không dùng hiệu ứng làm nội dung nhảy hoặc thay đổi layout mạnh.
> Kiểm tra độ tương phản cơ bản giữa chữ và nền.
- **Kết quả AI tạo ra:** Giảm độ dịch chuyển hover của card, bổ sung trạng thái `:active` cho link/button, tăng khả năng nhận biết focus bằng outline hiện có, thêm ký hiệu trạng thái bằng CSS bên cạnh nhãn chữ và giữ nguyên layout khi tương tác.
- **Nhận xét & Tinh chỉnh của SV:** Ưu tiên tương tác nhẹ, dễ sử dụng bằng bàn phím và không phụ thuộc riêng vào màu sắc.

### Lần 25: Thêm chỉ báo tăng giảm cho tổng quan kết quả
- **Prompt đã dùng:** Phần tổng quan kết quả thêm những chữ số, hoặc biểu tượng kiểu tăng (với màu xanh là) và giảm (với màu đỏ) để thể hiện sự tăng giảm với trước đó.
- **Kết quả AI tạo ra:** Bổ sung chỉ báo xu hướng tăng/giảm cho từng thẻ Tổng quan kết quả bằng số liệu, biểu tượng mũi tên, nhãn chữ và màu xanh/đỏ; thêm `aria-label` để screen reader hiểu mức thay đổi so với tháng trước.
- **Nhận xét & Tinh chỉnh của SV:** Thông tin tăng giảm cần được thể hiện bằng cả văn bản và biểu tượng, không phụ thuộc riêng vào màu sắc.

### Lần 26: Đổi tên thương hiệu
- **Prompt đã dùng:** Đổi tên thành LHULearnTrack.
- **Kết quả AI tạo ra:** Đổi tên thương hiệu hiển thị trên toàn bộ website từ LearnTrack thành LHULearnTrack, gồm logo, tiêu đề trang, mô tả truy cập và footer.
- **Nhận xét & Tinh chỉnh của SV:** Tên thương hiệu mới cần được đồng bộ trên tất cả các trang.

### Lần 27: Bổ sung thông tin liên hệ vào footer
- **Prompt đã dùng:** Thêm footer có chứa thông tin dạng như địa chỉ, sđt liên hệ,... sử dụng cùng tông màu với trang. Vẫn giữ nguyên mục © 2026 LHULearnTrack - Dashboard học tập cá nhân.
- **Kết quả AI tạo ra:** Bổ sung tên thương hiệu, địa chỉ, số điện thoại và email vào footer của cả bốn trang; giữ nguyên dòng bản quyền và thiết kế footer bằng tông màu tím-xanh đồng nhất với website.
- **Nhận xét & Tinh chỉnh của SV:** Footer cần cung cấp thông tin liên hệ rõ ràng, dễ đọc và vẫn giữ nội dung bản quyền hiện tại.

### Lần 28: Kéo dài footer toàn bộ chiều ngang
- **Prompt đã dùng:** Footer phải kéo dài hết phần ngang cuối trang
- **Kết quả AI tạo ra:** Đặt footer rộng 100% viewport, bỏ giới hạn chiều rộng và căn phần nội dung theo khung tối đa 1200px; giữ nguyên màu sắc, thông tin liên hệ và responsive.
- **Nhận xét & Tinh chỉnh của SV:** Nền và đường viền footer cần phủ kín toàn bộ chiều ngang cuối trang.

### Lần 29: Chuyển footer thành khung chữ nhật không viền
- **Prompt đã dùng:** làm thành khung chủ nhật, không cần viền đâu
- **Kết quả AI tạo ra:** Giữ footer phủ toàn bộ chiều ngang, loại bỏ đường viền và bo góc để footer hiển thị như một khối chữ nhật liền mạch.
- **Nhận xét & Tinh chỉnh của SV:** Footer cần đơn giản, không có đường viền bao quanh.

### Lần 30: Sắp xếp lại liên kết footer và đổi địa chỉ
- **Prompt đã dùng:** 2 mục trang chủ và liên hệ đưa xuống dưới sau mục điện thoại, đổi địa chỉ thành đường Huỳnh Văn Nghệ, phường Trấn Biên, TP Đồng Nai
- **Kết quả AI tạo ra:** Đưa hai liên kết Trang chủ và Liên hệ xuống sau thông tin điện thoại, giữ email ở phần tiếp theo và đổi địa chỉ trên toàn bộ footer thành Đường Huỳnh Văn Nghệ, phường Trấn Biên, TP Đồng Nai.
- **Nhận xét & Tinh chỉnh của SV:** Footer cần hiển thị thông tin liên hệ theo thứ tự địa chỉ, điện thoại, liên kết và email.

### Lần 31: Căn chỉnh thông tin footer trên cùng một hàng
- **Prompt đã dùng:** Địa chỉ rồi tới điện thoại, rồi email rồi trang chủ và liên hệ nằm ngang cùng 1 hàng ấy, dòng 2026 LHU để bên phải ấy
- **Kết quả AI tạo ra:** Gom địa chỉ, điện thoại, email, Trang chủ và Liên hệ vào một hàng thông tin trong footer; đẩy dòng bản quyền sang bên phải trên desktop và cho phép tự xuống dòng trên mobile.
- **Nhận xét & Tinh chỉnh của SV:** Footer cần trình bày thông tin liên hệ theo một hàng ngang rõ ràng, còn bản quyền nằm tách về phía bên phải.

### Lần 32: Tách dòng thông tin điện thoại và email
- **Prompt đã dùng:** Điện thoại xuống dòng rồi email xuống dòng
- **Kết quả AI tạo ra:** Xếp địa chỉ, số điện thoại và email thành các dòng riêng trong footer; giữ các liên kết Trang chủ và Liên hệ nằm ngang.
- **Nhận xét & Tinh chỉnh của SV:** Thông tin liên hệ cần dễ đọc hơn bằng cách tách từng mục thành một dòng.

### Lần 33: Bổ sung ảnh chụp thật và icon công nghệ
- **Prompt đã dùng:** Bạn hãy kiếm ảnh minh hoạ từ trên Internet và lấy cái thực, không lấy kiểu vector. Kiếm luôn các icon cho HMTL, JSS,... trong mục dashboard cá nhân. Chuyển đổi tất cả thành webp
- **Kết quả AI tạo ra:** Tải ảnh chụp góc học tập thực tế từ Unsplash và các biểu tượng HTML5, CSS3, JavaScript, GitHub, React từ Devicon; lưu tất cả tài nguyên cục bộ trong `assets/` dưới định dạng WebP. Tích hợp ảnh vào khu vực chào mừng và icon vào các thẻ khóa học trong dashboard.
- **Nhận xét & Tinh chỉnh của SV:** Ưu tiên ảnh chụp thực tế thay cho hình minh hoạ vector; tài nguyên được chuyển đổi sang WebP để giảm dung lượng và không phụ thuộc lúc hiển thị vào CDN.

### Lần 34: Chuyển ảnh góc học tập thành background
- **Prompt đã dùng:** Arnh study workspace thành background ấy
- **Kết quả AI tạo ra:** Chuyển `study-workspace.webp` thành ảnh nền cho khu vực chào mừng trên dashboard, thêm lớp phủ màu để nội dung chữ vẫn dễ đọc và bỏ khung ảnh riêng.
- **Nhận xét & Tinh chỉnh của SV:** Ảnh minh hoạ phù hợp hơn khi được dùng làm background cho hero/dashboard welcome.

### Lần 35: Phân tích website và cập nhật README
- **Prompt đã dùng:** Phân tích trang web và tạo nội dung vào file readme. Sau đó push toàn bộ lên repo của tôi.
- **Kết quả AI tạo ra:** Phân tích cấu trúc, giao diện, công nghệ, khả năng responsive, accessibility, tài nguyên hình ảnh và giới hạn hiện tại; sau đó cập nhật `README.md` với hướng dẫn và mô tả dự án.
- **Nhận xét & Tinh chỉnh của SV:** README cần phản ánh đúng trạng thái website frontend tĩnh và cấu trúc tài nguyên hiện tại.

### Lần 36: Rà soát checklist kỹ thuật tối thiểu
- **Prompt đã dùng:** II. YÊU CẦU KỸ THUẬT VÀ KHUNG TỐI THIỂU CỦA WEBSITE ... Rà soát lại xem đã có đủ như yêu cầu chưa
- **Kết quả AI tạo ra:** Kiểm tra semantic HTML5, CSS Variables, Grid/Flexbox, Animate.css, AOS, hover và focus trên toàn bộ website; đồng bộ liên kết thư viện, class Animate.css và thuộc tính `data-aos` cho trang chủ.
- **Nhận xét & Tinh chỉnh của SV:** Giữ website không dùng JavaScript nên AOS CDN được kết hợp với fallback CSS hiện có để nội dung vẫn hiển thị khi không có JavaScript.

### Lần 37: Bổ sung thông tin sinh viên vào prompt log
- **Prompt đã dùng:** Bổ sung tên Nguyễn Duy Phúc Lộc và MSSV 125001712 vào prompt log và push luôn đi
- **Kết quả AI tạo ra:** Cập nhật họ tên và MSSV ở phần thông tin đầu file `PROMPT_LOG.md`.
- **Nhận xét & Tinh chỉnh của SV:** Thông tin sinh viên cần được điền đầy đủ để hoàn thiện hồ sơ bài tập.
