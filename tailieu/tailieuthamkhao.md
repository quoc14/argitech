# AGRITECH AIoT

> **Vấn đề thật → Nhu cầu thật → Giải pháp phù hợp → Sản phẩm hoạt động thế nào → Sử dụng ra sao → Công nghệ cốt lõi → Kiểm thử thực tế → Người dùng đánh giá → Giới hạn → Hướng hoàn thiện**

## Giải pháp hỗ trợ nông dân trong canh tác

| Thông tin               | Nội dung                     |
| ----------------------- | ---------------------------- |
| **Đội thi**             | GREEN HORIZON                |
| **Trường**              | THPT Trường Xuân – Đồng Tháp |
| **Giáo viên hướng dẫn** | Nguyễn Đức Vĩnh              |

### Gợi ý trang bìa

Không để quá nhiều chữ.

Nên có:

- Logo Samsung Solve for Tomorrow.
- Tên sản phẩm.
- Tên đội.
- Trường.
- **Một ảnh lớn của sản phẩm thật ngoài đồng ruộng.**

Không nên tiếp tục dùng hình minh họa như ở bản vòng sơ khảo.

---

# Mục lục

- **Chương 1. Vấn đề thực tế và nhu cầu người dùng**
  - 1.1. Bối cảnh và vấn đề
  - 1.2. Người dùng hướng tới
  - 1.3. Từ nhu cầu thực tế đến yêu cầu của sản phẩm
- **Chương 2. Giải pháp AgriTech AIoT**
  - 2.1. Tổng quan sản phẩm
  - 2.2. Các chức năng chính của sản phẩm
  - 2.3. Những điểm nổi bật trong thiết kế
- **Chương 3. Cấu tạo và nguyên lý hoạt động**
  - 3.1. Cấu tạo sản phẩm
  - 3.2. Kiến trúc hoạt động tổng thể
  - 3.3. Luồng xử lý hình ảnh
  - 3.4. Luồng xử lý cảm biến
  - 3.5. Hoạt động khi kết nối bị gián đoạn
  - 3.6. Chu kỳ hoạt động của hệ thống
- **Chương 4. Hướng dẫn sử dụng sản phẩm**
  - 4.1. Lắp đặt
  - 4.2. Khởi động sản phẩm
  - 4.3. Chế độ tự động
  - 4.4. Chế độ người dùng chủ động
  - 4.5. Hướng dẫn sử dụng Web
  - 4.6. Xử lý một số tình huống thường gặp
  - 4.7. Tắt và thu hồi sản phẩm
- **Chương 5. Công nghệ và quá trình xây dựng**
  - 5.1. Bộ dữ liệu
  - 5.2. 10 trạng thái phân loại
  - 5.3. Huấn luyện mô hình
  - 5.4. Kết quả huấn luyện
  - 5.5. GradCAM
  - 5.6. Lưu trữ và đồng bộ dữ liệu
  - 5.7. Trợ lý AI
- **Chương 6. Kiểm thử và kết quả thực nghiệm**
  - 6.1. Phương pháp kiểm thử
  - 6.2. Kiểm thử trong điều kiện thử nghiệm
  - 6.3. Kết quả trí tuệ nhân tạo
  - 6.4. Kiểm thử ngoài đồng ruộng
  - 6.5. Các trường hợp chưa thành công
  - 6.6. Điều nhóm rút ra từ kiểm thử
- **Chương 7. Phản hồi người dùng, giới hạn và cải tiến**
  - 7.1. Phản hồi thực tế
  - 7.2. Từ phản hồi đến cải tiến
  - 7.3. Giới hạn hiện tại
  - 7.4. Những gì đã chứng minh và chưa chứng minh đầy đủ
- **Chương 8. Khả năng triển khai và hướng phát triển**
  - 8.1. Chi phí các linh kiện chính
  - 8.2. Khả năng tiếp tục triển khai
  - 8.3. Hướng phát triển
  - 8.4. Phân công thành viên
  - 8.5. Tác động hiện tại và tác động kỳ vọng
- **Tài liệu tham khảo**
- **Phụ lục kỹ thuật**

---

# CHƯƠNG 1. VẤN ĐỀ THỰC TẾ VÀ NHU CẦU NGƯỜI DÙNG

## 1.1. Bối cảnh và vấn đề

Lúa là một trong những cây trồng quan trọng tại Việt Nam nói chung và Đồng Tháp nói riêng. Trong quá trình canh tác, người nông dân phải thường xuyên theo dõi tình trạng sinh trưởng của cây, phát hiện các biểu hiện sâu bệnh và kiểm tra những yếu tố liên quan đến môi trường đất.

Việc kiểm tra hiện nay phần lớn vẫn dựa vào quan sát trực tiếp và kinh nghiệm của người trồng lúa. Đây là nguồn kinh nghiệm có giá trị, nhưng trên những diện tích canh tác rộng, việc kiểm tra thường xuyên từng khu vực mất nhiều thời gian và công sức. Trong một số trường hợp, những biểu hiện bất thường trên cây chỉ được phát hiện khi đã trở nên rõ ràng hơn.

Bên cạnh tình trạng cây, các yếu tố như độ ẩm, nhiệt độ và dinh dưỡng đất cũng ảnh hưởng đến quá trình sinh trưởng. Tuy nhiên, những chỉ số này khó được đánh giá chính xác chỉ bằng quan sát thông thường.

Vì vậy, nhóm đặt ra câu hỏi:

> **Có thể xây dựng một hệ thống hỗ trợ người nông dân theo dõi đồng thời hình ảnh cây lúa và một số chỉ số môi trường đất, đồng thời cung cấp thông tin từ xa khi xuất hiện dấu hiệu bất thường hay không?**

Đây là vấn đề mà AgriTech AIoT hướng tới giải quyết.

> **CẦN CHÈN NGAY TẠI ĐÂY**

**Hình 1:** Ảnh ruộng lúa thực tế tại địa phương.

Tốt nhất dùng ảnh nhóm đã xuống ruộng, không dùng ảnh mạng.

**Hình 2:** Người nông dân đang kiểm tra lúa theo phương pháp thông thường.

Nếu nhóm có ảnh thật thì rất tốt.

> **CẦN BỔ SUNG 1–2 SỐ LIỆU CÓ NGUỒN**

Không nên tiếp tục viết chung chung:

> “Bệnh lúa gây thiệt hại 20–50%”

nếu chưa có nguồn rõ.

Nên có dạng:

> Theo [nguồn], bệnh X có thể gây ảnh hưởng… trong những điều kiện…

và trích nguồn ngay sau câu.

Chỉ cần **1–2 số liệu thật mạnh**, không cần 10 con số.

> **BỔ SUNG — BẰNG CHỨNG CHO VIỆC XÁC ĐỊNH VẤN ĐỀ**

Phần này nên có một box nhỏ để BGK hiểu nhóm không chỉ “nghĩ ra” vấn đề mà đã có quá trình tìm hiểu.

**Nhóm xác định vấn đề dựa trên:**

- quan sát trực tiếp tại khu vực trồng lúa;
- trao đổi với người nông dân;
- ý kiến của người có kinh nghiệm hoặc chuyên môn trong lĩnh vực nông nghiệp;
- các tài liệu chuyên môn và số liệu có nguồn rõ ràng.

