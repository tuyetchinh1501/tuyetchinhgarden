---
{"dg-publish":true,"permalink":"/05-daily-and-tasks/bai-viet-obsidian-tram-trung-chuyen-thong-tin-mien-phi-real-time/","title":"Biến Obsidian thành trạm trung chuyển thông tin — miễn phí và real-time","tags":["SecondBrain","Obsidian","AIproductivity","Teamwork","Workflow"]}
---


# Biến Obsidian thành trạm trung chuyển thông tin — miễn phí và real-time

> **Series: Giá trị của Second Brain trong thời đại AI**
> Ngày: 11/03/2026
> Case thực tế từ dự án Antigravity — Test hệ thống & cộng tác team

[[05. Daily & Tasks/Blog nhỏ của Tuyết Chinh\|Blog nhỏ của Tuyết Chinh]]
---

## Giá trị mình thu được

Hiện tại mình làm việc với Antigravity mỗi ngày mỗi giờ, trong giai đoạn quan trọng: lên kế hoạch tổng thể cho các kịch bản test app, tổng hợp kết quả test, theo dõi tiến độ, ghi nhận quy trình, và log bug cùng quá trình sửa lỗi hệ thống của Công ty

Đây là giai đoạn mà khối lượng tài liệu sinh ra rất lớn — mỗi kịch bản test là một file, mỗi lần chạy test lại cần ghi nhận kết quả, mỗi bug cần log chi tiết để team có thể đọc hiểu và xử lý.

Câu hỏi đặt ra: **Làm sao để vừa làm việc hiệu quả với AI, vừa chia sẻ nhanh cho team mà không tốn thao tác thừa?**

Và giá trị mình thu được sau việc này là:
- Ship tài liệu hoả tốc cho team
- Giảm bớt việc tạo ra quá nhiều file rác và tiết kiệm thời gian convert file
- Tiết kiệm số lượng token AI phải xử lý đồng nghĩa với tiết kiệm xiền :D

---

## Vấn đề thực tế

Khi làm việc với Antigravity/Claude (hoặc bất kỳ AI nào), định dạng tối ưu nhất cho tài liệu là **Markdown**. Lý do đơn giản:

- AI đọc và xử lý markdown cực nhanh, không cần parse phức tạp.
- Mình chỉnh sửa, bổ sung nội dung trực tiếp trong quá trình trao đổi với AI mà không bị lệch format.
- Cấu trúc rõ ràng: heading, list, table, code block — đủ để mô tả kịch bản test, log bug, hay tổng hợp tiến độ.

Nhưng vấn đề nằm ở **khâu chia sẻ cho team**:

1. **File markdown thô** — team không quen đọc, nhìn thấy cú pháp `##`, `- [ ]`, `|---|` là rối mắt ngay.
2. **Convert sang doc/PDF rồi gửi** — mất thêm 2–3 thao tác mỗi lần, và quan trọng hơn là tạo ra nhiều phiên bản file khác nhau. Sửa file gốc xong lại phải convert lại, gửi lại. Team không biết đang đọc đúng bản mới nhất hay không.
3. **Copy nội dung vào Google Docs hay Lark Docs** — lại thêm một bước trung gian, format bị lệch, và giờ phải maintain song song 2 nơi.

Tóm lại: **quy trình bị đứt đoạn giữa "nơi tạo ra nội dung" và "nơi team đọc nội dung"**.

---

## Giải pháp: Obsidian làm trạm trung chuyển

Ý tưởng cốt lõi học từ người đi trước, rất đơn giản: **để Obsidian đứng giữa, nhận file markdown từ AI và hiển thị sẵn sàng để chia sẻ - không cần convert, không cần gửi file**.

### Bước 1: Kết nối AI → Obsidian (thực ra là... không cần kết nối gì cả)

Mấu chốt nằm ở chỗ này: **thư mục vault của Obsidian chính là thư mục Chinh đang làm việc với Antigravity/Claude**. Cùng một đường dẫn, cùng một nơi.

Ví dụ thực tế: thư mục dự án của Chinh là `D:\OneDrive\Chinh Homepage\02. Products - Project\3. Service\16. DSS_247`. Chinh vừa trỏ Claude/Antigravity vào thư mục này để lưu output, vừa mở thư mục này làm vault trong Obsidian. Vậy là xong — không có bước trung gian nào.

