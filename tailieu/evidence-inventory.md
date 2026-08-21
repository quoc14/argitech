# EVIDENCE INVENTORY — AgriTech AIoT | GREEN HORIZON

> **Mục đích:** kiểm kê *đang có bằng chứng gì / còn thiếu gì* theo 7 nhóm (vấn đề · người dùng · demo · test · số liệu · iteration · tác động), để mentor làm việc với đội và giao đúng việc.
>
> **Khung tham chiếu (Samsung NZ):** một dự án mạnh đi theo chuỗi **STAKEHOLDER → PROTOTYPE → TESTING → EVALUATION**, và **xác định trước các phép đo (trước / trong / sau)** cùng **kết quả hữu hình** sẽ tạo ra. Tài liệu này gắn từng bằng chứng vào đúng mắt xích đó.
>
> **Ký hiệu trạng thái:** ✅ Đủ, có thể đưa vào video/tài liệu ngay · 🟡 Có một phần / cần bổ sung số hoặc footage · ❌ Chưa có.
> **Cập nhật lần cuối:** 19/8/2026 (điền lại sau mỗi buổi họp).

---

## 0. Bản đồ nhanh: bằng chứng gắn vào chuỗi Samsung NZ

| Mắt xích | Bằng chứng cốt lõi | Tình trạng chung |
|---|---|---|
| **STAKEHOLDER** (người dùng tham gia xuyên suốt) | Khảo sát, phỏng vấn, nông dân thử & phản hồi | 🟡→❌ **yếu nhất** |
| **PROTOTYPE** (sản phẩm chạy được) | Trạm thật, camera→AI→kết quả, dashboard, offline | ✅ có sản phẩm — 🟡 cần **quay lại thành footage** |
| **TESTING** (kiểm thử có số) | Benchmark AI, latency, hiệu chuẩn cảm biến, field test | 🟡 có AI benchmark, thiếu field stats & sensor error |
| **EVALUATION** (đánh giá + đo tác động) | Đo trước/sau, phản hồi người dùng, KPI | ❌ chủ yếu là kỳ vọng |

> Nhận định: **PROTOTYPE mạnh, nhưng STAKEHOLDER và EVALUATION đang là chỗ hổng** — đúng khung Samsung NZ đánh giá cao.

---

## 1. BẰNG CHỨNG VỀ VẤN ĐỀ

| Bằng chứng | Trạng thái | Đang có ở đâu | Còn thiếu → việc cần làm | Ai / Hạn |
|---|---|---|---|---|
| Mô tả vấn đề (phát hiện bệnh muộn, bón phân cảm tính) | ✅ | `agritech.md` §2 | — | — |
| Số liệu thiệt hại do bệnh lúa (nguồn tin cậy) | ❌ | — | Tra 1–2 số có nguồn (viện/sở NN, bài báo) | |
| Khảo sát nông dân địa phương (định lượng) | ❌ | — | Chạy khảo sát N≥30–50 (form đã có ở `buoi1/1-...`) | |
| Quan sát/ảnh thực địa vấn đề | 🟡 | (ảnh rời?) | Quay B-roll ruộng + lá bệnh thật | |

---

## 2. BẰNG CHỨNG VỀ NGƯỜI DÙNG (STAKEHOLDER)

| Bằng chứng | Trạng thái | Đang có ở đâu | Còn thiếu → việc cần làm | Ai / Hạn |
|---|---|---|---|---|
| Chân dung người dùng (nông dân, HTX…) | ✅ | `agritech.md` §4 | — | — |
| Đã nói chuyện/phỏng vấn nông dân thật | ❌ | — | Phỏng vấn 2–3 người, quay clip 5–10s | |
| Nông dân đã **thử** sản phẩm | ❌ | — | Cho ≥1 nông dân thử tại ruộng | |
| Phản hồi người dùng làm sản phẩm **thay đổi** | ❌ | — | Ghi lại feedback → điều chỉnh gì | |

> ⭐ Đây là nhóm Samsung NZ chấm rất cao (stakeholder tham gia **xuyên suốt**, không chỉ khảo sát 1 lần đầu). Ưu tiên lấp.

---

## 3. BẰNG CHỨNG DEMO / PROTOTYPE HOẠT ĐỘNG

| Bằng chứng | Trạng thái | Đang có ở đâu | Còn thiếu → việc cần làm | Ai / Hạn |
|---|---|---|---|---|
| Prototype vật lý chạy được | ✅ | Sản phẩm | Giữ nguyên | — |
| Chuỗi camera → AI → kết quả (live) | 🟡 | Chạy được | **Quay** thành footage liên hoàn (`demo-choreography.md` Demo 1) | |
| GradCAM heatmap | 🟡 | Có | Quay 3–5 cặp ảnh gốc/heatmap đẹp | |
| Web dashboard chạy | ✅→🟡 | Web app hoạt động | **Screen-record** ≥4 màn (Demo 2) | |
| Cảnh báo SMS/gọi | 🟡 | SIM7600 có | Quay tin SMS thật trên điện thoại | |
| Offline → SQLite → sync | 🟡 | Cơ chế có | Diễn live rút mạng (Demo 3) | |
| LCD hiển thị tại trạm | 🟡 | Có | Quay cận LCD | |
| Chatbot có ngữ cảnh ruộng | 🟡 | Có | Screen-record 1 lượt hỏi–đáp | |