Nếu nhóm có ảnh, biên bản hoặc ghi chú từ các buổi trao đổi thì có thể đưa một phần vào phụ lục.

---

## 1.2. Người dùng hướng tới

AgriTech AIoT hướng tới **người trực tiếp trồng và quản lý ruộng lúa**, đặc biệt là những người có nhu cầu:

- theo dõi tình trạng cây lúa thường xuyên;
- có thêm thông tin hỗ trợ nhận biết biểu hiện bất thường;
- theo dõi một số chỉ số môi trường đất tại vị trí quan trắc;
- xem dữ liệu khi không có mặt trực tiếp tại ruộng;
- nhận thông báo khi hệ thống phát hiện điều kiện cần chú ý.

Trong quá trình thử nghiệm, nhóm đã đưa sản phẩm đến khu vực trồng lúa tại xã Phương Thịnh, Đồng Tháp để người dân và người có kinh nghiệm trong lĩnh vực nông nghiệp trực tiếp quan sát, trải nghiệm và đóng góp ý kiến.

> **CẦN CHÈN**

**Hình 3:** Nhóm làm việc với chú Nguyễn Thanh Khương.

Chú có hơn 25 năm kinh nghiệm trồng lúa ....

Có thể thiết kế thành một thẻ:

> **Người dùng trải nghiệm**
> Nguyễn Thanh Khương
> Hơn 25 năm làm nghề trồng lúa
> Xã Phương Thịnh – Đồng Tháp

Bên cạnh là ảnh.

> **NẾU CÓ THỂ BỔ SUNG**

Một box:

### Một số nhu cầu nhóm ghi nhận

Ví dụ:

> “Ruộng rộng nên không thể lúc nào cũng đi kiểm tra hết.”

> “Nếu có cảnh báo từ xa thì sẽ thuận tiện hơn.”

Nếu nhóm tổng hợp lại ý thì ghi:

> **Tóm tắt ý kiến người dùng (hoặc hỏi từng người hay khảo sát là tốt nhất)**

> **BỔ SUNG — NẾU CÒN THỜI GIAN NÊN LÀM THÊM KHẢO SÁT NHỎ**

Không cần khảo sát hàng trăm người. Có thể hỏi khoảng một số người trồng lúa tại địa phương với cùng một nhóm câu hỏi ngắn:

1. Bình thường cô/chú kiểm tra tình trạng lúa như thế nào?
2. Khó khăn nhất khi theo dõi ruộng là gì?
3. Cô/chú có thường sử dụng thiết bị để kiểm tra đất không?
4. Việc nhận cảnh báo khi không có mặt tại ruộng có hữu ích không?
5. Nếu sử dụng một thiết bị như AgriTech AIoT, điều gì quan trọng nhất: dễ sử dụng, chính xác, bền, giá thành hay yếu tố khác?

Nếu làm khảo sát, nên tổng hợp thành biểu đồ nhỏ và **không suy rộng kết quả cho toàn bộ nông dân**.

---

## 1.3. Từ nhu cầu thực tế đến yêu cầu của sản phẩm

| Nhu cầu/điều kiện thực tế                | Yêu cầu với sản phẩm                       | Cách AgriTech AIoT đáp ứng           |
| ---------------------------------------- | ------------------------------------------ | ------------------------------------ |
| Cần theo dõi tình trạng cây              | Có khả năng thu nhận và phân tích hình ảnh | Camera + mô hình AI                  |
| Khó đánh giá đất bằng cảm quan           | Có dữ liệu định lượng tại điểm đo          | NPK + nhiệt độ + độ ẩm               |
| Không thể luôn có mặt tại ruộng          | Theo dõi được từ xa                        | Giao diện Web                        |
| Cần biết khi có bất thường               | Có cơ chế thông báo                        | Cảnh báo + SMS                       |
| Kết nối ngoài ruộng có thể không ổn định | Chức năng cốt lõi giảm phụ thuộc máy chủ   | Xử lý tại Raspberry Pi + lưu cục bộ  |
| Người dùng không chuyên công nghệ        | Thao tác đơn giản                          | Chế độ tự động + giao diện trực quan |

> **Các thành phần công nghệ của AgriTech AIoT được lựa chọn từ nhu cầu sử dụng thực tế .....**

> **BỔ SUNG — CÓ THỂ HOÀN THIỆN CÂU KẾT**

> **Các thành phần công nghệ của AgriTech AIoT được lựa chọn từ nhu cầu sử dụng thực tế, trong đó mỗi thành phần đảm nhiệm một vai trò cụ thể trong việc thu thập dữ liệu, xử lý, theo dõi hoặc cảnh báo cho người dùng.**

Điểm quan trọng là làm rõ:

> **Không phải nhóm sử dụng nhiều công nghệ để sản phẩm “nhiều tính năng”, mà mỗi công nghệ phải trả lời được một nhu cầu cụ thể.**

---

# CHƯƠNG 2. GIẢI PHÁP AGRITECH AIoT

## 2.1. Tổng quan sản phẩm

AgriTech AIoT là hệ thống hỗ trợ theo dõi tình trạng cây lúa và một số chỉ số môi trường đất thông qua sự kết hợp giữa camera, cảm biến, trí tuệ nhân tạo và kết nối mạng di động.

Raspberry Pi 4 đóng vai trò xử lý trung tâm. Camera cung cấp hình ảnh cây lúa cho mô hình trí tuệ nhân tạo phân loại trạng thái. Song song đó, các cảm biến thu thập dữ liệu NPK, nhiệt độ và độ ẩm tại vị trí đặt đầu dò.

Kết quả được:

- xử lý tại thiết bị;
- hiển thị tại trạm;
- lưu trữ;
- đồng bộ lên hệ thống Web;
- và có thể kích hoạt cảnh báo tới người sử dụng khi thỏa mãn điều kiện được thiết lập.

> **CẦN CHÈN**

**Hình 4.** Ảnh toàn cảnh sản phẩm thật.

Ảnh cần rõ, dễ nhìn. Đánh số trực tiếp các thành phần:

1. Camera.
2. Raspberry Pi.
3. Cảm biến.
4. SIM7600.
5. LCD.
6. Nguồn.

Để BGK nhìn ảnh phải hiểu ngay.

---

### 2.1.1. Mức độ hoàn thiện các chức năng hiện tại

Nên có bảng này ngay sau phần tổng quan để BGK phân biệt rõ **cái gì sản phẩm đã thực hiện được, cái gì còn cần kiểm thử thêm**.

| Chức năng                         | Mức độ hiện tại        |
| --------------------------------- | ---------------------- |
| Thu nhận hình ảnh                 | Đã thực hiện           |
| Phân loại 10 trạng thái           | Đã thực hiện           |
| Thu dữ liệu NPK                   | Đã thực hiện           |
| Nhiệt độ, độ ẩm đất               | Đã thực hiện           |
| Hiển thị tại trạm                 | Đã thực hiện           |
| Theo dõi trên Web                 | Đã thực hiện           |
| Cảnh báo qua SMS                  | Đã thực hiện           |
| Lưu dữ liệu cục bộ                | Đã tích hợp            |
| Đồng bộ sau khi mất mạng          | Đã thiết kế/triển khai |
| GradCAM                           | Đã tích hợp            |
| Trợ lý AI                         | Đã tích hợp            |
| Nguồn năng lượng mặt trời dài hạn | Cần kiểm thử thêm      |
| Hoạt động lâu dài ngoài ruộng     | Cần kiểm thử thêm      |

