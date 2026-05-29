# Checklist Technical SEO: Hướng Dẫn Kiểm Tra Website Toàn Diện Chuẩn Google

## Technical SEO là gì?

Technical SEO là quá trình tối ưu các yếu tố kỹ thuật của website nhằm giúp công cụ tìm kiếm như Google dễ dàng thu thập dữ liệu (Crawl), lập chỉ mục (Index) và hiểu nội dung website. Một website có nội dung tốt nhưng nền tảng kỹ thuật yếu vẫn có thể gặp khó khăn trong việc đạt thứ hạng cao trên Google.

Việc xây dựng một checklist Technical SEO giúp doanh nghiệp, SEOer và quản trị website phát hiện sớm các lỗi kỹ thuật ảnh hưởng đến hiệu suất tìm kiếm và trải nghiệm người dùng.

---

# 1. Cấu Trúc Website Và Thanh Điều Hướng

Cấu trúc website đóng vai trò như bản đồ giúp người dùng và Google hiểu được mối quan hệ giữa các trang.

### Tiêu chí cần kiểm tra

* Cấu trúc website rõ ràng, phân cấp hợp lý.
* Danh mục và chuyên mục được tổ chức logic.
* Mỗi trang không nên cách trang chủ quá 3 lần nhấp chuột.
* Có Breadcrumb cho các trang nội dung.

### Lợi ích

* Google dễ crawl dữ liệu.
* Người dùng dễ tìm kiếm thông tin.
* Tăng khả năng phân phối sức mạnh Internal Link.

---

# 2. Đồng Bộ Phiên Bản Domain

Một website có thể tồn tại nhiều phiên bản:

* http://domain.com
* https://domain.com
* http://www.domain.com
* https://www.domain.com

Nếu không đồng bộ sẽ gây ra lỗi trùng lặp nội dung (Duplicate Content).

### Tiêu chí cần kiểm tra

* Chỉ sử dụng một phiên bản chính.
* Thiết lập chuyển hướng 301 cho các phiên bản còn lại.
* Phiên bản HTTPS phải được ưu tiên.

### Ví dụ

Tất cả các phiên bản phải chuyển hướng về:

https://www.domain.com

hoặc

https://domain.com

---

# 3. Đồng Bộ Phiên Bản URL

Nhiều website vô tình tạo ra nhiều URL khác nhau cho cùng một nội dung.

### Ví dụ

* domain.com/dich-vu
* domain.com/dich-vu/
* domain.com/DICH-VU

Google có thể xem đây là các URL khác nhau.

### Tiêu chí cần kiểm tra

* Thống nhất định dạng URL.
* Sử dụng URL thân thiện SEO.
* URL ngắn gọn, dễ đọc.
* Hạn chế tham số không cần thiết.

### Lợi ích

* Tránh Duplicate Content.
* Tập trung sức mạnh SEO cho một URL duy nhất.

---

# 4. Kiểm Tra Broken Links

Broken Link là các liên kết dẫn đến trang không tồn tại hoặc báo lỗi 404.

### Các loại Broken Link

* Internal Broken Links
* External Broken Links

### Tác hại

* Trải nghiệm người dùng kém.
* Google đánh giá chất lượng website thấp hơn.
* Lãng phí Crawl Budget.

### Cách kiểm tra

* Google Search Console
* Screaming Frog SEO Spider
* Ahrefs Site Audit
* Semrush Site Audit

### Cách khắc phục

* Cập nhật URL mới.
* Chuyển hướng 301.
* Loại bỏ liên kết không cần thiết.

---

# 5. Kiểm Tra Redirect Và Redirect Chain

Redirect giúp chuyển người dùng từ URL cũ sang URL mới.

### Các loại Redirect

#### 301 Redirect

Chuyển hướng vĩnh viễn.

#### 302 Redirect

Chuyển hướng tạm thời.

### Redirect Chain là gì?

Ví dụ:

URL A → URL B → URL C

Google phải đi qua nhiều bước trước khi đến URL cuối cùng.

### Tác hại

* Tăng thời gian tải trang.
* Mất một phần sức mạnh SEO.
* Gây khó khăn cho bot tìm kiếm.

### Tiêu chí tối ưu

Nên:

URL A → URL C

Không nên:

URL A → URL B → URL C → URL D

---

# 6. Robots.txt

Robots.txt là tệp hướng dẫn bot tìm kiếm truy cập hoặc không truy cập vào các khu vực cụ thể của website.

### Ví dụ

User-agent: *

Disallow: /admin/

Allow: /

### Kiểm tra

* Robots.txt có tồn tại hay không.
* Không chặn nhầm các trang cần index.
* Cho phép Google truy cập CSS và JavaScript.

### Lỗi thường gặp

