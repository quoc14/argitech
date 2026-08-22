# Ghi chú meeting buổi 1 — Góp ý kịch bản video

> **Lưu ý từ anh:** Những góp ý dưới đây chỉ mang tính tham khảo. Các em nên luôn đặt câu hỏi “Tại sao?” trước mỗi đề xuất và chủ động lựa chọn điều phù hợp với sản phẩm, câu chuyện cũng như điều kiện thực tế của đội. Nếu các em thấy quan điểm và cách làm hiện tại của mình là hợp lý, hãy tự tin giữ vững . Mình cứ là mình thôi. Cố lên các em!
>
## Cách đọc ký hiệu 

Trong tài liệu này, các ký hiệu như `D21` hoặc `D24:D26` dùng để chỉ vị trí nội dung trong file kịch bản Sheet:

- Chữ cái là **tên cột**. Ví dụ: `D` là cột D, hiện đang chứa phần **lời thoại**.
- Con số là **số hàng**. Ví dụ: `21` là hàng 21.
- Vì vậy, `D21` nghĩa là **ô nằm ở cột D, hàng 21**.
- Ký hiệu `D24:D26` nghĩa là **các ô từ D24 đến D26**, tức cột D từ hàng 24 đến hàng 26.


## 1. Thời lượng và mục tiêu của video

Kịch bản hiện có khoảng **2.027 từ**, tương đương khoảng **15 phút 35 giây** ở tốc độ 130 từ/phút. Con số này chưa tính khoảng nghỉ, diễn xuất, demo, phỏng vấn và chuyển cảnh.

Nên đặt mục tiêu bản xuất cuối khoảng **13 phút 20 giây**, chừa ít nhất 40–60 giây an toàn so với giới hạn 15 phút. Mục tiêu lời thoại khoảng **1.400–1.550 từ**, vì phần demo cần khoảng lặng để người xem quan sát màn hình và kết quả.

Kịch bản cần có một phân đoạn demo **đầu vào → xử lý → đầu ra** đủ rõ và liên tục. Nên đưa demo thật lên trước, dành thời lượng cho testing và để hình ảnh (sơ đồ) cho phần giải thích kỹ thuật để không phải nói hay liệt kê nhiều.

## 2. Mạch kể chuyện

### Mạch hiện tại

```text
Vấn đề
→ giới thiệu nhiều chức năng
→ giải thích kỹ thuật
→ dữ liệu AI
→ chatbot/web
→ phỏng vấn
→ kết
```

### Mạch đề xuất

```text
Khoảnh khắc sản phẩm chạy
→ vấn đề thật
→ đội và giải pháp
→ demo
→ testing có số
→ quá trình cải tiến
→ người dùng thật
→ khả thi, giới hạn và lời kết
```

## 3. Mỗi điều đưa ra phải có minh chứng

| Điều muốn nói | Minh chứng phải hiện |
|---|---|
| AI phân loại bệnh | Ảnh đầu vào, kết quả lớp bệnh, confidence và thời gian xử lý |
| AI chạy tại trạm | Cảnh Raspberry Pi đang xử lý hoặc log chạy model trên Pi |
| Theo dõi dữ liệu đất | Giá trị NPK/nhiệt độ/độ ẩm trên LCD hoặc dashboard |
| Có cảnh báo | Điện thoại nhận SMS/cuộc gọi thật trong cùng một tình huống demo |
| Hoạt động khi mất mạng | Ngắt mạng, dữ liệu lưu SQLite, kết nối lại và đồng bộ |
| Chatbot dùng ngữ cảnh ruộng | Câu hỏi, dữ liệu ngữ cảnh và câu trả lời liên quan cùng xuất hiện |
| AI có kết quả tốt | Test setup, số mẫu, số đúng/sai và trường hợp sai |
| Người dùng thấy hữu ích | Người dùng thao tác và phản hồi tự nhiên, không đọc lời quảng cáo |

> Không nhất thiết phải đưa toàn bộ các minh chứng trên vào video. Đội nên ưu tiên những phần mạnh nhất, quay được rõ ràng và có giá trị thuyết phục cao.

## 4. Góp ý theo từng phần của kịch bản

### 4.1. Mở đầu