## 2.2. Các chức năng chính của sản phẩm

Nên thiết kế thành **infographic 5 chức năng**, thay vì 1 trang chữ dài.

### 2.2.1. Phân loại trạng thái cây lúa bằng trí tuệ nhân tạo

Camera thu nhận hình ảnh cây lúa theo chế độ tự động hoặc khi người dùng chủ động yêu cầu.

Hình ảnh được chuyển tới Raspberry Pi và xử lý bằng mô hình YOLO11s-cls.

Mô hình được xây dựng để phân loại **10 trạng thái của cây lúa**, gồm 9 nhóm bệnh hoặc biểu hiện sâu hại và 1 trạng thái bình thường.

Kết quả chính gồm:

- trạng thái được dự đoán;
- độ tin cậy;
- hình ảnh tương ứng.

> **CẦN CHÈN**

Một ví dụ thật:

**Ảnh đầu vào → kết quả phân loại → Confidence**

Nhớ YOLO là không phải detect nên không được nói là bounding box.

---

### 2.2.2. Theo dõi dữ liệu môi trường đất

Sản phẩm sử dụng các cảm biến để ghi nhận:

- hàm lượng N;
- P;
- K;
- nhiệt độ;
- độ ẩm đất.

Các dữ liệu này được đọc tại vị trí đặt đầu dò và gửi về Raspberry Pi để xử lý, lưu trữ và hiển thị.

Cần ghi rõ:

> **Các thông số phản ánh điều kiện tại vị trí đặt cảm biến, không đại diện mặc nhiên cho toàn bộ thửa ruộng.**

Điểm này rất nên chủ động nói.

> **CẦN CHÈN**

Ảnh thật đầu cảm biến đang cắm ngoài ruộng.

---

### 2.2.3. Cảnh báo khi phát hiện bất thường

Khi kết quả phân loại hoặc dữ liệu cảm biến đáp ứng điều kiện cảnh báo đã thiết lập (điều kiện thiết lập là gì cần làm rõ ... ), hệ thống có thể kích hoạt cảnh báo và gửi tin nhắn tới người dùng thông qua module SIM7600.

> **CẦN CHÈN**

**Screenshot SMS thật mà sản phẩm đã gửi.**

Đây là bằng chứng mạnh hơn rất nhiều so với mô tả 1 đoạn dài.

> **BỔ SUNG — PHẢI LÀM RÕ LOGIC CẢNH BÁO**

Nên có bảng:

| Loại cảnh báo     | Điều kiện kích hoạt thực tế               | Hành động của hệ thống           |
| ----------------- | ----------------------------------------- | -------------------------------- |
| Cảnh báo AI       | Confidence ≥ ... và lớp dự đoán thuộc ... | Lưu ảnh + SMS/Web                |
| Cảnh báo NPK      | Giá trị ... vượt/ngắn hơn ngưỡng ...      | LCD/Web/SMS                      |
| Cảnh báo độ ẩm    | Giá trị ...                               | ...                              |
| Cảnh báo nhiệt độ | Giá trị ...                               | ...                              |
| Thiết bị/mạng     | Mất kết nối trong ...                     | Lưu cục bộ / hiển thị trạng thái |

Phải lấy đúng ngưỡng đang được cấu hình trong mã nguồn và làm rõ cơ sở lựa chọn ngưỡng.

---

### 2.2.4. Theo dõi từ xa

Giao diện Web cho phép người sử dụng xem:

- trạng thái hệ thống;
- hình ảnh cây;
- kết quả phân loại;
- dữ liệu NPK;
- nhiệt độ;
- độ ẩm;
- lịch sử;
- cảnh báo.

> **CẦN CHÈN**

Screenshot Web thật các màn.

---

### 2.2.5. Trợ lý ảo hỗ trợ người dùng

AgriTech AIoT tích hợp trợ lý ảo để người dùng có thể trao đổi bằng ngôn ngữ tự nhiên.

Kết quả phân loại và dữ liệu cảm biến có thể được cung cấp cho trợ lý làm ngữ cảnh nhằm hỗ trợ giải thích thông tin dễ hiểu hơn.

Ở giai đoạn hiện tại, trợ lý ảo được xác định là **công cụ hỗ trợ thông tin**, không thay thế chuyên gia nông nghiệp.

Đối với những nội dung liên quan đến:

- thuốc bảo vệ thực vật;
- liều lượng;
- phương pháp xử lý chuyên môn,

thông tin cần được đối chiếu với tài liệu nông nghiệp đáng tin cậy trước khi áp dụng.

> **CẦN CHÈN**

Một screenshot hội thoại tốt nhất.

Không cần đưa System Prompt vào.

---

## 2.3. Những điểm nổi bật trong thiết kế

Nên dùng:

### 1. Xử lý trí tuệ nhân tạo tại thiết bị

Mô hình được triển khai trên Raspberry Pi, giúp quá trình phân loại hình ảnh không bắt buộc phải truyền ảnh lên máy chủ để xử lý.

### 2. Lưu dữ liệu cục bộ

Khi kết nối tới máy chủ bị gián đoạn, dữ liệu có thể được lưu tại Raspberry Pi và đồng bộ lại sau khi kết nối được phục hồi.

### 3. Kết hợp nhiều nguồn thông tin

Sản phẩm kết hợp:

> **Hình ảnh cây + dữ liệu đất + cảnh báo + theo dõi từ xa.**

### 4. Nhiều cách theo dõi

Người sử dụng có thể nhận thông tin:

- tại trạm;
- qua Web;
- qua SMS.

> **BỔ SUNG — GỢI Ý TRÌNH BÀY**

Không để thành bốn đoạn chữ. Có thể trình bày thành bốn ô ngang hoặc bố cục 2 × 2 như sau:

| Điểm nổi bật                    | Thành phần                | Giá trị                                                |
| ------------------------------- | ------------------------- | ------------------------------------------------------ |
| **Xử lý tại thiết bị**          | AI chạy trên Raspberry Pi | Giảm phụ thuộc máy chủ đối với chức năng phân loại.    |
| **Lưu dữ liệu cục bộ**          | SQLite tại thiết bị       | Giữ dữ liệu tạm thời khi kết nối máy chủ bị gián đoạn. |
| **Kết hợp nhiều nguồn dữ liệu** | Camera + cảm biến         | Cung cấp thêm thông tin về cây và đất.                 |
| **Nhiều kênh theo dõi**         | LCD + Web + SMS           | Phù hợp với các tình huống sử dụng khác nhau.          |

Ở giữa có thể đặt ảnh sản phẩm thật.

---

# CHƯƠNG 3. CẤU TẠO VÀ NGUYÊN LÝ HOẠT ĐỘNG

## 3.1. Cấu tạo sản phẩm

