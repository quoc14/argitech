# PHẢN HỒI & ĐỊNH HƯỚNG HOÀN THIỆN VIDEO + TÀI LIỆU

## Gửi đội GREEN HORIZON — dự án AgriTech AIoT

Gửi các em,

Trước hết anh thấy: sản phẩm của các em **đã chạy được thật**, web cũng hoạt động. Đây là nền tảng rất tốt, việc còn lại **không phải làm lại sản phẩm**, mà là **quay và viết sao cho ban giám khảo tin rằng nó chạy thật và có ích**.

Một điều anh muốn các em nhớ suốt: **cứ thành thật.** Dự án của mình là **bước đầu** — nghiên cứu và đưa ra một cách giải quyết, giúp người nông dân tiếp cận công nghệ. Nó chưa phải sản phẩm hoàn chỉnh để bán, và điều đó **hoàn toàn bình thường**. Ban giám khảo rất thích một nhóm biết rõ mình làm được gì, chưa làm được gì, và sẽ làm gì tiếp. Nói thật làm dự án mạnh hơn, chứ không yếu đi.

---

## 1. Ban giám khảo quan tâm điều gì nhất?

Có 3 điều, theo đúng thứ tự:

1. **Sản phẩm có chạy thật không?** → Cái này các em đã có. Chỉ cần **quay cho thấy nó đang chạy**.
2. **Có bằng chứng, số liệu chứng minh không?** → Đây là phần cần đầu tư nhiều nhất từ giờ.
3. **Video và tài liệu có rõ ràng không?** → Trình bày đẹp là quan trọng, nhưng đứng **sau** 2 điều trên.

**Nguyên tắc vàng:** ĐỪNG CHỈ NÓI — HÃY CHO XEM.

- Đừng nói "sản phẩm hoạt động tốt" → **cho xem cảnh nó đang chạy + con số**.
- Đừng nói "vấn đề nghiêm trọng" → **cho xem hình thật + số liệu**.
- Đừng nói "người dùng thấy hữu ích" → **cho xem nông dân dùng thử + họ nói gì**.

**Một lưu ý riêng cho dự án của mình:** Điều đáng nói là: **AI giúp giải quyết việc mà cách làm cũ chưa làm tốt** — phát hiện bệnh sớm ngay tại ruộng, và chạy được cả khi mất mạng.

---

## 2. Trả lời câu hỏi của các em

### 2.1. Điểm yếu ban giám khảo có thể "bắt bài" — và cách xử lý

Hầu hết cách xử lý **không phải sửa sản phẩm**, mà là **nói cho đúng và có phương án**.

| Ban giám khảo có thể hỏi                                  | Cách các em xử lý                                                                                                                                                                                                                                                                                                                                                                                                                   |
| --------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **"AI nhận diện dựa vào ảnh — ảnh mờ, chụp xa thì sao?"** | Nói rõ: camera đặt cố định, tự chụp gần theo lịch nên ảnh đủ rõ. Ngoài ra hệ thống có cơ chế: **khi AI không chắc chắn (độ tin cậy dưới 50%) thì yêu cầu chụp lại**, không đoán bừa. Còn ảnh mờ/xa thì ghi vào phần "hạn chế + hướng phát triển" (nâng cấp camera zoom sau này).                                                                                                                                                    |
| **"Con số chính xác của AI là bao nhiêu?"**               | Chọn **một** con số và nói kèm điều kiện, ví dụ: _"Khi test 120 ảnh trên máy tại trạm, đúng 119 ảnh, tức 99,2%, với ảnh rõ."_ Nếu được, cho xem thêm **AI đúng/sai ở từng loại bệnh** (loại nào hay nhầm) — càng thành thật càng đáng tin.                                                                                                                                                                                          |
| **"Cảm biến đo có chính xác không?"**                     | **Đừng nói "cảm biến chính xác, sai số rất thấp"** (vì mình chưa có máy chuẩn để đối chiếu). Hãy nói đúng: _"Với linh kiện, sơ đồ nối và code này, thiết bị đọc ra chỉ số đất **ổn định và hợp lý**; trước khi lắp, tụi em đã kiểm tra kết nối bằng phần mềm mô phỏng. Việc đo đối chiếu với máy chuẩn là bước tiếp theo."_ Có thể chứng minh bằng cách **đo nhiều lần cùng một chỗ → thấy kết quả ổn định, không nhảy lung tung**. |
| **"Nói chạy offline mà sao vẫn cần mạng?"**               | Tách rõ 2 phần: **phần chẩn đoán bệnh chạy ngay tại trạm, không cần mạng**; còn chatbot và đồng bộ lên web là phần thêm khi có mạng.                                                                                                                                                                                                                                                                                                |
| **"Sản phẩm tự động canh tác à?"**                        | Nói rõ: hệ thống **theo dõi → phát hiện bệnh → cảnh báo → tư vấn**; **chưa** tự phun thuốc/tưới/bón.                                                                                                                                                                                                                                                                                                                                |
| **"Nhân rộng cả nước được không?"**                       | Nói thật: mình đang chạy ở **một trạm** (bước đầu). Việc đặt nhiều camera, camera zoom, giám sát từ xa là **hướng phát triển**, chưa làm.                                                                                                                                                                                                                                                                                           |
| **"Em phụ trách phần nào?"** (hỏi từng bạn)               | **Mỗi bạn phải tự giải thích được phần mình làm** mà không cần anh/thầy nhắc.                                                                                                                                                                                                                                                                                                                                                       |

