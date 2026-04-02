---
{"dg-publish":true,"permalink":"/01-projects/dss-corp/dss-to-trinh-trien-khai/"}
---


# TỜ TRÌNH ĐỀ XUẤT KẾ HOẠCH CHUYỂN ĐỔI SỐ DSS

> ⬅️ [[01. Projects/DSS-Corp/Trang Chủ\|Quay lại Trang chủ Dự án DSS-Corp]]

**Kính gửi:** Ban Giám Đốc – Sếp Tiền  
**Người đề xuất:** Tuyết Chinh  
**Ngày báo cáo:** ___/___/2026  
**Mục tiêu:** Thống nhất vận hành — Giảm tải thủ công — Minh bạch dữ liệu hệ thống trên toàn bộ công ty DSS.

---

## I. HIỆN TRẠNG THỰC TẾ DƯỚI GÓC ĐỘ QUẢN TRỊ

Hiện tại, công ty quy mô 60 nhân sự với 6 phòng ban đang gặp rào cản về kết nối dữ liệu và hiệu suất làm việc do sử dụng công cụ phân tán:

| Vấn đề hiện tại | Hệ quả rủi ro & Bất cập |
|-----------------|--------------------------|
| 📱 **Giao tiếp chính qua Zalo cá nhân** | Thông tin công việc dễ bị trôi. Quan trọng nhất: Nhân viên nghỉ việc sẽ mang theo toàn bộ data, lịch sử trao đổi, thông tin đối tác của công ty. |
| 📊 **Quản lý bằng Excel/Google Sheet rời rạc** | Mỗi phòng ban lưu trữ 1 kiểu. Dữ liệu phân mảnh, trùng lặp và cực kỳ khó đối chiếu, đồng bộ qua lại giữa Kinh doanh - Kế toán - Kho. |
| 🕐 **Chấm công qua Máy free → Xuất Excel** | Bộ phận HCNS đang tốn 3-5 ngày mỗi tháng chỉ để xuất file, kiểm tra và tính tay lương. Dễ xảy ra sai sót con người. |
| 📄 **Phê duyệt đơn từ qua Zalo/Giấy** | Phân tán, sếp khó tra cứu lại lịch sử ai đã duyệt. Mất thời gian chờ đợi khi người duyệt đi vắng. |
| 🔍 **Báo cáo tổng hợp** | Sếp cần số liệu gấp, nhân sự phải lật đật liên hệ các phòng ban gom số liệu từ chục file khác nhau. Không có báo cáo Real-time. |

> 💡 **Nhận định:** Công cụ rời rạc → Dữ liệu đứt gãy → Chậm ra quyết định và lãng phí nguồn lực nhân sự vào việc "chạy cơm".

---

## II. GIẢI PHÁP ĐỀ XUẤT: LARK SUITE

Thay vì mua sắm, tích hợp nhiều phần mềm lẻ tẻ, Chinh đề xuất dịch chuyển toàn bộ vận hành nội bộ lên 1 nền tảng duy nhất là **Lark Suite**.

### 1. Mô hình dự kiến
- 💬 **Lark Messenger:** Thay thế Zalo, tạo kênh trao đổi công việc bảo mật.
- 📋 **Lark Base:** Thay thế Excel, làm cơ sở dữ liệu số cho các phòng ban.
- ✅ **Lark Approval:** Số hóa toàn bộ giấy tờ, đơn từ trình ký.
- 🕐 **Lark Attendance:** Tracking chấm công trực tiếp, làm mới quy trình ca kíp - chuyển đổi hoặc vẫn tận dụng ZKBio Zlink trước đã.
- 📊 **Dashboard:** Gom dữ liệu tổng quan, phục vụ cho Ban Giám đốc quản trị.

### 2. Ưu điểm thiết thực mang lại cho DSS
- **Bảo mật tuyệt đối:** Lịch sử chat, tài liệu, file đều là tài sản của công ty. Cắt quyền 1 account là ngắt toàn bộ truy cập khi nhân sự chuyển công tác.
- **Tiện lợi 1 App:** Nhân viên đi thị trường, thợ kỹ thuật ở công trình chỉ cần cài 1 ứng dụng trên điện thoại để chấm công, giao việc, báo cáo.
- **Tối ưu chi phí:** Có thể bắt đầu xây dựng bằng bản Miễn phí (Standard ≤ 50 user), chạy thử nghiệm ổn định. Sau này áp dụng bản Pro ($12/user) kết hợp với bản A2 Frontline cho nhóm thợ/kỹ thuật để tối ưu nhất chi phí mua bản quyền.

---

## III. HÌNH DUNG ÁP DỤNG THỰC TẾ