* Chặn toàn bộ website bằng:

Disallow: /

Điều này khiến Google không thể lập chỉ mục website.

---

# 7. XML Sitemap

Sitemap là danh sách các URL quan trọng của website.

### Vai trò

* Giúp Google phát hiện URL nhanh hơn.
* Hỗ trợ index website mới.

### Tiêu chí cần kiểm tra

* Sitemap hoạt động bình thường.
* Không chứa URL lỗi 404.
* Không chứa URL Redirect.
* Chỉ chứa URL chuẩn (Canonical URL).

### Đường dẫn phổ biến

https://domain.com/sitemap.xml

### Công cụ kiểm tra

* Google Search Console
* Screaming Frog

---

# 8. Meta Robots

Meta Robots giúp kiểm soát việc Google lập chỉ mục từng trang.

### Các thuộc tính phổ biến

#### Index

Cho phép Google index trang.

<meta name="robots" content="index">

#### Noindex

Không cho phép index.

<meta name="robots" content="noindex">

#### Nofollow

Không truyền giá trị SEO qua liên kết.

<meta name="robots" content="nofollow">

### Kiểm tra

* Trang quan trọng không bị Noindex.
* Trang quản trị nên Noindex.
* Trang cảm ơn hoặc trang lọc sản phẩm nên cân nhắc Noindex.

---

# 9. SSL Và HTTPS

Google xem HTTPS là tín hiệu xếp hạng.

### Kiểm tra

* Website sử dụng SSL hợp lệ.
* Không có cảnh báo "Not Secure".
* Không tồn tại Mixed Content.

### Lợi ích

* Bảo mật dữ liệu người dùng.
* Tăng độ tin cậy.
* Hỗ trợ SEO.

---

# 10. Tốc Độ Tải Trang

Page Speed là yếu tố quan trọng trong Core Web Vitals.

### Chỉ số cần quan tâm

* Largest Contentful Paint (LCP)
* Interaction To Next Paint (INP)
* Cumulative Layout Shift (CLS)

### Công cụ kiểm tra

* Google PageSpeed Insights
* GTmetrix
* Lighthouse

### Cách tối ưu

* Nén ảnh.
* Sử dụng CDN.
* Giảm JavaScript không cần thiết.
* Kích hoạt Browser Cache.

---

# 11. Mobile-Friendly

Google hiện sử dụng Mobile-First Indexing.

### Kiểm tra

* Website hiển thị tốt trên điện thoại.
* Font chữ dễ đọc.
* Nút bấm đủ lớn.
* Không bị tràn màn hình.

### Công cụ

Google Mobile Friendly Test.

---

# 12. Trang 404

Trang 404 xuất hiện khi URL không tồn tại.

### Trang 404 tốt cần

* Thông báo rõ ràng.
* Có nút quay lại trang chủ.
* Có thanh tìm kiếm.
* Giữ nhận diện thương hiệu.

### Tránh

* Redirect toàn bộ lỗi 404 về trang chủ.
* Trang 404 trắng hoặc không có nội dung.

---

# 13. Canonical URL

Canonical giúp Google xác định URL chính.

### Ví dụ

<link rel="canonical" href="https://domain.com/dich-vu-seo">

### Lợi ích

* Tránh Duplicate Content.
* Tập trung sức mạnh SEO.

---

# 14. Schema Markup

Schema là dữ liệu có cấu trúc giúp Google hiểu nội dung tốt hơn.

### Các loại phổ biến

* Organization
* Local Business
* Product
* FAQ
* Article
* Breadcrumb

### Lợi ích

* Tăng khả năng hiển thị Rich Snippets.
* Cải thiện CTR.

---

# 15. Hreflang

Hreflang dành cho website đa ngôn ngữ.

### Ví dụ

* Tiếng Việt: vi-VN
* Tiếng Anh: en-US

### Mục đích

Giúp Google hiển thị đúng phiên bản ngôn ngữ cho người dùng từng quốc gia.

---

# Kết Luận

Technical SEO là nền móng của mọi chiến dịch SEO. Một website có nội dung chất lượng và backlink mạnh nhưng tồn tại nhiều lỗi kỹ thuật vẫn khó đạt được hiệu quả tối đa trên Google.

Checklist Technical SEO bao gồm các hạng mục quan trọng như:

* Cấu trúc website
* Domain và URL chuẩn hóa
* Broken Links
* Redirect
* Robots.txt
* Sitemap
* Meta Robots
* SSL
* Tốc độ tải trang
* Mobile-Friendly
* Trang 404
* Canonical
* Schema
* Hreflang

Việc kiểm tra định kỳ các yếu tố trên sẽ giúp website duy trì hiệu suất SEO ổn định, cải thiện khả năng index và nâng cao trải nghiệm người dùng.
