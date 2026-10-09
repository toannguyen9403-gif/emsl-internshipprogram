# Website EMSL Intern — Version-3

Version-3 là một bản sao riêng được phát triển từ nội dung của Version-2. Toàn bộ mã nguồn, dữ liệu và ảnh cần để chạy website nằm trong thư mục này.

## Cấu trúc thư mục

| File / thư mục | Vai trò |
|---|---|
| `index.html` | Giao diện website, điều hướng, bản dịch mặc định và chế độ chỉnh sửa `?edit`. |
| `content.json` | Nội dung chương trình, nghiên cứu, liên hệ, ảnh, đường dẫn và các thay đổi xuất từ chế độ chỉnh sửa. |
| `assets/` | Toàn bộ ảnh và tài nguyên hình ảnh dùng trên website. |
| `README.md` | Hướng dẫn sử dụng và cập nhật bản này. |

## Điều hướng trong Version-3

Thanh điều hướng chính gồm **Home — Programs — Research Topics — Contact**. Programs là nút mở menu con, không mở một trang chứa tất cả thông tin chương trình. Khi đưa chuột vào Programs trên máy tính, menu hiện đúng ba mục: **Upcoming Program — Past Programs — About IRIP**. Có thể bấm nút Programs hoặc dùng bàn phím để mở menu; trên điện thoại, chạm Programs để mở menu con rồi chọn mục cần xem.

Khi chọn một mục, website chỉ hiển thị nội dung thuộc mục đó; các trang khác được ẩn.

| Mục điều hướng | Nội dung hiển thị |
|---|---|
| Home | Trang giới thiệu đầu website. |
| Programs → Upcoming Program | Chương trình sắp tới. |
| Programs → Past Programs | Các kỳ thực tập đã diễn ra và nội dung liên quan đến từng kỳ. |
| Programs → About IRIP | Giới thiệu mở rộng về chương trình, bốn khối trải nghiệm, Life in Seoul và FAQ đã có nội dung. |
| Research Topics | Chủ đề nghiên cứu và các tab phòng thí nghiệm. |
| Contact | Thông tin liên hệ, website liên quan và bản đồ. |

**Program Timeline đã được xóa**, bao gồm phần nội dung và các thành phần chỉnh sửa liên quan. Life in Seoul đã được chuyển từ Home sang About IRIP; phần Program Overview cũ được phát triển thành phần giới thiệu mở rộng tại About IRIP. FAQ được giữ tại About IRIP để bảo toàn thông tin có ích, nhưng không có mục điều hướng riêng. Khi dữ liệu FAQ chưa được điền, phần này có thể được ẩn trong chế độ xem thông thường.

Việc chuyển mục diễn ra ngay trong trình duyệt, không tải lại toàn bộ trang. Địa chỉ dùng phần sau dấu `#` để ghi nhớ mục đang xem:

| Địa chỉ | Trang được mở |
|---|---|
| `#home` | Home. |
| `#upcoming` | Upcoming Program. |
| `#archive` | Past Programs. |
| `#about-irip` | About IRIP. |
| `#research` | Research Topics. |
| `#contact` | Contact. |

Các liên kết cũ `#programs` được chuyển sang Upcoming Program; `#overview` và `#life` mở About IRIP. Có thể dùng nút Back/Forward của trình duyệt để trở lại trang trước. Các liên kết đến phần cụ thể, chẳng hạn một kỳ thực tập đã diễn ra, sẽ mở đúng trang chứa phần đó.

## Nội dung About IRIP

Phần mở đầu giới thiệu IRIP là chương trình mùa hè dự kiến tổ chức hằng năm tại Seoul, cùng ba thông tin nổi bật: **6 tuần trong phòng thí nghiệm — mentor 1:1 — 100% tiếng Anh cho hoạt động học thuật**. Bốn khối nội dung bên dưới trình bày quy trình nghiên cứu và hỗ trợ từ mentor; phương pháp, báo cáo hằng tuần và cơ hội phát triển kết quả thành bài báo SCI/SCIE hoặc báo cáo hội nghị; cộng đồng học thuật dùng tiếng Anh; trải nghiệm đời sống và văn hóa Seoul. Cơ hội công bố được diễn đạt là khả năng phát triển từ kết quả nghiên cứu.