Sản phẩm gồm các khối chính:

| Thành phần             | Vai trò                   |
| ---------------------- | ------------------------- |
| Raspberry Pi 4 Model B | Xử lý trung tâm           |
| Camera Hikvision       | Thu nhận hình ảnh         |
| Cảm biến NPK           | Thu thập N, P, K          |
| DS18B20                | Đo nhiệt độ               |
| FC-28 + ADS1115        | Đo độ ẩm đất              |
| SIM7600                | Mạng di động và SMS       |
| LCD                    | Hiển thị tại thiết bị     |
| Bộ nguồn               | Cấp năng lượng            |
| Hộp và kết cấu         | Bảo vệ, cố định linh kiện |

> **CẦN CHÈN**

Ảnh bên trong hộp thiết bị.

Ảnh ngoài hộp.

Ảnh sensor.

Có thể dành **1 trang visual**.

---

## 3.2. Kiến trúc hoạt động tổng thể

Phần chính chỉ nên có **1 sơ đồ duy nhất**.

> **SƠ ĐỒ ĐỀ XUẤT**

```text
Camera + cảm biến đất
          ↓
     Raspberry Pi
  ├─ Xử lý hình ảnh
  ├─ Chạy mô hình AI
  ├─ Đọc cảm biến
  ├─ Kiểm tra điều kiện
  └─ Lưu dữ liệu
          ↓
LCD / lưu cục bộ / cảnh báo
          ↓
SIM7600 / mạng di động
          ↓
       Máy chủ
          ↓
    Web / người dùng
```

---

> **CẦN LÀM LẠI SƠ ĐỒ**

Các flowchart hiện tại quá sâu và chữ quá nhỏ.

---

## 3.3. Luồng xử lý hình ảnh

Luồng được mô tả như sau:

```text
Camera
  ↓
Thu nhận ảnh
  ↓
Tiền xử lý
  ↓
YOLO11s-cls
  ↓
Lớp dự đoán + độ tin cậy
  ↓
GradCAM (khi cần giải thích)
  ↓
Lưu kết quả
  ↓
Kiểm tra điều kiện cảnh báo
```

> **CẦN SỬA TOÀN TÀI LIỆU**

Không còn:

> “tọa độ bệnh”

> “bounding box”

> “YOLO khoanh vùng bệnh”

---

## 3.4. Luồng xử lý cảm biến

```text
NPK + nhiệt độ + độ ẩm
            ↓
       Raspberry Pi
            ↓
       Đọc và xử lý
            ↓
        Lưu cục bộ
            ↓
       Hiển thị LCD
            ↓
      Đồng bộ lên Web
            ↓
Kiểm tra điều kiện cảnh báo
```

Không ghi tất cả sensor đều RS485.

Cần ghi đúng:

- NPK → kiểm tra RS485/Modbus.
- DS18B20 → 1-Wire.
- FC-28 → Analog.
- ADS1115 → I2C.

---

## 3.5. Hoạt động khi kết nối bị gián đoạn

| Chức năng            | Có kết nối | Mất kết nối máy chủ    |
| -------------------- | ---------: | ---------------------: |
| Đọc cảm biến         | Có         | Có                     |
| AI trên Raspberry Pi | Có         | Có                     |
| Hiển thị LCD         | Có         | Có                     |
| Lưu cục bộ           | Có         | Có                     |
| Đồng bộ Web          | Có         | Tạm dừng               |
| Web từ xa            | Có         | Không cập nhật mới     |
| Trợ lý ảo            | Có         | Không                  |
| SMS                  | Có         | Phụ thuộc mạng di động |

> **BỔ SUNG — CẦN PHÂN BIỆT HAI TRƯỜNG HỢP**

**Trường hợp A – mất kết nối tới máy chủ nhưng SIM vẫn có sóng:**
AI, cảm biến, LCD và lưu cục bộ vẫn có thể hoạt động; SMS có thể vẫn hoạt động nếu dịch vụ di động còn khả dụng.

**Trường hợp B – mất cả mạng di động:**
AI, cảm biến, LCD và lưu cục bộ vẫn hoạt động; Web, trợ lý AI và SMS không thể truyền ra ngoài cho tới khi kết nối được khôi phục.

Điểm này nên được giải thích vì rất dễ bị BGK hỏi.

---

## 3.6. Chu kỳ hoạt động của hệ thống

Đây là phần cần làm rõ để tránh việc tài liệu lúc nói “liên tục”, lúc nói “3 lần/ngày”, lúc nói “từng phút”.

| Tác vụ            | Chu kỳ/tần suất thực tế       | Nguồn xác nhận     |
| ----------------- | ----------------------------- | ------------------ |
| Camera tự động    | 3 lần/ngày – giờ cụ thể: ...  | Mã nguồn/cấu hình  |
| Chụp theo yêu cầu | Khi người dùng thao tác       | Demo               |
| AI phân loại      | Mỗi ảnh được đưa vào hệ thống | Mã nguồn           |
| Đọc NPK           | ...                           | Mã nguồn           |
| Đọc nhiệt độ      | ...                           | Mã nguồn           |
| Đọc độ ẩm         | ...                           | Mã nguồn           |
| Ghi SQLite        | ...                           | Mã nguồn           |
| Đồng bộ Web       | ...                           | Mã nguồn           |
| Kiểm tra mạng     | ...                           | Mã nguồn           |
| Cảnh báo          | Khi đạt điều kiện đã cấu hình | Logic chương trình |

**Các ô ... mở source code và điền đúng.**

Và nhớ đính kèm link source code ở phần phụ lục .

---

# CHƯƠNG 4. HƯỚNG DẪN SỬ DỤNG SẢN PHẨM

Đây là chương cần **nhiều ảnh nhất và ít chữ nhất**.

## 4.1. Lắp đặt

### Bước 1. Chọn vị trí

Đặt sản phẩm tại vị trí cần quan sát.

### Bước 2. Điều chỉnh camera

Camera cần hướng về khu vực cây lúa cần theo dõi.

### Bước 3. Đặt cảm biến

Đưa các đầu dò xuống vị trí cần đo theo hướng dẫn kỹ thuật.

### Bước 4. Kiểm tra nguồn

Đảm bảo nguồn điện được cấp ổn định.

### Bước 5. Kiểm tra SIM

Xác nhận SIM7600 nhận mạng.

### Bước 6. Bật hệ thống

Khởi động sản phẩm.

> **CẦN CHỤP MỚI**

Tốt nhất nhóm thực hiện lại thao tác và chụp:

**6 ảnh = 6 bước.**

---

## 4.2. Khởi động sản phẩm

Sau khi bật nguồn:

1. Raspberry Pi khởi động.
2. Camera được kiểm tra.
3. Các cảm biến được kiểm tra.
4. Module SIM7600 được kiểm tra.
5. Màn hình hiển thị trạng thái.
6. Chương trình chính bắt đầu hoạt động.

> **CẦN CHÈN**

Ảnh màn hình khi:

- đang khởi động;
- hoạt động bình thường;
- có cảnh báo.

---

## 4.3. Chế độ tự động

Theo nội dung hiện tại, hệ thống thu nhận và phân tích hình ảnh **3 lần/ngày**.