Flycam, nông dân và học sinh hỏi chuyện là hướng tốt. Tuy nhiên, 30 giây đầu cần tạo ngay cảm giác: “Đây là vấn đề thật và sản phẩm này có lý do để tồn tại”.

Đoạn hiện tại:

> “Nếu một ngày, trên cánh đồng xuất hiện những dấu hiệu bệnh đầu tiên… Người nông dân có thể phát hiện ra trước khi cả cánh đồng bị ảnh hưởng hay không?”
>
> “Nếu đất đang thiếu dinh dưỡng, cây lúa đang gặp vấn đề… chúng ta có thể biết điều đó trước khi nhìn thấy hậu quả?”
>
> “Và nếu trí tuệ nhân tạo có thể trở thành một ‘đôi mắt’ quan sát đồng ruộng 24 giờ mỗi ngày thì sao?”

Ba câu hỏi liên tiếp hơi dài. Câu “đôi mắt quan sát đồng ruộng 24 giờ mỗi ngày” cũng mâu thuẫn với chế độ tự chụp ba lần/ngày.

Có thể thay bằng:

> Liệu có thể đặt một trạm ngay tại ruộng để theo dõi cây lúa, phân tích ảnh và cảnh báo sớm cho người nông dân?

Hoặc mở theo hướng:

> Một chiếc lá lúa vừa xuất hiện dấu hiệu bất thường. Nếu phát hiện muộn, cả ruộng có thể bị ảnh hưởng. Với người nông dân, việc phát hiện sớm không hề dễ, vì phần lớn vẫn dựa vào quan sát và kinh nghiệm.

Sau đó dẫn vào câu hỏi:

> Vậy có thể tạo một trạm đặt ngay tại ruộng, tự quan sát cây lúa, đo đất và cảnh báo sớm cho người nông dân hay không?

### 4.2. Chế độ hoạt động và sáu chức năng

Đoạn hiện tại:

> AgriTech hoạt động linh hoạt ở hai chế độ: chế độ tự động, mỗi ngày tự chụp và phân tích ba lần; và chế độ người dùng, khi cần người dùng có thể ấn nút điều khiển tại trạm hoặc gián tiếp qua web.
>
> Mọi người có thể hình dung AgriTech giống như một “trợ lý nông nghiệp thông minh” luôn túc trực 24/7 ngoài cánh đồng. Nhóm chúng em đã nghiên cứu và tích hợp cho trạm sáu chức năng cốt lõi để quan sát, phân tích và hỗ trợ người dân, bao gồm:
>
> - Nhận diện bệnh trên cây lúa bằng AI.
> - Đưa ra phác đồ điều trị chuẩn khoa học.
> - Giám sát chất lượng đất: nồng độ NPK, nhiệt độ và độ ẩm.
> - Theo dõi và cảnh báo khi phát hiện các dấu hiệu bất thường.
> - Trợ lý ảo giúp tư vấn trực tiếp cho người nông dân và trả lời các thắc mắc về kỹ thuật canh tác.
> - Quản lý và theo dõi cánh đồng từ xa qua web trên điện thoại.

**Vấn đề:** việc liệt kê sáu chức năng mất hơn một phút nhưng chưa tạo bằng chứng. “Trợ lý 24/7” mâu thuẫn với lịch chụp, còn “phác đồ điều trị chuẩn khoa học” là khẳng định chưa có đủ cơ sở.

**Cách sửa:** gom thành ba giá trị người dùng dễ nhớ:

1. Quan sát cây bằng camera và AI.
2. Theo dõi chỉ số đất bằng cảm biến.
3. Gửi dữ liệu, cảnh báo và gợi ý tham khảo tới người dùng.

Không cần đọc nguyên danh sách các tech stack được sử dụng.

**Cách nói an toàn:**

> AgriTech hỗ trợ phân loại tình trạng bệnh từ ảnh lá lúa, theo dõi một số chỉ số đất và gửi kết quả tới người dùng qua LCD, web hoặc cảnh báo từ xa.

### 4.3. Cấu tạo và chu trình tổng quát (`D21`, `D23`)

`D21` hơi dài và lặp lại phần chức năng. `D23` tiếp tục tóm tắt chính nội dung vừa nói.

Nên dùng một sơ đồ đơn giản vì nếu nói quá nhiều, người nghe có thể không nắm được luồng hoạt động:

```text
Camera/cảm biến
→ Raspberry Pi
→ AI/quy tắc
→ lưu dữ liệu
→ LCD/web/SMS
```

Thời lượng phần này nên khoảng 25–30 giây.

### 4.4. Luồng hoạt động (`D24:D26`)

Phần này quá dài. Những nội dung về Raspberry Pi, OpenCV, YOLO, BGR sang RGB, normalize, Data Augmentation, MQTT/HTTP và SQLite rất hữu ích trong tài liệu, nhưng nếu đưa quá nhiều vào video sẽ làm người xem mất mạch.

Trong video, kỹ thuật chỉ cần phục vụ câu chuyện:

```text
Camera chụp ảnh
→ AI phân tích
→ cảm biến đo đất
→ Raspberry Pi xử lý
→ web/SMS/LCD hiển thị cảnh báo
```

Những chi tiết như Data Augmentation, normalize ảnh và giao thức truyền dữ liệu nên đưa vào tài liệu hoặc phụ lục.

**Không nên đọc trong video:**

- “hai tiến trình chạy song song”;
- BGR → RGB, JSON, MQTT/HTTP;
- “nút quyết định trung tâm”;
- “Ngắt ưu tiên (Interrupt)”;
- “Delay định sẵn”.

**Nên cho thấy:**

1. Camera lấy một ảnh cụ thể.
2. Model trả về lớp và confidence.
3. Cảm biến trả về số đo.
4. Hệ thống xác định trạng thái bình thường hoặc bất thường.
5. Kết quả được lưu và gửi tới người dùng.

**Lưu ý kỹ thuật:** YOLO11s-cls là mô hình **classification**. Nên dùng “phân loại tình trạng bệnh từ ảnh”, không dùng “phát hiện mầm bệnh” hoặc “khoanh vùng vết bệnh” nếu không có model detection riêng. GradCAM chỉ nên gọi là “heatmap” hoặc “vùng AI chú ý”.

### 4.5. Dataset và tiền xử lý AI (`D28:D32`)

Phần này hầu như là lý thuyết AI nhưng chưa nói rõ kết quả kiểm thử. Với BGK, **mô hình làm được gì và được test thế nào** quan trọng hơn phần lý thuyết về normalize hoặc Data Augmentation.

**Nên giữ trong 35–45 giây:**

- YOLO11s-cls, 10 lớp: 9 bệnh và 1 bình thường.
- Dataset 10.407 ảnh, chia train/validation/test theo tỷ lệ 80/10/10.
- Nguồn Paddy Doctor và ảnh thực địa, nếu đội có hồ sơ nguồn rõ.
- Kết quả benchmark đã được chốt và điều kiện test.

**Nên chuyển sang tài liệu:** 224 × 224, BGR → RGB, normalize `[0, 1]`, danh sách đầy đủ augmentation và giải thích image-level labeling.

**Phải xác minh trước khi nói:**

- Ảnh thực địa thực sự chiếm bao nhiêu ảnh và được thu ở đâu?
- Ai xác nhận nhãn? Chỉ nói “chuyên gia nông nghiệp xác định” nếu có người, quy trình và bằng chứng cụ thể.
- Ba con số 98,14%, 94,20% và 99,20% là các phép đo khác nhau như thế nào?

Khuyến nghị trong video: sử dụng kết quả dễ kiểm chứng nhất, chẳng hạn:

> Trong bài test riêng 120 ảnh trên Raspberry Pi, hệ thống phân loại đúng 119 ảnh; một ảnh Hispa bị nhầm thành Blast.

### 4.6. Đưa sản phẩm đến người dùng (`D34`)

Có thể dùng một đoạn phim tua nhanh về quá trình vận chuyển trạm, lắp đặt, người nông dân thao tác, xem LCD/web và phản hồi. Điều quan trọng là phải cho thấy người dùng thực sự thử sản phẩm.

Nên bổ sung để thể hiện quá trình làm việc:

- người dùng đã thử tác vụ nào;
- đội quan sát được điều gì;
- đội đã thay đổi gì sau phản hồi.

### 4.7. Chatbot (`D36:D37`)

Phần này nên dài khoảng 30–40 giây và được thể hiện bằng một screen recording rõ ràng.

**Demo đề xuất:**