### 2.2. Cách cân bằng dữ liệu & giúp AI nhận diện chính xác hơn

**Làm được ngay (không cần train lại):**

- **Đếm số ảnh mỗi loại bệnh** → xem loại nào ít ảnh (bị "lép vế").
- **Xem AI hay nhầm cặp bệnh nào với nhau** (ví dụ Hispa ↔ Blast) để biết loại nào yếu.
- Báo cáo độ chính xác **từng loại bệnh**, không chỉ một con số chung.
- Thêm một bước **lọc ảnh mờ**: ảnh nào quá mờ thì bỏ, chỉ cho AI nhận diện ảnh rõ.

**Nếu còn thời gian train lại mô hình:**

- **Tạo thêm ảnh cho loại ít ảnh** bằng cách xoay, lật, đổi sáng tối, cắt cúp. Đặc biệt nên **thêm cả ảnh làm mờ nhẹ và ảnh độ phân giải thấp** để AI quen với ảnh chụp xa/mờ ngoài ruộng — chính là điểm yếu đang lo.
- Cho mô hình **"ưu tiên học" các loại bệnh ít ảnh** hơn (đặt trọng số cao hơn khi huấn luyện).
- **Chụp bổ sung ảnh thật ngoài ruộng** cho những loại hay nhầm.

**Nếu không kịp làm hết:** cứ **viết những cách này vào tài liệu như phần "phương pháp và hướng phát triển"**. Ban giám khảo đánh giá cao việc các em **biết cách làm**, kể cả khi thời gian ngắn chưa làm xong hết.

> Lời khuyên: thời gian còn ít, ưu tiên nhóm "làm được ngay". Phần train lại làm tới đâu hay tới đó.

### 2.3. Phần tài liệu cần có những gì?

Cuộc thi yêu cầu nộp **một tài liệu (Word hoặc PowerPoint)** mô tả và hướng dẫn sản phẩm. **Không bắt buộc phải theo đúng bao nhiêu chương** — nên các em cứ trình bày sao cho **người đọc hiểu và tin** là được.

Hãy nhớ: **video để người xem HIỂU nhanh; tài liệu để người đọc KIỂM CHỨNG** những gì video nói.

Một tài liệu tốt nên có (chọn lọc theo dự án của mình):