> **CẦN XÁC MINH**

- Mấy giờ sáng?
- Mấy giờ trưa?
- Mấy giờ chiều?
- Cảm biến bao lâu đọc một lần?
- Dữ liệu bao lâu đồng bộ?

Nên làm bảng:

| Hoạt động      | Chu kỳ                       |
| -------------- | ---------------------------- |
| Camera tự động | ...                          |
| Đọc sensor     | ...                          |
| AI inference   | Theo mỗi ảnh                 |
| Đồng bộ Web    | ...                          |
| Cảnh báo       | Khi điều kiện được kích hoạt |

> **NÊN CÓ TIMELINE**

**07:00 → 12:00 → 17:00**

Nếu có phần set up giờ trong code.

---

## 4.4. Chế độ người dùng chủ động

Khi muốn kiểm tra ngoài lịch tự động, người dùng có thể thực hiện kiểm tra trực tiếp tại thiết bị.

Nếu sản phẩm thực sự hỗ trợ thao tác từ Web thì mô tả thêm.

> **CẦN CHÈN**

Ảnh tay người dùng bấm nút.

Nếu có nút trên Web → screenshot.

---

## 4.5. Hướng dẫn sử dụng Web

Nên chiếm khoảng **1–2 trang**.

### Các thành phần cần đánh số trên giao diện

1. Trạng thái thiết bị.
2. Ảnh mới nhất.
3. Kết quả AI.
4. NPK.
5. Nhiệt độ.
6. Độ ẩm.
7. Lịch sử.
8. Cảnh báo.
9. Trợ lý AI.

> **BỔ SUNG — NÊN CÓ LUỒNG THAO TÁC NGƯỜI DÙNG**

Ví dụ:

**Đăng nhập → Chọn trạm → Xem trạng thái → Xem dữ liệu/ảnh → Kiểm tra cảnh báo → Xem lịch sử → Hỏi trợ lý nếu cần.**

Nếu Web có nút chụp theo yêu cầu:

**Chọn trạm → Chụp ảnh → Chờ xử lý → Nhận kết quả → Xem confidence/ảnh.**

---

## 4.6. Xử lý một số tình huống thường gặp

Dưới đây là bảng tham khảo:

| Hiện tượng                | Nguyên nhân có thể  | Cách xử lý              |
| ------------------------- | ------------------- | ----------------------- |
| Không có hình ảnh         | Camera chưa kết nối | Kiểm tra camera/USB     |
| Không có dữ liệu cảm biến | Dây hoặc đầu dò     | Kiểm tra kết nối/vị trí |
| Web chưa cập nhật         | Kết nối mạng        | Kiểm tra SIM/4G         |
| SMS không gửi             | Không có sóng       | Kiểm tra SIM/tín hiệu   |
| Độ tin cậy thấp           | Ảnh không rõ        | Chụp lại ảnh            |
| Dữ liệu chưa lên server   | Mất kết nối         | Chờ đồng bộ lại         |

---

## 4.7. Tắt và thu hồi sản phẩm

Phần hướng dẫn sử dụng nên có cả cách kết thúc vận hành.

### Bước 1. Dừng hoạt động

Dừng chế độ tự động hoặc chương trình chính theo cách nhóm đã thiết kế.

### Bước 2. Chờ hoàn tất ghi dữ liệu

Đảm bảo dữ liệu đang xử lý đã được lưu trước khi ngắt nguồn.

### Bước 3. Tắt nguồn

Không ngắt điện đột ngột nếu Raspberry Pi đang ghi dữ liệu vào thẻ nhớ.

### Bước 4. Thu đầu dò

Tháo các đầu cảm biến khỏi đất và vệ sinh phù hợp.

### Bước 5. Kiểm tra camera và hộp thiết bị

Lau camera, kiểm tra bùn, nước, dây kết nối và các vị trí có dấu hiệu bất thường.

### Bước 6. Ghi nhận tình trạng sau sử dụng

Nếu xuất hiện lỗi hoặc hư hỏng, ghi lại để phục vụ lần thử tiếp theo.

> **CẦN CHÈN**

1–2 ảnh thao tác thu hồi/vệ sinh thiết bị nếu có thể.

---

# CHƯƠNG 5. CÔNG NGHỆ VÀ QUÁ TRÌNH XÂY DỰNG

## 5.1. Bộ dữ liệu

Nhóm sử dụng bộ dữ liệu có tổng quy mô hiện được ghi nhận là **10.407 ảnh**.

Nguồn gồm:

- Paddy Doctor;
- hình ảnh bổ sung từ thực địa.

Cần lập bảng:

| Nguồn           | Số ảnh |
| --------------- | -----: |
| Paddy Doctor    | X      |
| Ảnh nhóm tự thu | X      |
| Tổng            | 10.407 |

Tiếp theo:

| Tập        | Số ảnh |
| ---------- | -----: |
| Train      | X      |
| Validation | X      |
| Test       | X      |

Không nên chỉ ghi tỷ lệ 80/10/10.

> **BỔ SUNG — CẦN GHI THÊM CÁCH XÁC NHẬN NHÃN**

| Nguồn                  | Ai/nguồn xác nhận nhãn   |
| ---------------------- | ------------------------ |
| Paddy Doctor           | Nhãn theo bộ dữ liệu gốc |
| Ảnh nhóm tự thu        | ...                      |
| Ảnh thực địa dùng test | ...                      |

Có thể bổ sung là kỹ sư hay chuyên gia nông nghiệp mà nhóm đã mời xác nhận.

---

## 5.2. 10 trạng thái phân loại

Nên làm **grid 2 × 5**.

Mỗi ô:

- 1 ảnh;
- tên tiếng Anh;
- tên tiếng Việt.

Không để 10 tên thành danh sách chữ đơn thuần.

> **BỔ SUNG**

Caption chung nên ghi:

> **Mười trạng thái mà mô hình hiện được huấn luyện để phân loại, gồm 9 nhóm bệnh hoặc biểu hiện sâu hại và 1 trạng thái bình thường.**

---

## 5.3. Huấn luyện mô hình

Tài liệu chính chỉ giữ:

- YOLO11s-cls;
- 224 × 224;
- pretrained ImageNet;
- tối đa 100 epoch;
- early stopping.

> **CHUYỂN PHỤ LỤC**

- learning rate;
- momentum;
- weight decay;
- warmup;
- toàn bộ augmentation.

> **BẮT BUỘC KIỂM TRA**

Nếu Mosaic không thực sự được áp dụng trong lần huấn luyện mô hình phân loại thì bỏ nội dung này.

| Kỹ thuật | Xác suất | Mô tả                                                                                   |
| -------- | -------: | --------------------------------------------------------------------------------------- |
| Mosaic   | 1,0      | Ghép bốn ảnh; chủ yếu dùng cho bài toán phát hiện đối tượng và tắt trong 10 epoch cuối. |

---

## 5.4. Kết quả huấn luyện

Dùng **1 biểu đồ training**.

Không cần hai trang bảng.

Sau biểu đồ chỉ giải thích:

- loss giảm;
- accuracy tăng;
- mô hình hội tụ.

Nhưng các con số phải được kiểm tra lại trước.