1. Màn hình hiển thị kết quả AI và dữ liệu ruộng hiện tại.
2. Người dùng hỏi một câu cụ thể.
3. Chatbot trả lời có nhắc đúng ngữ cảnh đó.
4. Chèn nhãn: “Gợi ý tham khảo — không thay thế chuyên gia nông nghiệp”.

Nhãn trên là cần thiết vì AI vẫn cần con người kiểm chứng. Việc ghi rõ đây là nội dung do AI hỗ trợ cũng giúp cách trình bày minh bạch hơn.

Không gọi chatbot là “chuyên gia” theo nghĩa bảo đảm chuyên môn. Cách nói phù hợp hơn là “trợ lý AI được định hướng cho ngữ cảnh canh tác lúa”.

### 4.8. Web dashboard (`D39:D42`)

Nên quay màn hình trực tiếp, di chuột hoặc chạm chậm và crop đúng khu vực cần nhìn.

**Cần cho thấy tối thiểu:**

- thông tin trạm và thời điểm cập nhật;
- ảnh gần nhất và kết quả AI;
- NPK, nhiệt độ và độ ẩm;
- lịch sử hoặc biểu đồ;
- trạng thái cảnh báo;
- một lượt chatbot nếu cần thiết.

“Theo thời gian thực” chỉ dùng nếu dữ liệu cập nhật liên tục theo đúng nghĩa. Nếu trạm chụp ba lần/ngày, dùng “theo từng lần cập nhật” hoặc “được lưu theo thời gian”.

### 4.9. Phỏng vấn nông dân và kỹ sư (`D44:D45`)

Phần này cần tự nhiên nhất có thể, tổng thời lượng khoảng 30 giây đến 1 phút.

**Nông dân:** hỏi mở và để bác trả lời tự nhiên:

- “Khâu nào khi thăm ruộng làm bác mất nhiều thời gian nhất?”
- “Sau khi thử xem kết quả trên máy hoặc điện thoại, bác thấy phần nào dễ hoặc khó dùng?”
- “Nếu dùng ngoài ruộng lâu dài, bác muốn đội sửa điều gì?”

**Kỹ sư:** nên có một nhận xét và một giới hạn. Không nhờ chuyên gia khẳng định “phác đồ điều trị chuẩn khoa học” nếu chưa đánh giá phương pháp, nguồn khuyến nghị và thử nghiệm.

Nên ghi toàn bộ cuộc phỏng vấn, sau đó chọn những đoạn hợp lý. Có thể gửi câu hỏi trước, nhưng không nên để nhân vật học thuộc câu trả lời.

### 4.10. Định hướng và lời kết (`D49:D53`)

Phần này đang lặp các ý “đồng hành”, “bền vững” và “chủ động”, vì vậy có thể rút ngắn hơn.

Nên có đủ ba ý:

1. Hiện tại sản phẩm đã làm được gì.
2. Giới hạn còn lại là gì.
3. Bước kiểm chứng tiếp theo là gì.

## 5. Bảng thay thế câu chữ tham khảo

| Câu hiện tại | Nên đổi thành |
|---|---|
| “Quan sát đồng ruộng 24/7” | “Theo dõi định kỳ theo lịch cấu hình và hỗ trợ cảnh báo khi có bất thường.” |
| “Nhận diện/phát hiện mầm bệnh” | “Phân loại tình trạng bệnh từ ảnh lá lúa.” |
| “Đưa ra phác đồ điều trị chuẩn khoa học” | “Đưa ra gợi ý xử lý tham khảo dựa trên kết quả nhận dạng và dữ liệu ruộng.” |
| “Ngưỡng an toàn sinh thái” | “Ngưỡng cảnh báo được cấu hình cho từng chỉ số”; nêu nguồn nếu có. |
| “Dữ liệu được chuyên gia xác định” | Chỉ giữ khi có chuyên gia, quy trình xác nhận và bằng chứng; nếu không, mô tả đúng nguồn dữ liệu. |
| “Biểu đồ theo thời gian thực” | “Biểu đồ dữ liệu theo từng lần cập nhật.” |
| “AI đánh giá sức khỏe cây trồng” | “AI phân loại ảnh lá; hệ thống đồng thời ghi nhận một số chỉ số đất để hỗ trợ đánh giá tình trạng ruộng.” |
| “Gọi/SMS khẩn cấp” | “Gửi cảnh báo SMS/cuộc gọi khi điều kiện cảnh báo được kích hoạt.” |
| “Tư vấn sát thực tế nhất” | “Tạo gợi ý có tham chiếu dữ liệu hiện tại của ruộng.” |
| “Mang lại canh tác chính xác, hiệu quả hơn” | “Hướng tới hỗ trợ người dùng theo dõi và ra quyết định dựa trên dữ liệu.” |