> Nhóm này **đã tồn tại trong sản phẩm** — việc còn lại chủ yếu là **QUAY LẠI** cho giám khảo nhìn thấy (không phải làm mới).

---

## 4. BẰNG CHỨNG TESTING (kiểm thử có số)

| Bằng chứng | Trạng thái | Đang có ở đâu | Còn thiếu → việc cần làm | Ai / Hạn |
|---|---|---|---|---|
| Benchmark AI trên Pi (120 ảnh, 119/120) | ✅ | `agritech.md` §22 | Tái hiện + quay/log; chốt cách trình bày | |
| Tốc độ nhận dạng (80–120ms ONNX) | 🟡 | Hồ sơ | Tái hiện bằng log hiện trên màn hình | |
| Hiệu chuẩn cảm biến (sai số %) | ❌ | "sai số thấp" nhưng không số | Đo vs thiết bị chuẩn → % sai số, số lần đo | |
| Field test có thống kê | 🟡 | Mô tả định tính §23 | Bảng 20–30 lượt chụp lá thật → AI vs thực tế → % | |
| Độ ổn định/uptime ngoài ruộng | ❌ | — | Ghi số giờ chạy liên tục / lỗi gặp | |
| Test khôi phục offline | 🟡 | Cơ chế có | Ghi tỉ lệ sync thành công sau mất mạng | |

---

## 5. BẰNG CHỨNG SỐ LIỆU / DỮ LIỆU

| Bằng chứng | Trạng thái | Đang có ở đâu | Còn thiếu → việc cần làm | Ai / Hạn |
|---|---|---|---|---|
| Dataset 10.407 ảnh / 10 lớp / 80-10-10 | ✅ | `agritech.md` §7 | Mô tả nguồn (PaddyDoctor + thực địa) | |
| Con số accuracy nêu bật | 🟡 | 3 số (98,14 / 94,20 / 99,20%) | **Chốt 1 con số + ngữ cảnh** (đặt câu hỏi cho đội) | |
| Raw test data 120 ảnh | 🟡 | (có?) | Xuất bảng cho Phụ lục | |
| Số liệu cảm biến theo thời gian | 🟡 | Trong DB | Xuất 1 biểu đồ biến thiên đẹp | |

---

## 6. BẰNG CHỨNG ITERATION (thử → sai → sửa)

| Bằng chứng | Trạng thái | Đang có ở đâu | Còn thiếu → việc cần làm | Ai / Hạn |
|---|---|---|---|---|
| Nhật ký V1 → V2 → V3 | ❌ | — | Moi từ đội: lỗi từng gặp, sửa gì, kết quả | |
| Ảnh quá trình chế tạo/lắp đặt | 🟡 | (ảnh cũ?) | Gom ảnh cũ theo mốc thời gian | |
| Vấn đề kỹ thuật & cách khắc phục | ✅ | `agritech.md` §27 | Chuyển thành bảng iteration | |

> Nhóm này Samsung quốc tế đánh giá mạnh (iteration–testing–feedback–evaluation). Chỉ cần **kể lại đúng** hành trình đã có.

---

## 7. BẰNG CHỨNG TÁC ĐỘNG (EVALUATION)

| Bằng chứng | Trạng thái | Đang có ở đâu | Còn thiếu → việc cần làm | Ai / Hạn |
|---|---|---|---|---|
| Chi phí prototype (BOM) | ✅ | `agritech.md` §24 | — | — |
| So sánh chi phí vs giải pháp khác | 🟡 | Định tính | Giá thật ≥1 đối thủ | |
| Tác động kinh tế/môi trường | ❌(đo)/🟡(kỳ vọng) | §25 | Ghi rõ **Projected**; nêu cơ sở tính | |
| Đo trước/sau thực tế | ❌ | — | Xem "Kế hoạch đo" bên dưới | |
| Mức sẵn sàng chi trả của nông dân | ❌ | — | Lấy từ khảo sát (câu E2) | |

---

## 8. KẾ HOẠCH ĐO — TRƯỚC / TRONG / SAU (theo yêu cầu project-plan Samsung NZ)

Xác định phép đo **trước khi làm**, để có baseline mà so — đây là điểm project-plan mẫu yêu cầu.