---

## 5.5. GradCAM

Dùng hình có sẵn:

**Ảnh gốc → heatmap → kết quả.**

Nên viết:

> Trong các ví dụ được kiểm tra, bản đồ nhiệt cho thấy mô hình tập trung nhiều vào các vùng lá có biểu hiện bất thường.

> **BỔ SUNG**

Mỗi ví dụ GradCAM nên ghi:

**Nhãn đúng:** ...
**Dự đoán:** ...
**Độ tin cậy:** ...
**Nhận xét vùng chú ý:** ...

Nên có cả:

- một trường hợp AI dự đoán đúng;
- nếu có thể, một trường hợp AI dự đoán sai.

Như vậy GradCAM có giá trị phân tích hơn.

---

## 5.6. Lưu trữ và đồng bộ dữ liệu

Dùng sơ đồ đơn giản:

```text
Raspberry Pi
     ↓
   SQLite
     ↓
  Có mạng?
   ↙    ↘
Không     Có
  ↓        ↓
Lưu cục bộ  Đồng bộ lên MySQL
```

> **BỔ SUNG — NÊN CÓ MỘT BÀI TEST RIÊNG**

1. Đếm số bản ghi trước khi ngắt mạng.
2. Ngắt kết nối tới máy chủ.
3. Tạo thêm X bản ghi.
4. Kiểm tra các bản ghi nằm trong SQLite.
5. Khôi phục kết nối.
6. Kiểm tra X bản ghi được đồng bộ.
7. Kiểm tra có thiếu/trùng bản ghi hay không.

---

## 5.7. Trợ lý AI

Không đưa System Prompt dài vào.

Chỉ cần sơ đồ:

**AI result + sensor data + user question**

↓

GPT-4o-mini

↓

**Response**

Có thêm box:

> **Lưu ý:** Nội dung tư vấn chuyên môn cần được kiểm chứng bằng nguồn nông nghiệp phù hợp. Lưu ý AI có thể sai...

> **BỔ SUNG — NÊN PHÂN BIỆT**

**Dữ liệu đầu vào từ hệ thống:**
Kết quả AI + NPK + nhiệt độ + độ ẩm + câu hỏi.

**Vai trò của trợ lý:**
Giải thích, tổng hợp thông tin, hỗ trợ tra cứu.

**Không được coi là:**
Công cụ tự động quyết định thuốc, liều lượng hoặc thay thế cán bộ nông nghiệp.

---

# CHƯƠNG 6. KIỂM THỬ VÀ KẾT QUẢ THỰC NGHIỆM

Đây nên là **chương quan trọng cần đầu tư**

## 6.1. Phương pháp kiểm thử

Nên dùng bảng:

| Nội dung       | Điều kiện       | Số lần/mẫu | Tiêu chí        |
| -------------- | --------------- | ---------: | --------------- |
| AI trên bộ ảnh | Bộ ảnh kiểm thử | 120        | đúng/sai        |
| AI thực địa    | Ngoài ruộng     | 30         | đúng/sai        |
| Cảnh báo       | Ngoài ruộng     | 20         | thành công      |
| Sensor         | Ngoài ruộng     | 20         | thu dữ liệu     |
| Web            | Ngoài ruộng     | 25         | truyền/hiển thị |

> **CẦN BỔ SUNG**

“Đúng” được xác định thế nào?

Đặc biệt AI field:

> Ai xác nhận 26/30 là đúng?

Đây là câu BGK có thể hỏi.

---

### 6.1.1. Tiêu chí xác định một lượt kiểm thử thành công

| Hạng mục       | Một lượt được tính là thành công khi...                                                                                   |
| -------------- | ------------------------------------------------------------------------------------------------------------------------- |
| AI trên ảnh    | Nhãn dự đoán trùng với nhãn được dùng để đối chiếu                                                                        |
| AI ngoài ruộng | Kết quả hệ thống trùng với kết quả đối chiếu theo phương pháp nhóm đã xác định                                            |
| Sensor         | Thiết bị đọc được dữ liệu, dữ liệu được lưu/hiển thị hợp lệ và không phát sinh lỗi kết nối                                |
| Cảnh báo       | Điều kiện cảnh báo được kích hoạt và tin nhắn/thông báo tới được thiết bị người dùng trong khoảng thời gian nhóm quy định |
| Web            | Dữ liệu được truyền và hiển thị đúng với bản ghi tại thiết bị                                                             |
| Lưu cục bộ     | Dữ liệu vẫn được ghi khi máy chủ không kết nối                                                                            |
| Đồng bộ        | Dữ liệu offline được đưa lên server sau khi có kết nối mà không thiếu/trùng                                               |

> **CẦN CHỐT**

Đội phải tự xác định cụ thể:

> “trong bao lâu thì SMS được coi là thành công?”

Ví dụ 10 giây, 30 giây hay 1 phút phải dựa trên quy trình test thực tế, không tự đặt sau khi test.

---

## 6.2. Kiểm thử trong điều kiện thử nghiệm

Viết:

> Trước khi đưa sản phẩm xuống ruộng, nhóm kiểm tra riêng từng thành phần gồm camera, cảm biến, hệ thống xử lý, kết nối 4G, Web và chức năng cảnh báo.

> **CẦN CHÈN**

Ảnh nhóm đang test trên bàn.

Hiện đã có ảnh nhưng nên chọn 1–2 ảnh rõ hơn.

> **VỀ CẢM BIẾN**

Nếu có dữ liệu hiệu chuẩn thật:

| Thiết bị chuẩn | Sensor | Sai số |
| -------------- | ------ | ------ |

Nếu không có:

**bỏ từ “hiệu chuẩn”.**

> **BỔ SUNG**

Nếu chưa có thiết bị chuẩn, có thể kiểm tra theo hướng:

> **độ ổn định và phản ứng của cảm biến**

Ví dụ:

- đọc lặp lại nhiều lần tại cùng vị trí;
- thay đổi độ ẩm để xem sensor có phản ứng;
- thay đổi độ sâu cắm;
- ghi raw data.

Không biến bài test này thành “độ chính xác cảm biến” nếu chưa có chuẩn đối chiếu.

---

## 6.3. Kết quả trí tuệ nhân tạo

| Đánh giá      | Dataset | N   | Metric         | Kết quả   |
| ------------- | ------- | --: | -------------- | --------: |
| Validation    | ...     | ... | Top-1          | ...       |
| Test          | ...     | ... | Accuracy       | ...       |
| 120 ảnh       | ...     | 120 | Accuracy       | 99,2%     |
| Ngoài ruộng   | Field   | 30  | Tỷ lệ đúng     | 86,7%     |

Sau đó xác định:

**94,20% là gì?**
→ tập nào, epoch nào?

**98,14% là gì?**
→ tập nào, file nào?

**99,2% là gì?**
→ 119/120 ảnh.

**86,7% là gì?**
→ 26/30 lượt ngoài thực địa.

---

## 6.4. Kiểm thử ngoài đồng ruộng

Đây là **trang vàng**.

Làm to:

### 86,7%

Phân loại trạng thái

### 90%

Cảnh báo

### 95%

Dữ liệu đất

### 92%

Theo dõi Web