Phần giới thiệu và bốn khối có đủ bản EN/VI/KO. Trong nhóm **Bố cục** của Edit, `layout.valueCols` nhận **1 hoặc 2** cột cho About IRIP; màn hình điện thoại tự xếp các khối thành một cột.

## Bố cục Home và chân trang

Phần giới thiệu Home, đường kẻ ngang và dòng thông tin bên dưới được căn giữa trong cùng một khung nội dung. Tiêu đề giữ **SSU-UED** liền với tên chương trình; bản tiếng Anh được bố trí trên một đến hai dòng ở màn hình máy tính và tự xuống dòng theo chiều rộng điện thoại. Tên trên thanh điều hướng dùng thống nhất **SSU-UED** với dấu gạch nối thông thường.

Mục **Quick links** ở chân trang chỉ gồm **Home — About IRIP — Contact**. Cột **Program archive** riêng vẫn giữ liên kết tới các kỳ thực tập. Chân trang dùng ba cột nội dung thực trên máy tính và tự chuyển bố cục cho màn hình nhỏ. Các thay đổi bố cục này giữ nguyên ba mục con Programs và cơ chế chỉ hiện nội dung thuộc trang được chọn.

## Apply đang được ẩn

Nút Apply, các liên kết Apply và toàn bộ phần Apply được ẩn trong bản này, kể cả khi mở `?edit`. Các trường chỉnh sửa đường dẫn Apply và ảnh QR cũng được bỏ khỏi bảng chỉnh sửa để phù hợp với giao diện hiện tại.

Dữ liệu và phần mã nguồn liên quan đến Apply vẫn được giữ lại để có thể khôi phục về sau. Nhập một đường dẫn Apply vào `content.json` không tự làm nút hoặc phần Apply xuất hiện. Khi muốn mở lại tính năng này, cần yêu cầu người sửa mã nguồn cập nhật cơ chế hiển thị trong `index.html`.

## Chạy thử trên máy

Nên mở website qua một máy chủ HTTP cục bộ để trình duyệt tải được `content.json` đầy đủ. Mở terminal tại thư mục Version-3 rồi chạy, nếu máy đã có Python:

```powershell
python -m http.server 8000
```

Sau đó mở:

```text
http://localhost:8000/
```

Để chỉnh sửa nội dung:

```text
http://localhost:8000/?edit
```

Có thể thêm mục cần xem, ví dụ `http://localhost:8000/?edit#about-irip`. Dừng máy chủ bằng `Ctrl+C` trong terminal. Nếu cổng 8000 đang được dùng, chọn cổng khác trong lệnh và địa chỉ trình duyệt.

Mở `index.html` bằng cách nhấp đúp có thể khiến trình duyệt chặn việc đọc `content.json`. Vì vậy, cách mở trực tiếp file không phù hợp để kiểm tra dữ liệu đã chỉnh sửa.

## Đưa lên GitHub Pages hoặc hosting tĩnh

1. Tải toàn bộ nội dung trong thư mục Version-3 lên thư mục được dùng để phục vụ website: `index.html`, `content.json` và cả thư mục `assets/`.
2. Giữ nguyên vị trí tương đối của các file. Ví dụ, ảnh `assets/campus-view.jpg` phải nằm trong thư mục `assets` bên cạnh `index.html`.
3. Đợi hosting cập nhật rồi mở địa chỉ website để kiểm tra bốn mục điều hướng và các ngôn ngữ.

Nếu muốn lưu nhiều phiên bản cạnh nhau trên hosting, có thể tải nguyên thư mục Version-3 lên và truy cập bằng đường dẫn tương ứng. Cơ chế chuyển mục bằng `#` không yêu cầu cấu hình chuyển hướng riêng trên máy chủ.