Khi Claude tạo ra file markdown (kế hoạch test, log kết quả, danh sách bug...), file đó được lưu thẳng vào thư mục dự án. Mà thư mục dự án cũng chính là vault Obsidian. Nên **file vừa tạo xong là tự động xuất hiện trong Obsidian** dưới dạng note — đã được render đẹp, có heading, có bảng, có checklist — mà Chinh không cần mở file, không cần copy-paste, không cần di chuyển file đi đâu cả.

Không có bước "sync", không có bước "import". Obsidian đọc native markdown — file nào nằm trong vault là hiển thị ngay, đúng format.

### Bước 2: Publish trực tiếp lên online

Chinh đã cài plugin cho phép publish note lên web (dùng vercel). Quy trình chỉ còn:

1. File markdown được tạo xong → tự hiện trong Obsidian.
2. Chinh mở note, kiểm tra nhanh → chọn **Publish**.
3. Lấy link → gửi cho team.

Thế là xong. Team mở link, đọc trực tiếp trên trình duyệt. Nội dung hiển thị dạng text bình thường, có format đẹp, không cần cài gì thêm.

**Và quan trọng nhất**: khi Chinh cập nhật file gốc (sửa bug status, thêm kết quả test mới, điều chỉnh kế hoạch), team chỉ cần refresh link là thấy nội dung mới nhất — **real-time, đúng bản gốc, không nhầm phiên bản**.

---

## So sánh: Trước và sau

| | Trước | Sau (với Obsidian) |
|---|---|---|
| **Tạo tài liệu** | Làm với AI → file markdown | Làm với AI → file markdown |
| **Chia sẻ team** | Convert doc/PDF → gửi file → team download | Publish link → gửi link → team mở trình duyệt |
| **Cập nhật nội dung** | Sửa file gốc → convert lại → gửi lại → team xác nhận đúng bản | Sửa file gốc → team refresh link |
| **Số thao tác thừa** | 3–5 bước mỗi lần cập nhật | 1 bước (publish lại sau khi cập nhật nội dung) |
| **Rủi ro nhầm phiên bản** | Cao — nhiều file trôi nổi | Không — luôn là bản gốc duy nhất |
| **Chi phí** | Phụ thuộc tool convert | Miễn phí |

---

## Bây giờ mình hiểu thêm một giá trị nữa của Second Brain

Trước đây chỉ hiểu Second Brain chỉ là "nơi lưu ghi chú cá nhân". Nhưng case hôm nay cho thấy một góc khác: **Second Brain có thể là điểm nối giữa quy trình làm việc cá nhân và cộng tác team**.

Cụ thể với Obsidian:

- Nó là **nơi nhận đầu ra từ AI** — vì bản chất là thư mục chứa file markdown, không cần import hay sync phức tạp.
- Nó là **nơi hiển thị nội dung dễ đọc ngay lập tức** — vì render markdown native, không cần convert.
- Nó là **nơi phân phối thông tin ra ngoài** — vì có plugin publish, biến note thành trang web chỉ bằng 1 click.

Ba vai trò đó gộp lại, Obsidian trở thành **trạm trung chuyển thông tin**: nhận từ AI, xử lý tại chỗ, phát ra cho team - nhanh, gọn, miễn phí, và luôn đúng bản gốc.

---

## Mấy thứ mình rút ra

- Plugin publish có nhiều lựa chọn miễn phí (Digital Garden, Quartz, hoặc các giải pháp tự host). Không nhất thiết phải dùng Obsidian Publish trả phí.
- Nếu team cần brainstorm hay comment, có thể kết hợp thêm bước gửi link vào nhóm chat (Lark, Zalo, Slack...) để thảo luận. Obsidian đóng vai trò "nguồn sự thật duy nhất" cho nội dung, còn thảo luận diễn ra ở kênh chat =>dùng bot tóm ý và bắn lại vào Antigravity
- Cách này đặc biệt phù hợp với người làm back office như mình khi tài liệu thay đổi liên tục trong ngày và team cần đọc bản mới nhất ngay lập tức.

---

*Tags: #SecondBrain #Obsidian #AIproductivity #Teamwork #Workflow*

*Chinh Productivity — tuyetchinh.com*