Bên dưới là bảng chi tiết.

| Chức năng | Thử | Thành công | Tỷ lệ | Vấn đề                     |
| --------- | --: | ---------: | ----: | -------------------------- |
| AI        | 30  | 26         | 86,7% | ảnh mờ, ánh sáng, nhầm lớp |
| Cảnh báo  | 20  | 18         | 90%   | kết nối                    |
| Sensor    | 20  | 19         | 95%   | đầu dò                     |
| Web       | 25  | 23         | 92%   | mạng                       |

> **CẦN CHÈN**

Ảnh thật ở ruộng.

Ảnh sản phẩm.

Ảnh nhóm kiểm tra điện thoại.

---

## 6.5. Các trường hợp chưa thành công

Đây nên là mục riêng.

### Trường hợp 1: ảnh bị mưa làm mờ

→ AI phân loại sai.

### Trường hợp 2: ánh sáng thay đổi

→ chất lượng ảnh giảm.

### Trường hợp 3: cảm biến đặt sai độ sâu

→ dữ liệu không phù hợp.

### Trường hợp 4: mạng không ổn định

→ Web/SMS chậm.

> **BỔ SUNG — NÊN TRÌNH BÀY MỖI FAILURE THEO 4 Ô**

**Hiện tượng → Bằng chứng → Nguyên nhân dự kiến → Hành động tiếp theo**

Ví dụ:

**Ảnh camera bị mờ**

**Bằng chứng:** ảnh X tại thời điểm Y.

**Nguyên nhân:** nước mưa trên mặt kính.

**Ảnh hưởng:** AI dự đoán sai.

**Hướng cải tiến:** che camera tốt hơn + kiểm tra chất lượng ảnh trước inference.

Nếu còn ảnh lỗi thật thì **nhất định chèn**.

---

## 6.6. Điều nhóm rút ra từ kiểm thử

Phần này nên có ngay sau failure cases.

### 1. Kết quả trên bộ ảnh không phản ánh hoàn toàn điều kiện ngoài ruộng

Kết quả 119/120 cao hơn đáng kể so với 26/30 ngoài thực địa. Điều này cho thấy các yếu tố như ánh sáng, mưa, góc camera và chất lượng ảnh có ảnh hưởng lớn.

### 2. Cách lắp đặt cảm biến là một phần của hệ thống

Một lần test không thành công do đầu dò chưa đúng độ sâu cho thấy kết quả không chỉ phụ thuộc sensor mà còn phụ thuộc cách sử dụng.

### 3. Kết nối vẫn là một giới hạn

4G và SMS giúp tăng khả năng liên lạc nhưng không loại bỏ được hoàn toàn lỗi mạng.

### 4. Cần kiểm tra toàn bộ chuỗi, không chỉ từng thành phần

Một mô hình AI tốt chưa đồng nghĩa sản phẩm thực tế sẽ luôn cho kết quả tốt nếu camera, mạng hoặc thao tác người dùng gặp vấn đề.

---

# CHƯƠNG 7. PHẢN HỒI NGƯỜI DÙNG, GIỚI HẠN VÀ CẢI TIẾN

## 7.1. Phản hồi thực tế

nên thêm người dùng ....

### Nguyễn Thanh Khương

**Kinh nghiệm:** hơn 25 năm trồng lúa.

**Địa điểm:** Phương Thịnh – Đồng Tháp.

**Nội dung trải nghiệm:**
Theo dõi kết quả nhận diện, dữ liệu và giao diện.

**Nhận xét chính:**
Ý tưởng có tính thực tế nhưng cần tiếp tục cải thiện độ chính xác và đơn giản hóa cách sử dụng.

### Người có chuyên môn

Phải điền đúng:

- Họ tên.
- Chuyên môn.
- Đơn vị nếu có.

> **BỔ SUNG**

Đối với mỗi người nên ghi thêm:

**Người này đã trực tiếp trải nghiệm gì?**

Ví dụ:

- xem kết quả AI;
- xem Web;
- nhận SMS;
- xem dữ liệu sensor;
- thao tác trực tiếp.

Như vậy feedback có bối cảnh hơn.

---

## 7.2. Từ phản hồi đến cải tiến

| Phản hồi/vấn đề         | Bằng chứng nhóm ghi nhận    | Nhóm hiểu vấn đề gì                  | Hành động tiếp theo                           |
| ----------------------- | --------------------------- | ------------------------------------ | --------------------------------------------- |
| Cần tăng độ chính xác   | 26/30 ngoài ruộng           | Dữ liệu thực tế khó hơn tập ảnh      | Thu thêm ảnh thực địa, kiểm tra ánh sáng/mưa  |
| Cần dễ sử dụng          | Người dùng góp ý            | Người dùng không muốn thao tác nhiều | Giữ chế độ tự động, giảm số bước trên Web     |
| Thiết bị cần bền        | Camera bị ảnh hưởng bởi mưa | Thiết kế ngoài trời cần test thêm    | Cải thiện che chắn, test nước/nhiệt           |
| Mạng chập chờn          | 18/20 cảnh báo, 23/25 Web   | Kết nối ảnh hưởng trải nghiệm        | Lưu local, retry, hiển thị trạng thái offline |
| Sensor phụ thuộc vị trí | 1 lượt lỗi do độ sâu        | Quy trình lắp đặt ảnh hưởng dữ liệu  | Chuẩn hóa độ sâu và thử nhiều vị trí          |

> **Feedback → Evidence → Lesson → Action.**

---

## 7.3. Giới hạn hiện tại

Nên thể hiện dưới dạng **6 icon**, không phải đoạn văn dài.

### Camera

Chỉ quan sát một vùng.

### Sensor

Chỉ phản ánh vị trí đặt.

### AI (YOLO)

Bị ảnh hưởng bởi ánh sáng, mưa, góc chụp.

### Network

Một số chức năng phụ thuộc mạng di động.

### Power

Chưa kiểm thử dài cả mùa vụ.

### AI assistant (Chatbot)

Cần nguồn kiến thức được kiểm chứng.

Đây là phần rất có giá trị.

---

## 7.4. Những gì đã chứng minh và chưa chứng minh đầy đủ

Nên có một trang hoặc nửa trang rất rõ.

### Sản phẩm hiện đã có bằng chứng

✓ Camera và hệ thống xử lý hình ảnh hoạt động.

✓ Mô hình AI đã được triển khai và chạy inference.

✓ Cảm biến đã được tích hợp và đọc dữ liệu.

✓ LCD hiển thị được thông tin.

✓ Web đã hiển thị dữ liệu/hình ảnh.

✓ SMS đã được gửi trong các lượt thử.

✓ Sản phẩm đã được đưa ra ngoài ruộng.

✓ Có kết quả thực nghiệm với số lượt cụ thể.

✓ Có người dùng trải nghiệm và phản hồi.

### Chưa được chứng minh đầy đủ

△ Một camera có thể đại diện cho toàn bộ thửa ruộng.

△ Một vị trí cảm biến có thể đại diện cho toàn bộ ruộng.

△ Sản phẩm hoạt động ổn định 24/7 trong thời gian dài.

△ Toàn bộ hệ thống đạt IP65.