| Phòng ban | Cách làm hiện tại | Sau khi số hóa trên Lark | Tiết kiệm / Cải thiện |
|-----------|--------------------|---------------------------|----------------------|
| **HCNS** | Máy chấm công → Excel → Khớp tay | App chấm công di động/Wifi + Base lương chạy công thức tự động | Tiết kiệm **~3 ngày** chốt công/lương mỗi tháng |
| **HCNS** | Xin nghỉ phép, công tác qua Zalo | Flow phê duyệt tự động duyệt tuần tự | 1 chạm, tự động cập nhật và trừ phép năm |
| **Dự án** | Quản lý tiến độ trên nhiều file/nhóm | 1 Base theo dõi Dự án chung + hiển thị bảng Gantt | Sếp nắm ngay dự án nào đang có nguy cơ chậm trễ |
| **Kinh doanh** | Word/Sheet làm báo giá riêng lẻ | Database danh sách Khách hàng + Deal | Nắm bắt tỷ lệ chuyển đổi, lịch sử tư vấn liền mạch |
| **Kế toán** | Đối soát qua file xuất từ PM Kế toán | Dùng Misa làm phần mềm Lõi Tài chính, giữ Base là nơi đối soát số liệu vận hành | Rút ngắn thời gian khớp số liệu giữa Kế toán - Kinh doanh - Dự án |

---

## IV. LỘ TRÌNH THỰC HIỆN (DỰ KIẾN 12 THÁNG)

Chinh đề xuất áp dụng phương pháp **Chuyển đổi cuốn chiếu** — làm đến đâu, chắc đến đó, tuyệt đối không áp đặt đồng loạt gây ngợp cho nhân sự.

1. **Giai đoạn 1: Nền tảng (Tháng 1-3)**
   - Đưa sơ đồ tổ chức lên Lark, chuẩn hóa nhóm Chat (Messenger).
   - Số hóa phòng HCNS: Đẩy flow Chấm công, Phê duyệt, Quản lý Hồ sơ nhân sự lên hệ thống.
   - Nhằm giúp toàn thể nhân sự tạo thói quen dùng App mỗi ngày.

2. **Giai đoạn 2: Nghiệp vụ Core (Tháng 4-6)**
   - Số hóa luồng theo dõi Tiến độ Dự án.
   - Số hóa Khách hàng & Pipeline (Phòng Kinh doanh).

3. **Giai đoạn 3 & 4: Tự động hóa & Tối ưu (Tháng 7-12)**
   - Setup các bot trích xuất báo cáo, báo nhắc nhở deadline tự động.
   - Hoàn thiện Dashboard tổng hợp các luồng dữ liệu liên phòng ban về cho Ban Giám đốc.

---

## V. CÁCH THỨC THỰC HIỆN & SỰ HỖ TRỢ CẦN THIẾT

1. 🥇 **Triển khai phòng HCNS đầu tiên:** Chinh sẽ ngồi phỏng vấn bộ phận nhân sự khoảng 60 phút để map lại toàn bộ luồng quy chế tính công, tính lương hiện tại.
2. 🥈 **Tạo bản Demo & Dùng thử:** Chinh tự dựng cấu trúc trên phần mềm, mời đại diện phòng ban dùng thử (chưa áp dụng chính thức vội).
3. 🥉 **Áp dụng chính thức & Chuyển sang phòng tiếp theo:** Khi HCNS ổn, chuyển qua phòng Dự án, Kinh doanh...

**Đề xuất sự hỗ trợ từ Ban Giám đốc:**
- Sếp Tiền thông báo chủ trương xuống các Trưởng phòng để thông suốt tinh thần hợp tác.
- Yêu cầu các bộ phận cung cấp biểu mẫu/file Excel đang thao tác thực tế (không cần số liệu mật) để Chinh cấu trúc lại thành dữ liệu số.

---

## VI. MỤC TIÊU & KỲ VỌNG NỘI BỘ

- **Không gây shock vận hành:** Việc kinh doanh của công ty vẫn diễn ra bình thường trong thời gian chuyển đổi. Phần mềm mới sinh ra nhằm loại bỏ việc nhập liệu lại 2 lần, chứ không ép nhân sự ôm thêm việc.
- **Loại bỏ công việc "Chạy cơm":** Xóa sổ tình trạng xin chữ ký trình giấy, hoặc tự copy/paste số liệu qua lại từ 5 file Excel khác nhau (nhắm tới trong 6 tháng đầu).
- **Quản trị trung tâm Real-time:** Kết thúc lộ trình, Sếp Tiền chỉ cần sử dụng điện thoại, mở 1 màn hình để thấy ngay: Tình hình nhân sự tại vị trí, Chi phí/Doanh thu sơ bộ, Tiến độ các Dự án cốt lõi có xanh chín không.

---

## VII. KẾ HOẠCH TUẦN TỚI (NEXT STEPS)

| # | Hành động | Trách nhiệm | Thời gian dự kiến |
|---|-----------|-------------|-------------------|
| 1 | Sếp phê duyệt chủ trương triển khai nội bộ | Sếp Tiền | Tuần này |
| 2 | Sếp thông báo định hướng cho các cấp quản lý | Sếp Tiền | Tuần này |
| 3 | Phân tích thực trạng: Phỏng vấn nghiệp vụ P. HCNS | Chinh + P. HCNS | Tuần sau |
| 4 | Xây dựng khung quản lý Nhân sự & Chấm công bản nháp | Chinh | Tuần 2-3 |
| 5 | Báo cáo tiến độ hoàn thành Phase 1 cho GĐ | Chinh | Cuối tháng 5 |

---

*(Hết tờ trình)*