### 8.1. Đo TRƯỚC (Baseline — hiện trạng khi chưa có sản phẩm)
| Chỉ số | Cách đo | Mục tiêu con số |
|---|---|---|
| % nông dân phát hiện bệnh muộn | Khảo sát (câu B3) | vd "X% thường/thỉnh thoảng phát hiện muộn" |
| % nông dân bón phân theo cảm tính | Khảo sát (câu C1) | vd "Y% không đo đất trước khi bón" |
| Thời gian kiểm tra ruộng thủ công | Hỏi nông dân (phút/lần, lần/tuần) | baseline giờ công |
| Rào cản dùng công nghệ hiện có | Khảo sát (câu D2) | % theo từng rào cản |

### 8.2. Đo TRONG (Prototype testing — sản phẩm vận hành thế nào)
| Chỉ số | Cách đo | Kết quả hiện có |
|---|---|---|
| Độ chính xác nhận dạng bệnh | Test 120 ảnh trên Pi | 119/120 = 99,2% ⚠️[chốt] |
| Tốc độ nhận dạng | Log thời gian/ảnh | 80–120ms (ONNX) |
| Sai số cảm biến | Đối chiếu thiết bị chuẩn | ❌ cần đo |
| Tỉ lệ nhận diện đúng ngoài ruộng | Field test log 20–30 mẫu | ❌ cần lập bảng |
| Khả năng chạy khi mất mạng | Test rút mạng + đếm lần sync đúng | 🟡 cần ghi số |
| Độ ổn định | Số giờ chạy liên tục / số lần treo | ❌ cần ghi |

### 8.3. Đo SAU (Evaluation — đánh giá & tác động)
| Chỉ số | Cách đo | Ghi chú |
|---|---|---|
| Phản hồi người dùng | Nông dân thử → thang điểm + nhận xét | ❌ cần làm |
| Mức sẵn sàng sử dụng / chi trả | Khảo sát (E1, E2) | ❌ cần làm |
| Thay đổi sản phẩm nhờ feedback | Ghi trước/sau | ❌ cần làm |
| Tác động dự phóng (giảm phân/thuốc, tăng năng suất) | **Projected** — nêu cơ sở, KHÔNG gọi là kết quả đã đạt | ⚠️ ghi rõ nhãn |

---

## 9. KẾT QUẢ HỮU HÌNH có thể tạo ra (Tangible outputs)

Những "vật phẩm" cụ thể dự án sẽ nộp/trình được — đây là thứ project-plan Samsung NZ muốn thấy liệt kê trước:

- [x] Trạm prototype vật lý hoạt động
- [x] Bộ dữ liệu 10.407 ảnh / 10 lớp
- [x] Web dashboard đang chạy
- [x] Bảng chi phí BOM (5,658tr)
- [ ] Báo cáo benchmark AI (bảng 120 ảnh + biểu đồ)
- [ ] Field test log có thống kê
- [ ] Báo cáo hiệu chuẩn cảm biến (% sai số)
- [ ] Báo cáo khảo sát nông dân (biểu đồ %)
- [ ] Clip phỏng vấn / nông dân thử
- [ ] Bộ ảnh GradCAM (gốc ↔ heatmap)
- [ ] Video demo 3 tình huống (liên hoàn / dashboard / offline)
- [ ] Bảng iteration V1→V2→V3
- [ ] Bảng so sánh giải pháp (có giá thật)
- [ ] Video dự thi + Tài liệu 15 phần

---

## 10. ƯU TIÊN LẤP TRƯỚC KHI QUAY (theo deadline 15/9)

Xếp theo tỉ lệ "tác động lớn / công ít":

1. **Quay lại cái đã chạy** (Demo 1/2/3 + GradCAM + SMS) — công ít, bằng chứng mạnh nhất. 🟡→✅
2. **Chốt con số accuracy** + tái hiện log — 1 buổi. 🟡→✅
3. **Khảo sát nông dân** (ra % vấn đề + người dùng) — lấp mắt xích STAKEHOLDER. ❌→✅
4. **Field test log + hiệu chuẩn cảm biến** (số cụ thể) — lấp TESTING. ❌/🟡→✅
5. **Nông dân thử + clip phỏng vấn** — lấp STAKEHOLDER/EVALUATION. ❌→🟡
6. **Bảng iteration** — kể lại hành trình đã có. ❌→✅

> Nguyên tắc: mục 1–2 gần như chỉ tốn công **quay & trình bày** (sản phẩm đã có) → làm trước. Mục 3–5 cần ra thực địa → xếp lịch sớm vì phụ thuộc thời tiết/nông dân.

---

## Cách dùng tài liệu này trong buổi họp
1. Cùng đội đi từng bảng, cập nhật cột **Trạng thái** cho đúng thực tế (nhiều ô có thể đã ✅ mà tôi chưa biết).
2. Điền cột **Ai / Hạn** cho mọi dòng ❌ và 🟡.
3. Dòng nào không kịp trước 15/9 → quyết định: bỏ khỏi claim, hay ghi là **Next step** (đừng biến kỳ vọng thành kết quả).