## Chỉnh sửa nội dung bằng `?edit`

Thêm `?edit` vào địa chỉ website để mở bảng chỉnh sửa. Khi địa chỉ đã có một mục sau dấu `#`, đặt `?edit` trước dấu `#`, ví dụ:

```text
https://<tên-bạn>.github.io/<tên-repo>/?edit#about-irip
```

1. Chọn Home, Research Topics hoặc Contact; với nội dung chương trình, mở menu Programs rồi chọn Upcoming Program, Past Programs hoặc About IRIP để xem đúng phần cần sửa.
2. Chọn EN, VI hoặc KR trên website hoặc trong bảng chỉnh sửa. Nội dung có bản dịch được sửa theo ngôn ngữ đang chọn.
3. Nhập nội dung trong bảng hoặc sửa trực tiếp chữ trên trang khi chế độ sửa trực tiếp đang bật. Nút bút chì trên các khối nội dung mở nhanh trường tương ứng trong bảng.
4. Bấm **Tải file content.json** để tải dữ liệu đã sửa về máy.
5. Thay `content.json` của bản Version-3 đang triển khai bằng file vừa tải. Nếu có ảnh mới, tải cả các ảnh mới vào `assets/`.
6. Tải lại website để kiểm tra kết quả.

Thay đổi trong bảng được lưu dưới dạng bản nháp trong trình duyệt; bản nháp không tự cập nhật file trên máy hoặc website đã triển khai. Phải xuất và thay `content.json` để lưu nội dung vào bộ website.

Nhóm **About IRIP (EN/VI/KO)** trong bảng Edit có các trường riêng cho phần mở đầu, thông tin nổi bật và bốn khối nội dung theo ngôn ngữ đang chọn. Bút chì trên khối mở đúng nhóm này; sửa chữ trực tiếp trên trang và nhập trong bảng dùng chung dữ liệu và đồng bộ với nhau. Khi xuất, các thay đổi nằm trong `content.json` tại `text.en`, `text.vi` hoặc `text.ko`. Cập nhật từng ngôn ngữ khi thay đổi nội dung.

Version-3 dùng khóa lưu ngôn ngữ và bản nháp riêng, tách khỏi Version-2. Bản nháp thuộc trình duyệt và địa chỉ website đang dùng; khi đổi trình duyệt, thiết bị hoặc địa chỉ triển khai, bản nháp cũ có thể không có ở nơi mới. Nút xóa bản nháp chỉ xóa bản nháp của Version-3.

## Ngôn ngữ

Website hỗ trợ **EN — tiếng Anh, VI — tiếng Việt, KR — tiếng Hàn**. Cả ba ngôn ngữ dùng chung cấu trúc bốn mục chính, ba mục con trong Programs và cùng cơ chế ẩn Apply. Tên menu và nội dung được hiển thị theo ngôn ngữ đang chọn.

Những nội dung có trường ngôn ngữ riêng phải được cập nhật cho từng bản. Nếu một trường chưa có bản dịch, website có thể dùng nội dung tiếng Anh làm dự phòng. Những trường dữ liệu chung, như email, số điện thoại, ngày tháng, tên kỳ và đường dẫn ảnh, được dùng chung giữa các ngôn ngữ theo cấu trúc `content.json` hiện tại.

Đổi ngôn ngữ trong khi đang xem một mục vẫn giữ người xem trong mục đó; không làm các mục khác xuất hiện cùng lúc.

## Chỉnh `content.json` trực tiếp

Có thể mở `content.json` bằng trình soạn thảo hoặc công cụ chỉnh sửa file trên GitHub. Giữ đúng cú pháp JSON: chuỗi dùng dấu nháy kép, các mục cách nhau bằng dấu phẩy và không có dấu phẩy thừa sau mục cuối.