## 6. Demo tham khảo

> Đây là gợi ý từ AI. Đội có thể sáng tạo theo hướng riêng; phần nào thật sự cần thiết và quay được rõ ràng thì đưa vào, không cần sử dụng toàn bộ.

### 6.1. Demo camera, AI và cảnh báo

Quay một mạch bản rộng để chứng minh tính liên tục, sau đó lấy thêm cận cảnh để dựng:

1. Hiện prototype và lá hoặc ảnh đầu vào trong cùng không gian.
2. Kích hoạt chụp bằng nút tại trạm hoặc web.
3. Cận camera và trạng thái đang xử lý.
4. Cận kết quả lớp bệnh, confidence và thời gian.
5. Hiện GradCAM cạnh ảnh gốc, gọi đúng là vùng AI chú ý.
6. Cận LCD hoặc dashboard cập nhật.
7. Điện thoại nhận SMS/cuộc gọi nếu điều kiện cảnh báo được kích hoạt.

### 6.2. Demo cảm biến và dashboard

- Quay đầu cảm biến đang đặt đúng cách.
- Hiện giá trị trên trạm và web với cùng thời điểm.
- Nếu tạo thay đổi môi trường để minh họa, nói rõ đó là tình huống test.
- Không khẳng định độ chính xác nếu chưa đối chiếu với thiết bị chuẩn.

### 6.3. Demo chatbot có ngữ cảnh

- Chuẩn bị một tình huống mà dữ liệu ruộng có giá trị rõ.
- Đặt một câu hỏi ngắn, đúng nhu cầu của nông dân.
- Để câu trả lời hiện đủ lâu cho người xem đọc.
- Không dùng câu trả lời có liều lượng thuốc cụ thể nếu chưa có nguồn chuyên môn và cơ chế an toàn phù hợp.

## 7. Phần testing nên bổ sung

> Đây là nội dung tham khảo. Kịch bản hiện gần như chưa dành thời lượng cho bằng chứng định lượng. Có thể dùng một bảng hoặc graphic ngắn.

| Phép thử | Cần nói rõ | Hình nên hiện |
|---|---|---|
| Benchmark AI | 120 ảnh, 10 lớp, 119 đúng, 1 sai; điều kiện và phiên bản model | Tóm tắt kết quả + ảnh Hispa bị nhầm thành Blast |
| Tốc độ xử lý | Thiết bị, model ONNX/GradCAM, số lượt đo | Log thời gian và trung vị/trung bình |
| Field test | Số mẫu lá thật, ai xác nhận đúng/sai | Bảng ngắn hoặc biểu đồ, 2–3 ảnh đại diện |
| Cảm biến | Thiết bị đối chiếu, số lần đo và sai số | Cảnh đo song song + bảng sai số |
| Mất mạng | Số lần thử, số bản ghi đồng bộ thành công | Log offline → sync |
| Độ ổn định | Số giờ chạy và lỗi đã gặp | Timeline chạy và sự cố |

## 8. Cách quay để video có chất lượng cao

> Các thông số dưới đây là gợi ý tham khảo từ AI.

### 8.1. Hình ảnh

- Chọn một chuẩn quay thống nhất: 25 fps hoặc 30 fps; không trộn tùy tiện.
- Nếu thiết bị hỗ trợ, quay 4K để có dư địa crop nhưng xuất video theo yêu cầu cuộc thi.
- Khóa cân bằng trắng và phơi sáng ở các cảnh quan trọng để màu không thay đổi giữa chừng.
- Mỗi hành động quan trọng quay đủ ba cỡ: toàn cảnh để thấy bối cảnh, trung cảnh để thấy người thao tác và cận cảnh để thấy bằng chứng.
- Không dùng zoom số; đưa máy gần hơn hoặc dùng tiêu cự phù hợp.
- Quay thêm 5 giây trước và sau mỗi hành động để dễ dựng.
- Flycam chỉ làm establishing shot; không để hình đẹp lấn át footage sản phẩm.