1. **Trang bìa** — tên dự án, đội, trường, thành viên.
2. **Tóm tắt 1 trang** — vấn đề · người dùng · giải pháp · công nghệ · kết quả nổi bật · tác động. (Đọc trang này là hiểu 80% dự án.)
3. **Vấn đề** — bối cảnh ở Đồng Tháp, ai gặp, nghiêm trọng thế nào, có số liệu/khảo sát.
4. **Cách làm hiện tại & khoảng trống** — hiện người ta xử lý ra sao, còn thiếu gì, mình lấp chỗ nào.
5. **Giải pháp & cấu tạo** — sơ đồ hệ thống, phần cứng, phần mềm, AI, luồng hoạt động.
6. **Quá trình làm sản phẩm** — dòng thời gian có ảnh thật (từ ý tưởng → bản đầu → chỉnh sửa → bản hiện tại).
7. **Cách kiểm thử** — test cái gì, điều kiện nào, bao nhiêu lần, đo bằng gì.
8. **Kết quả** — bảng, biểu đồ, ảnh. **Ghi rõ cái nào đã đo được, cái nào mới là mong đợi.**
9. **Người dùng thử & phản hồi** — ai thử, họ nói gì, mình sửa gì.
10. **Các phiên bản cải tiến** — bảng: bản nào, gặp lỗi gì, sửa gì, kết quả.
11. **Điểm mới/sáng tạo** — so với cách hiện có, mình khác ở đâu và vì sao điều đó quan trọng.
12. **Tác động** — giúp được ai, tiết kiệm/giảm được gì (ghi rõ cái nào là kỳ vọng).
13. **Chi phí** — bảng giá linh kiện, tổng tiền.
14. **Hạn chế & bước tiếp theo** — thành thật nêu cái chưa làm được + dự định khắc phục.
15. **Đóng góp của từng thành viên** — ai làm gì, có minh chứng.
16. **Hướng dẫn sử dụng** (nếu muốn gộp vào): thành phần bộ sản phẩm · cách lắp đặt · cấu hình lần đầu · dùng hằng ngày (đọc màn hình, xem web, hiểu 4 trạng thái, khi nhận tin cảnh báo thì làm gì, hỏi chatbot) · cách đọc kết quả AI · bảo trì · xử lý sự cố · câu hỏi thường gặp.

**Nên có hình:** sơ đồ vấn đề, biểu đồ khảo sát, ảnh ngoài ruộng, bảng so sánh, sơ đồ hệ thống, ảnh sản phẩm, dòng thời gian, bảng kết quả, bảng các phiên bản, bảng chi phí.

---

## 3. Cách nói cho đúng (thành thật mà vẫn mạnh)

| Đừng nói (dễ bị bắt)                      | Hãy nói (đúng & vững)                                                                                                                                  |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| "Cảm biến chính xác, sai số rất thấp"     | "Thiết bị đọc chỉ số đất **ổn định, hợp lý**; đã kiểm tra kết nối bằng phần mềm mô phỏng trước khi lắp; đo đối chiếu máy chuẩn là **bước tiếp theo**." |
| "AI chính xác 99,2% trong mọi trường hợp" | "Với ảnh rõ, chụp gần: đúng **119/120** ảnh test. Ảnh mờ/xa thì giảm, nên có cơ chế yêu cầu chụp lại."                                                 |
| "Chúng em dùng AI, IoT hiện đại"          | "Cách làm cũ khó phát hiện bệnh sớm tại chỗ; **AI chạy ngay tại trạm giúp** phát hiện sớm, kể cả khi mất mạng."                                        |
| "Hệ thống tự động canh tác"               | "Hệ thống **theo dõi – phát hiện – cảnh báo – tư vấn**; chưa tự phun/tưới/bón."                                                                        |
| "Có thể nhân rộng cả nước"                | "Đang chạy ở **một trạm**; hướng phát triển là nhiều camera, camera zoom, giám sát từ xa."                                                             |
| "Sản phẩm đã hoàn thiện"                  | "Đây là **bước đầu** nghiên cứu và đề xuất phương pháp; triển khai thật cần thêm thời gian thử nghiệm."                                                |

Những câu này nên xuất hiện ở phần **hạn chế + hướng phát triển** của video và tài liệu — đó thường là chỗ khiến ban giám khảo tin các em là người làm nghiêm túc.

---

## 4. Kiểm kê: đang có gì, còn thiếu gì?

Bảng này để cả nhóm cùng nhìn. Ký hiệu: **✅ đã có** · **🟡 có một phần, cần bổ sung** · **❌ chưa có**.
Các em điền cột **Ai làm / Hạn** cho từng dòng.

