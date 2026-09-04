[README.md](https://github.com/user-attachments/files/31819723/README.md)
# Website EMSL International Research Internship

Thư mục này là **bản hoàn chỉnh, chạy được ngay**. Chỉ cần đưa toàn bộ nội dung
bên trong lên GitHub là trang hoạt động.

## Thư mục có gì

| File / thư mục | Vai trò |
|---|---|
| `index.html` | Toàn bộ giao diện và mã nguồn trang web. Hiếm khi cần sửa. |
| `content.json` | **Toàn bộ nội dung chữ, ảnh, link.** Đây là file bạn sẽ sửa thường xuyên. |
| `assets/` | Tất cả hình ảnh. Tên file đã đổi thành chữ thường, không dấu, không khoảng trắng. |
| `README.md` | File này. Không ảnh hưởng tới website. |

## Cách đưa lên GitHub

1. Mở repository của bạn trên github.com
2. Bấm **Add file** → **Upload files**
3. Kéo thả `index.html`, `content.json` và **cả thư mục `assets`** vào
4. Kéo xuống dưới, bấm **Commit changes**

> Nếu repo đã có bản cũ, cứ upload đè lên — GitHub sẽ tự thay thế.

## Hai cách sửa nội dung

### Cách 1 — Sửa trực tiếp trên trang (dễ nhất)

Thêm `?edit` vào cuối địa chỉ web, ví dụ:

```
https://<tên-bạn>.github.io/<tên-repo>/?edit
```

Một bảng điều khiển tiếng Việt hiện ra bên phải với đầy đủ các mục:
kỳ sắp tới, điều kiện dự tuyển, mốc thời gian, liên hệ, link các nút, ảnh,
nhân sự, cảm nhận sinh viên, FAQ, chủ đề nghiên cứu, bố cục…

Sửa xong bấm **Tải file content.json** → máy tải về file mới → upload file đó
lên GitHub đè lên file cũ. Xong.

Nếu có thêm ảnh mới, bấm **Tải ảnh đã đổi tên** rồi upload các ảnh đó vào
thư mục `assets/`.

### Cách 2 — Sửa thẳng trên GitHub

Mở `content.json` trên github.com → bấm biểu tượng bút chì ✏️ → sửa → **Commit changes**.

Chỉ sửa phần nằm giữa hai dấu nháy kép `"..."`, đừng xoá dấu phẩy hay dấu ngoặc.

## Quy tắc quan trọng: chữ trong ngoặc vuông

Những chỗ chưa có nội dung thật được viết dạng `[Tên giáo sư]`, `[Research Topic]`…

- **Khách vào xem:** những chỗ đó **tự động ẩn đi**, kể cả cả mục hoặc cả thẻ nếu
  trống hoàn toàn. Nhờ vậy trang luôn trông hoàn chỉnh, không bao giờ lộ chữ tạm.
- **Khi mở `?edit`:** vẫn hiện nguyên để bạn biết chỗ nào cần điền.

Muốn nội dung nào xuất hiện, chỉ cần thay chữ trong ngoặc vuông bằng nội dung thật.

## Về hình ảnh

- Ảnh đặt trong thư mục `assets/`
- Trong `content.json` phải ghi kèm thư mục, ví dụ: `"assets/campus-view.jpg"`
- Đặt tên file **không dấu, không khoảng trắng**, dùng gạch ngang: `machine-1.jpg`
- Nên nén ảnh dưới 500 KB trước khi dùng, nếu không trang sẽ tải chậm
- Khung ảnh nào chưa có ảnh sẽ **tự ẩn**, không để lại ô xám trống