### 8.2. Âm thanh

- Ưu tiên micro cài áo cho lời trực tiếp; đồng thời thu một nguồn dự phòng.
- Kiểm tra tiếng gió ngoài ruộng và tiếng quạt hoặc thiết bị trước khi quay.
- Thu 20–30 giây âm thanh nền tại mỗi địa điểm để xử lý khi dựng.
- Nhạc phải thấp hơn giọng nói rõ rệt; không để nhạc cao trào che câu quan trọng.
- Không lồng voice quá nhanh để chạy theo thời lượng. Nên cắt chữ trước khi tăng tốc đọc.

### 8.3. Screen recording và graphic

- Screen record trực tiếp dashboard; không dùng camera quay màn hình cho toàn bộ demo.
- Phóng to đúng vùng cần xem, ẩn thông tin riêng tư và tắt thông báo cá nhân.
- Mỗi graphic chỉ truyền một ý; giữ trên màn hình đủ 3–5 giây.
- Subtitle tối đa hai dòng, tương phản cao, đúng chính tả và dùng cùng một font.
- Dùng màu nhất quán cho luồng input, xử lý và output/cảnh báo.

### 8.4. Continuity và độ tin cậy

- Thời gian trên dashboard, LCD, điện thoại và file log phải hợp lý với cùng một lần demo.
- Tên lớp bệnh và đơn vị đo phải thống nhất giữa lời nói, web và caption.
- Không dựng output của lần thử khác như thể là cùng một chuỗi liên tục.
- Chuẩn bị phương án backup: screen record, ảnh log và footage của một lần demo thành công trước đó.

## 9. Lời thoại mẫu cho các đoạn quan trọng

### 9.1. Mở đầu — 20–25 giây

> Đây là một hình ảnh lá lúa vừa được trạm AgriTech ghi nhận. Sau khi phân tích tại Raspberry Pi, hệ thống trả về tình trạng dự đoán, độ tin cậy và gửi kết quả tới người dùng. Nhưng trên thực tế, không phải dấu hiệu bất thường nào ngoài ruộng cũng được phát hiện kịp thời. Đó là vấn đề nhóm GREEN HORIZON muốn giải quyết.

### 9.2. Giới thiệu giải pháp — 30–35 giây

> AgriTech là trạm quan trắc AIoT đặt tại ruộng lúa. Camera ghi ảnh lá để AI phân loại tình trạng bệnh; cảm biến ghi nhận NPK, nhiệt độ và độ ẩm đất. Raspberry Pi xử lý dữ liệu tại trạm, sau đó kết quả được lưu và hiển thị qua LCD, web dashboard hoặc cảnh báo từ xa. Mục tiêu của hệ thống là giúp người nông dân có thêm dữ liệu để phát hiện bất thường và đưa ra quyết định kịp thời hơn.

### 9.3. Testing — 30–40 giây

> Nhóm không chỉ kiểm tra hệ thống bằng một vài hình ảnh minh họa. Trong bài test riêng gồm 120 ảnh, chia đều cho 10 lớp, phiên bản mô hình chạy trên Raspberry Pi phân loại đúng 119 ảnh và sai một ảnh Hispa thành Blast. Kết quả này chỉ phản ánh điều kiện của tập kiểm thử trên; vì vậy nhóm tiếp tục kiểm tra với ảnh thực địa và nhiều điều kiện ánh sáng khác nhau.

### 9.4. Giới hạn và kết — 35–45 giây

> Phiên bản hiện tại đã thực hiện được chuỗi quan sát, phân loại, ghi dữ liệu và cảnh báo. Tuy nhiên, nhóm vẫn cần mở rộng kiểm thử ngoài ruộng, đối chiếu cảm biến với thiết bị chuẩn và tối ưu độ bền của trạm. AgriTech không thay thế kinh nghiệm của người nông dân hay ý kiến chuyên gia; hệ thống hướng tới trở thành một công cụ cung cấp thêm dữ liệu để họ chủ động hơn trước những thay đổi trên cánh đồng.