### Nhóm 1 — Bằng chứng về VẤN ĐỀ

| Cần có                        | Tình trạng | Việc cần làm                                 | Ai / Hạn |
| ----------------------------- | ---------- | -------------------------------------------- | -------- |
| Mô tả vấn đề rõ ràng          | ✅         | Thu hẹp về Đồng Tháp: ai gặp, ở đâu, mức nào |          |
| Số liệu thiệt hại do bệnh lúa | ❌         | Tìm 1–2 con số có nguồn đáng tin             |          |
| Khảo sát nông dân (có số %)   | ❌         | Hỏi 30–50 người → ra tỉ lệ %                 |          |
| Hình/clip ngoài ruộng         | 🟡         | Quay cảnh ruộng + lá bệnh thật               |          |

### Nhóm 2 — Bằng chứng về NGƯỜI DÙNG (đang yếu nhất)

| Cần có                       | Tình trạng | Việc cần làm                                  | Ai / Hạn |
| ---------------------------- | ---------- | --------------------------------------------- | -------- |
| Biết rõ người dùng là ai     | ✅         | —                                             |          |
| Đã hỏi chuyện nông dân thật  | ❌         | Phỏng vấn 2–3 người, quay clip ngắn 5–10 giây |          |
| Nông dân đã **thử** sản phẩm | ❌         | Cho ít nhất 1 nông dân dùng thử               |          |
| Sản phẩm thay đổi nhờ góp ý  | ❌         | Ghi lại họ góp ý gì → mình chỉnh gì           |          |

### Nhóm 3 — Bằng chứng SẢN PHẨM CHẠY (đã có, cần QUAY lại)

| Cần có                                 | Tình trạng | Việc cần làm                            | Ai / Hạn |
| -------------------------------------- | ---------- | --------------------------------------- | -------- |
| Sản phẩm chạy được                     | ✅         | Giữ nguyên                              |          |
| Cảnh camera → AI → ra kết quả          | 🟡         | Quay một mạch, không cắt                |          |
| Ảnh AI tô sáng vùng bệnh (GradCAM)     | 🟡         | Chụp 3–5 cặp ảnh đẹp                    |          |
| Trang web đang chạy                    | 🟡         | Quay màn hình bấm qua các trang         |          |
| Tin nhắn cảnh báo về điện thoại        | 🟡         | Quay cảnh tin nhắn hiện trên điện thoại |          |
| Mất mạng vẫn chạy → có mạng tự đồng bộ | 🟡         | Quay cảnh rút mạng → vẫn chạy → nối lại |          |

### Nhóm 4 — Bằng chứng KIỂM THỬ (có số)

| Cần có                                 | Tình trạng | Việc cần làm                                   | Ai / Hạn |
| -------------------------------------- | ---------- | ---------------------------------------------- | -------- |
| Test AI 119/120 ảnh                    | ✅         | Chạy lại và quay/chụp màn hình                 |          |
| Tốc độ nhận diện (khoảng 0,1 giây/ảnh) | 🟡         | Cho hiện số lên màn hình khi chạy              |          |
| Độ ổn định của cảm biến                | ❌         | Đo nhiều lần cùng chỗ → cho thấy ổn định       |          |
| Thử ngoài ruộng có ghi số              | 🟡         | Chụp 20–30 lá thật → so kết quả AI với thực tế |          |
| Chạy liên tục bao lâu không lỗi        | ❌         | Ghi lại số giờ chạy / số lần lỗi               |          |

> Nhớ: **một lần demo thành công chưa phải là đã kiểm thử.** Cần thử nhiều lần, nhiều tình huống, rồi tính tỉ lệ.

### Nhóm 5 — SỐ LIỆU / DỮ LIỆU

| Cần có                            | Tình trạng | Việc cần làm                                           | Ai / Hạn |
| --------------------------------- | ---------- | ------------------------------------------------------ | -------- |
| Bộ dữ liệu 10.407 ảnh, 10 loại    | ✅         | Ghi rõ lấy từ đâu                                      |          |
| Con số % chính xác chính thức     | 🟡         | Chốt 1 con số + điều kiện, thêm số theo từng loại bệnh |          |
| Xem AI hay nhầm loại nào          | ❌         | Lập bảng đúng/sai từng loại                            |          |
| Biểu đồ chỉ số đất theo thời gian | 🟡         | Xuất 1 biểu đồ gọn, mỗi biểu đồ nói 1 ý                |          |