| Nhóm dữ liệu | Nội dung |
|---|---|
| `config` | Kỳ sắp tới, liên hệ, đường dẫn, ảnh và bố cục. |
| `programs` | Các kỳ thực tập và thông tin lưu trữ. |
| `testimonials` | Thông tin sinh viên, đề tài, hoạt động và kết quả. |
| `topics` | Chủ đề nghiên cứu và nội dung theo ngôn ngữ. |
| `faq` | Câu hỏi và câu trả lời theo ngôn ngữ. |
| `seoul` | Các khung ảnh Life in Seoul. |
| `text` | Những thay đổi chữ và bản dịch được xuất từ chế độ chỉnh sửa. |

Sau khi sửa file trực tiếp, kiểm tra lại website qua HTTP và trong cả EN/KR. Nếu đang mở `?edit` mà vẫn thấy nội dung cũ, bản nháp của trình duyệt có thể đang được áp dụng; xuất nội dung cần giữ rồi xóa bản nháp để đọc lại dữ liệu triển khai.

## Ảnh và nội dung chưa điền

- Đặt ảnh trong `assets/` và ghi đường dẫn đầy đủ tương đối trong dữ liệu, ví dụ `assets/campus-view.jpg`.
- Ưu tiên tên file chữ thường, không dấu và không khoảng trắng để dễ triển khai.
- Khi kéo thả ảnh trong `?edit`, ảnh được xem trước ngay trong trình duyệt. Cần tải ảnh đã đổi tên và tải chúng lên `assets/` cùng với `content.json` đã xuất.
- Nội dung trong ngoặc vuông, như `[Student Name]`, là chỗ giữ chỗ. Các phần chưa có dữ liệu thật có thể được ẩn trong chế độ xem thông thường và hiện để chỉnh sửa trong `?edit`.
- Quy tắc chỗ giữ chỗ không làm Apply xuất hiện: phần Apply vẫn bị ẩn theo cấu hình giao diện của Version-3.

## Kiểm tra sau khi cập nhật

1. Thanh điều hướng có đúng bốn mục chính. Đưa chuột vào Programs mở đúng ba mục con; chạm trên điện thoại cũng mở được menu.
2. Upcoming Program chỉ hiện chương trình sắp tới; Past Programs chỉ hiện các kỳ đã diễn ra; About IRIP chứa phần giới thiệu mở rộng, bốn khối trải nghiệm và Life in Seoul, cùng FAQ đã được điền. Home không còn Life in Seoul.
3. Không có Program Timeline trong nội dung website hoặc trong các thành phần chỉnh sửa.
4. Apply không xuất hiện ở thanh điều hướng, nội dung, chân trang hoặc chế độ `?edit`.
5. Chuyển EN/VI/KR vẫn giữ trang đang xem và hiển thị đúng bản dịch; đổi ngôn ngữ không làm các trang khác hiện cùng lúc.
6. Mở trực tiếp `#upcoming`, `#archive`, `#about-irip` và kiểm tra liên kết cũ `#programs`, `#overview`, `#life` mở đúng trang. Các liên kết đến kỳ thực tập và nút Back/Forward vẫn hoạt động.
7. Ảnh, bản đồ và nội dung xuất qua `?edit` vẫn còn sau khi thay `content.json` và tải lại website.
8. Trên Home, tiêu đề, đường kẻ ngang và dòng thông tin cùng căn giữa; tiêu đề không bị cắt hoặc tràn ngang trên điện thoại. Tên thanh điều hướng là SSU-UED.
9. Quick links có đúng Home, About IRIP và Contact; cột Program archive vẫn hiện các kỳ. Chân trang không để lại cột trống trên máy tính.
10. About IRIP có đủ bản dịch; sửa tại bảng hoặc trực tiếp trên trang đều đồng bộ và được xuất trong `text` của `content.json`. Bố cục 1/2 cột hoạt động trên máy tính và xếp một cột trên điện thoại.