△ Nguồn mặt trời đảm bảo vận hành liên tục.

△ Sản phẩm làm giảm bao nhiêu phân bón.

△ Sản phẩm làm giảm bao nhiêu thuốc bảo vệ thực vật.

△ Sản phẩm giúp tăng bao nhiêu năng suất.

△ Hiệu quả kinh tế khi triển khai diện rộng.

△ Trợ lý AI luôn cung cấp tư vấn nông nghiệp chính xác.

Đây là phần nên có vì nó cho thấy **đội hiểu rõ giới hạn của sản phẩm**.

---

# CHƯƠNG 8. KHẢ NĂNG TRIỂN KHAI VÀ HƯỚNG PHÁT TRIỂN

## 8.1. Chi phí các linh kiện chính

Giữ bảng hiện tại nhưng đổi tên nếu chưa đủ toàn bộ chi phí:

> **Chi phí các linh kiện chính của sản phẩm**

Thay vì:

> “Tổng chi phí sản phẩm”.

Vì còn:

- tấm pin năng lượng mặt trời;
- hộp;
- ADS1115;
- USB-RS485;
- thẻ nhớ;
- SIM;
- máy chủ;
- dữ liệu 4G;
- API AI.

> **BỔ SUNG — NÊN CHIA RÕ**

**Chi phí chế tạo ban đầu**

→ linh kiện, hộp, dây, khung, pin...

**Chi phí vận hành**

→ SIM/data, server, AI API...

Nếu chưa có đủ số liệu thì chỉ trình bày phần đầu và ghi:

> Chi phí vận hành chưa được tính đầy đủ trong giai đoạn hiện tại.

---

## 8.2. Khả năng tiếp tục triển khai


> Các thành phần chính của sản phẩm sử dụng phần cứng phổ biến và thiết kế theo dạng module, tạo điều kiện cho việc thay thế, nâng cấp và tiếp tục thử nghiệm.

Ở giai đoạn hiện tại:

> Việc triển khai trên diện rộng, đánh giá tuổi thọ thiết bị, hiệu quả kinh tế và mức giảm phân bón hoặc thuốc bảo vệ thực vật vẫn cần nghiên cứu dài hạn hơn.

---

## 8.3. Hướng phát triển

| Giới hạn                    | Bước tiếp theo                      |
| --------------------------- | ----------------------------------- |
| Độ chính xác thực địa 86,7% | Bổ sung ảnh thực địa                |
| Camera một vùng             | Nghiên cứu nhiều điểm quan sát      |
| Cảm biến tại một điểm       | Thử nghiệm nhiều vị trí đo          |
| Nguồn chưa kiểm thử dài hạn | Kiểm thử tiêu thụ và thời lượng     |
| Trợ lý AI                   | Xây dựng nguồn kiến thức kiểm chứng |
| Kiểm thử thực địa ngắn hạn  | Thử qua nhiều giai đoạn mùa vụ      |

---

## 8.4. Phân công thành viên


| Thành viên           | Phần phụ trách |
| -------------------- | -------------- |
| Đoàn Hồng Ngọc       | ...            |
| Nguyễn Thanh Khiêm   | ...            |
| Huỳnh Nguyễn Thư Kỳ  | ...            |
| Thạch Trần Đăng Khoa | ...            |

Không chỉ ghi:

> Trưởng nhóm / Thành viên.

---

## 8.5. Tác động hiện tại và tác động kỳ vọng


### Tác động hiện tại đã có bằng chứng

- sản phẩm đã được chế tạo và vận hành;
- đã thử ngoài điều kiện thực tế;
- có khả năng cung cấp thêm dữ liệu hình ảnh và đất tại vị trí quan trắc;
- có thể giúp người dùng theo dõi thông tin từ xa trong các lượt thử;
- giúp người dùng có thêm dữ liệu trước khi đưa ra quyết định canh tác;
- đã nhận được phản hồi từ người sử dụng để tiếp tục cải tiến.

### Tác động kỳ vọng

Nếu sản phẩm được tiếp tục kiểm thử và hoàn thiện, nhóm kỳ vọng có thể:

- hỗ trợ giảm công kiểm tra thủ công;
- hỗ trợ phát hiện dấu hiệu bất thường sớm hơn;
- hỗ trợ sử dụng phân bón và thuốc bảo vệ thực vật hợp lý hơn;
- góp phần giảm chi phí và tác động môi trường.



---

# TÀI LIỆU THAM KHẢO

Ngoài sách, phải có **nguồn trực tiếp mà dự án dùng**:

- Paddy Doctor.
- Ultralytics YOLO11.
- GradCAM.
- Raspberry Pi.
- SIM7600.
- Datasheet NPK.
- DS18B20.
- ADS1115.
- OpenAI.
- Tài liệu chuyên môn bệnh lúa.
- Nguồn thuốc BVTV nếu chatbot nhắc tới.
- Nguồn số liệu trong Chương 1.

---

# PHỤ LỤC KỸ THUẬT
phần này là những gì dài quá mà các em trình bày ở trên thì có thể đưa xuống đây phần trên chỉ cần trình bày cơ bản cho giám khảo hiểu là được , chi tiết có thể để ở phụ lục

## Phụ lục A. Sơ đồ dây

Sơ đồ dây.

## Phụ lục B. State machine

State machine.

## Phụ lục C. Sequence diagram

Sequence diagram.

## Phụ lục D. API

API.

## Phụ lục E. Cơ sở dữ liệu

Database.

## Phụ lục F. Cấu hình huấn luyện đầy đủ

Full training config.

## Phụ lục G. Augmentation

Augmentation.

## Phụ lục H. Biểu đồ huấn luyện và ma trận nhầm lẫn

Training curves + confusion matrix.

## Phụ lục I. Nhật ký kiểm thử thực địa

Raw field test.

## Phụ lục J. Mã nguồn và tài nguyên dự án

Phụ lục này nên được bổ sung vì đây là bằng chứng cho thấy đội có sản phẩm thật và có thể truy xuất phần kỹ thuật. Không nên đưa các đoạn mã dài vào tài liệu chính.

### Danh mục tài nguyên đề xuất

| Hạng mục              | Nội dung                              | Đường dẫn      |
| --------------------- | ------------------------------------- | -------------- |
| Mã nguồn Raspberry Pi | Thu thập sensor, camera, AI, cảnh báo | GitHub / Drive |
| Mã nguồn Web          | Giao diện quản lý và theo dõi         | GitHub / Drive |
| Backend/API           | Nhận dữ liệu, đồng bộ, chatbot        | GitHub / Drive |
| Mô hình AI            | File model, config, checkpoint        | Link lưu trữ   |
| Dataset               | Cấu trúc dữ liệu, thống kê, nguồn     | Link / mô tả   |
| Kết quả training      | `results.csv`, biểu đồ, log           | Link           |
| Nhật ký 120 ảnh       | Danh sách file + kết quả              | Link           |
| Nhật ký field test    | 30 AI, 20 SMS, 20 sensor, 25 Web      | Link           |
| Video demo            | Sản phẩm hoạt động thực tế            | Link           |
| Tài liệu kỹ thuật     | Wiring, API, database, hướng dẫn      | Link           |



---