### Nhóm 6 — QUÁ TRÌNH CẢI TIẾN

| Cần có                         | Tình trạng | Việc cần làm                                     | Ai / Hạn |
| ------------------------------ | ---------- | ------------------------------------------------ | -------- |
| Nhật ký các bản: bản 1 → 2 → 3 | ❌         | Nhớ lại: từng gặp lỗi gì, sửa gì, kết quả ra sao |          |
| Ảnh quá trình lắp ráp          | 🟡         | Gom lại ảnh cũ theo thứ tự thời gian             |          |

### Nhóm 7 — TÁC ĐỘNG

| Cần có                          | Tình trạng | Việc cần làm                                 | Ai / Hạn |
| ------------------------------- | ---------- | -------------------------------------------- | -------- |
| Bảng chi phí (5.658.000đ)       | ✅         | —                                            |          |
| So sánh giá với sản phẩm khác   | 🟡         | Tìm giá thật của ít nhất 1 sản phẩm tương tự |          |
| Lợi ích (giảm phân/thuốc…)      | 🟡         | Ghi rõ đây là **mong đợi**, kèm cách tính    |          |
| Nông dân sẵn sàng chi bao nhiêu | ❌         | Lấy từ khảo sát                              |          |

**Về việc đo lường, cố gắng có 3 mốc:**

- **Trước** (khi chưa có sản phẩm): bao nhiêu % nông dân phát hiện bệnh muộn, bón phân theo cảm tính…
- **Trong** (khi chạy sản phẩm): độ chính xác AI, tốc độ, độ ổn định cảm biến, chạy được khi mất mạng…
- **Sau** (đánh giá): nông dân thử thấy sao, sẵn sàng dùng không, mình sửa gì nhờ góp ý.

---

## 5. Việc cần làm — theo thứ tự ưu tiên (đến ngày 15/9)

### ① Làm trước — dễ và mạnh nhất (chủ yếu là QUAY lại cái đã chạy)

- [ ] Quay cảnh **camera → AI → tô vùng bệnh → màn hình → tin nhắn cảnh báo** (quay một mạch).
- [ ] Quay cảnh **rút mạng vẫn chạy → nối mạng lại tự đồng bộ** (đây là cảnh ấn tượng nhất).
- [ ] Quay **màn hình trang web** đang bấm (ít nhất 4 trang + chatbot).
- [ ] Chốt **con số chính xác của AI** và lập bảng đúng/sai từng loại bệnh.

### ② Làm thêm một chút

- [ ] Thêm bước **lọc ảnh mờ** và giải thích cơ chế "AI không chắc thì yêu cầu chụp lại".
- [ ] **Đo cảm biến nhiều lần** cùng một chỗ để cho thấy kết quả ổn định.
- [ ] Chụp **bộ ảnh AI tô vùng bệnh** cho đẹp.
- [ ] Viết **bảng các bản cải tiến** (bản 1 → 2 → 3).

### ③ Ra ruộng / gặp nông dân (nếu có thể)

- [ ] Cho **ít nhất 1 nông dân dùng thử** + quay **clip họ nói cảm nhận**.
- [ ] **Khảo sát nhanh** vài nông dân để có số liệu về vấn đề.

### ④ Làm tài liệu

- [ ] Hoàn thiện **tài liệu Word/PowerPoint** (theo gợi ý ở mục 2.3).
- [ ] Viết rõ phần **hạn chế + hướng phát triển**.
- [ ] Chèn đủ hình (sơ đồ, biểu đồ, ảnh thật).

---

## 6. Lời cuối

Dự án của các em **tốt và thật**. Điều thuyết phục ban giám khảo là: **cho họ thấy sản phẩm chạy thật + thành thật về giới hạn + có hướng đi tiếp rõ ràng**.

Cố lên nhé!
