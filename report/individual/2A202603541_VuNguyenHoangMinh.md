# Báo cáo cá nhân — 2A202603541_VuNguyenHoangMinh

## 1. Thông tin học viên

- Họ tên: Vũ Nguyễn Hoàng Minh
- MSSV: 2A202603541
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomABC
- Link repo nhóm: https://github.com/LufkyMama/K5-L3A-DAY02-NhomABC-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi bắt đầu một tuần học, tôi muốn thấy mọi deadline (LMS, email, nhóm chat) ở một chỗ, để không lỡ hạn nộp | Học viên | Mỗi tuần mất ~15 phút lục 3 nơi; tuần trước suýt trễ 1 bài vì deadline chỉ nằm trong tin nhắn nhóm |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi phải đọc một bài báo/tài liệu 10–20 trang trước buổi học, tôi muốn nắm ý chính và những phần cần đọc kỹ, để vào lớp hiểu kịp nội dung | Học viên | ~60 phút/bài, 2–3 bài/tuần (tự bấm giờ) |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi cần tìm lại một slide/ghi chú đã học tuần trước, tôi muốn tìm ra đúng file ngay, để không phải mở từng thư mục | Học viên | 10 phút/lần, 3–4 lần/tuần; tài liệu nằm ở Drive, LMS, Zalo |
| 4 | Tốn thời gian | Khi làm xong lab, tôi muốn điền báo cáo theo đúng mẫu mà không phải chép lại kết quả nhiều nơi, để nộp đúng hạn | Học viên | ~45 phút/lab, mỗi lab 1 lần |
| 5 | Pain từ người khác | Khi làm bài nhóm, các bạn muốn biết ai đang làm phần nào và đã xong chưa, để không làm trùng hoặc chờ nhau | Cả nhóm 3–4 người | Lab trước 2 người làm trùng 1 phần (~30 phút mỗi người lãng phí) |
| 6 | Tốn thời gian | Khi cài môi trường cho bài mới, tôi muốn chạy được ngay, để không mất thời gian sửa lỗi cài đặt | Học viên | ~30 phút/lần, khoảng 1 lần/2 tuần |
| 7 | Lặp lại | Khi ôn thi, tôi muốn gom ghi chú rải rác thành một bản ôn tập, để ôn có hệ thống | Học viên | ~2 giờ/môn mỗi kỳ |
| 8 | Pain từ người khác | Khi nhóm trưởng nhận bài của nhiều người, họ muốn bài có format thống nhất, để ghép nhanh | Nhóm trưởng | ~20 phút/lần chỉnh format, mỗi lần nộp nhóm |

**Nếu có dùng AI để gợi ý thêm:** AI gợi ý thêm ý #7 (gom ghi chú ôn thi) và #8 (thống nhất format bài nhóm) — giữ vì có tần suất và người chịu ảnh hưởng rõ. Bỏ ý "trợ lý học tập toàn diện" vì quá rộng, không có quy trình cụ thể để vẽ.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Chuẩn bị bài đọc trước buổi học (#2) | Actor rõ, quy trình 5 bước, baseline đo được (60 phút/bài) | "Hiểu đủ" đo thế nào? |
| 2 | Deadline rải rác nhiều nơi (#1) | Lặp lại hằng tuần, pain thật (suýt trễ hạn) | Có thể chỉ cần lịch, không cần gì thêm |
| 3 | Tìm lại tài liệu cũ (#3) | Nhiều bạn gặp, tần suất cao | Dữ liệu ở nhiều nền tảng, khó truy cập, phạm vi dễ phình |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi phải đọc một bài tài liệu 10–20 trang trước buổi học, tôi muốn nắm ý chính và những phần cần đọc kỹ, để vào lớp hiểu kịp nội dung |
| Actor | Học viên chuẩn bị bài trước mỗi buổi học |
| Thời điểm / bối cảnh | Tối trước buổi học, 2–3 bài/tuần |
| Quy trình hiện tại (3–7 bước) | 1. Mở tài liệu, lướt qua · 2. Đọc từ đầu đến cuối · 3. Gạch ý chính · 4. Viết ghi chú tóm tắt · 5. Đánh dấu chỗ chưa hiểu |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 đọc toàn bộ: ~35 phút, nhiều đoạn không liên quan mục tiêu buổi học |
| Impact (nếu không giải thì sao) | ~60 phút/bài × 2–3 bài/tuần = 2–3 giờ/tuần; khi thiếu thời gian thì đọc sơ, vào lớp không theo kịp |
| Success metric (baseline → target) | 60 → dưới 30 phút/bài; tự kiểm bằng 3 câu hỏi cuối bài, đúng ≥ 2/3 |
| Phương án không dùng AI | Đọc theo kỹ thuật SQ3R/đọc mục lục + tóm tắt + kết luận trước; checklist câu hỏi định hướng |
| Giả thuyết về AI (nếu có) | Công cụ tóm tắt cho bản nháp ý chính + danh sách phần cần đọc kỹ; người học vẫn đọc phần đó và kiểm lại |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[1 Lướt qua: 5'] → [2 Đọc toàn bộ: 35'] ← BOTTLENECK
→ [3 Gạch ý chính: 8'] → [4 Viết ghi chú: 10'] → [5 Đánh dấu chỗ chưa hiểu: 2']
Tổng ~60'
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu một tuần học, tôi muốn thấy mọi deadline ở một chỗ, để không lỡ hạn nộp |
| Actor | Học viên theo học nhiều môn/lab cùng lúc |
| Thời điểm / bối cảnh | Sáng thứ Hai hằng tuần |
| Quy trình hiện tại (3–7 bước) | 1. Mở LMS xem bài tập · 2. Lục email thông báo · 3. Cuộn tin nhắn nhóm tìm hạn · 4. Ghi tay vào sổ/lịch · 5. Đặt nhắc |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, cuộn tin nhắn nhóm: ~7 phút, dễ sót |
| Impact (nếu không giải thì sao) | ~15 phút/tuần; tuần trước suýt trễ 1 bài |
| Success metric (baseline → target) | 15 → 5 phút/tuần; 0 deadline bị bỏ sót/kỳ (baseline: 1 lần suýt trễ/tháng) |
| Phương án không dùng AI | Google Calendar dùng chung cho cả lớp/nhóm + quy ước ghi deadline vào một kênh ghim |
| Giả thuyết về AI (nếu có) | Có thể trích deadline từ tin nhắn tự do; nhưng cần kiểm lại độ chính xác |
| Cảm nhận nhanh | Rule / No AI |

Quy trình nháp hiện tại:

```text
[1 LMS: 3'] → [2 Email: 3'] → [3 Tin nhắn nhóm: 7'] ← BOTTLENECK
→ [4 Ghi tay: 2'] → [5 Đặt nhắc: 1']
Tổng ~16'
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần tìm lại một slide/ghi chú đã học tuần trước, tôi muốn tìm ra đúng file ngay, để không phải mở từng thư mục |
| Actor | Học viên khi ôn bài hoặc làm lab |
| Thời điểm / bối cảnh | Lúc làm lab hoặc ôn thi, 3–4 lần/tuần |
| Quy trình hiện tại (3–7 bước) | 1. Nhớ file ở đâu · 2. Mở Drive tìm · 3. Không thấy, sang LMS · 4. Sang Zalo/nhóm chat · 5. Mở và kiểm đúng file |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–4, đoán sai nơi lưu: ~7 phút |
| Impact (nếu không giải thì sao) | ~10 phút × 3–4 lần = 30–40 phút/tuần, ngắt mạch làm việc |
| Success metric (baseline → target) | 10 → dưới 2 phút/lần |
| Phương án không dùng AI | Quy ước đặt tên + một thư mục duy nhất theo môn/tuần |
| Giả thuyết về AI (nếu có) | Tìm kiếm theo nội dung trên mọi nguồn; cần quyền truy cập nhiều nền tảng |
| Cảm nhận nhanh | No AI / Chưa biết |

Quy trình nháp hiện tại:

```text
[1 Nhớ: 1'] → [2 Drive: 3'] → [3 LMS: 2'] → [4 Chat: 2'] ← BOTTLENECK (2–4)
→ [5 Kiểm file: 2']
Tổng ~10'
```

### Card muốn pitch nhất

- Card số: 1 (Chuẩn bị bài đọc trước buổi học)
- Vì sao: Baseline lớn nhất (60 phút), lặp lại nhiều lần/tuần, và có chỗ để so sánh đủ 4 mức can thiệp.
- Câu hỏi muốn nhóm phản biện: Nếu công cụ tóm tắt bỏ sót ý quan trọng thì người học có biết để đọc lại không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 60 phút chỉ là ước lượng | Đồng ý | Bấm giờ 3 bài liên tiếp để lấy số thật |
| "Hiểu đủ" chưa có cách đo | Đồng ý | Thêm 3 câu hỏi tự kiểm cuối bài vào metric |
| Gợi ý AI tự đọc và thay người học | Không đồng ý | Giữ boundary: người học vẫn đọc phần quan trọng |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 "Chuẩn bị bài đọc" | Vào shortlist, được chọn làm candidate |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Bài của bạn đo 'nhanh hơn' bằng gì, baseline lấy từ đâu?" | Bạn đó thêm số phút bấm giờ thật |
| Nhận phản biện | Câu hỏi tôi nhận được: "Chỉ đọc mục lục + kết luận có đủ không?" | Tôi thêm phương án No AI (SQ3R) vào so sánh 4 mức |
| Gom cluster / cây OST | Gom các candidate liên quan đọc/tổng hợp vào cluster A | Cây OST có 1 outcome, các nhánh là pain |
| Chọn candidate problem | Chấm điểm shortlist 3 candidate | Chọn bài có baseline đo được |
| Kiểm chứng / research | Phỏng vấn và tìm công cụ tóm tắt có sẵn | Nhóm đổi từ "tự xây" sang "dùng công cụ có sẵn" |
| Quy trình nhóm | Vẽ quy trình hiện tại/tương lai | Dùng làm bản cuối |
| Problem Statement | Viết v0 | Bổ sung metric chất lượng ở v1 |
| Mức can thiệp AI | Đề xuất Workflow | Nhóm chọn Workflow |
| Quyết định | Đề xuất Go, phạm vi nhỏ | Nhóm chọn Go với ngưỡng dừng |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm problem cho học viên | Nhắc ôn thi, format bài nhóm | Có ý quá rộng ("trợ lý học tập") | Bỏ ý không có quy trình thật |
| CP2 Problem Card | Đóng vai PM hoài nghi phản biện | Chỉ ra baseline chỉ là ước lượng | Gợi ý AI đọc thay hoàn toàn | Giữ boundary người học vẫn đọc |
| CP4 Research | Tìm công cụ tóm tắt tài liệu | Gợi ý vài công cụ có sẵn | Link/tính năng có thể đã đổi | Tự mở từng link, kiểm lại tính năng |
| CP5 Quy trình | Chuyển mô tả sang Mermaid | Nhanh | Gộp bước tóm tắt và kiểm tra thành một | Tách lại vì bước kiểm là điểm kiểm soát |
| CP5–6 Problem Statement | Hỏi lỗ hổng của v0 | Chỉ ra metric chỉ đo tốc độ | Đề xuất viết lại cả đoạn | Chỉ lấy điểm yếu, tự viết lại |
| CP6 Mức can thiệp / quyết định | Hỏi phản biện lựa chọn Workflow | Nhắc cân nhắc Rule trước | Quá khuyến khích dùng Agent | Giữ Workflow, ghi lý do không chọn Agent |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Tôi nhận ra nhiều bạn mô tả vấn đề rất cụ thể bằng con số (số phút, số lần mỗi tuần), còn bản scan đầu của tôi thiên về cảm giác "mất thời gian". Nghe các bạn pitch, tôi thấy một problem tốt thường có một bước nghẽn gọi tên được. Tôi cũng thấy vài vấn đề nghe hay nhưng thực ra chỉ cần đổi cách làm, không cần công nghệ gì thêm.

**6.2. Nhóm có lúc nào bị "solution-first" không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có. Lúc đầu có bạn đề xuất ngay "làm chatbot tóm tắt tài liệu" trước khi ai nói rõ ai đọc, đọc lúc nào, mất bao lâu. Khi vẽ cây OST, nhóm gạch "chatbot" ra khỏi tầng opportunity và đổi thành pain "đọc toàn bộ tài liệu tốn thời gian dù chỉ cần vài phần". Từ đó cuộc thảo luận chuyển sang bước nào trong quy trình đang nghẽn.

**6.3. Tôi có đổi ý sau khi bị phản biện không?**
Có. Tôi từng nghĩ Card #1 cần công cụ tóm tắt. Bạn trong nhóm hỏi "chỉ đọc mục lục, tóm tắt và kết luận có đủ không?". Tôi thêm phương án No AI vào bảng so sánh và đưa vào câu hỏi phỏng vấn. Kết quả là nhóm xác định rõ nhóm bạn nào đọc kỹ cần dùng công cụ, nhóm nào chỉ cần kỹ thuật đọc.

**6.4. Kết quả kiểm chứng có làm tôi bất ngờ không?**
Có. Tôi nghĩ ai cũng muốn tóm tắt cả bài, nhưng một số bạn cho biết họ thích tự đọc phần chính để không bỏ sót chi tiết. Điều đó làm tôi hiểu người học muốn được hỗ trợ chứ không phải được đọc thay, và thiết kế phải giữ vai trò người đọc.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Viết Success Metric có baseline, target và cách đo. Rất dễ viết "nhanh hơn" hoặc "hiểu tốt hơn", trong khi cần một con số và cách kiểm. Phần Boundary cũng khó vì phải nói rõ công cụ không được làm gì và khi nào cần người kiểm tra.

**6.6. Nếu làm lại, tôi sẽ đổi gì?**
Tôi sẽ bấm giờ thật ngay từ CP1 thay vì ước lượng, vì baseline thật làm mọi bước sau chắc hơn. Tôi cũng sẽ phản biện nhóm mạnh hơn về giả định "người học muốn tóm tắt" ngay từ CP3, thay vì đợi đến lúc kiểm chứng mới thấy tín hiệu phản bác.

**6.7. Hiểu bài:** Problem của nhóm là người học mất khoảng 60 phút/bài để chuẩn bị bài đọc trước buổi học, trong đó bước đọc toàn bộ chiếm khoảng 35 phút. Quy trình hiện tại gồm 5 bước thủ công; quy trình tương lai dùng Rule để lấy tài liệu vào khung câu hỏi định hướng, công cụ tóm tắt tạo nháp ý chính, và người học vẫn đọc phần quan trọng rồi tự kiểm. Metric là giảm từ 60 xuống dưới 30 phút/bài và trả lời đúng ít nhất 2/3 câu hỏi tự kiểm. Boundary: công cụ không thay người học đọc phần quan trọng và không đưa ý không có trong tài liệu. Mức can thiệp chọn là Workflow vì các bước cố định, chỉ riêng bước tóm tắt cần xử lý ngôn ngữ; Agent là thừa. Quyết định là Go phạm vi nhỏ với ngưỡng dừng nếu 2 tuần mà điểm tự kiểm tụt dưới 2/3 thì quay lại kỹ thuật đọc không dùng AI.

---

## 7. Tài liệu tham khảo

- docs/01-worksheet.md, docs/02-deliverable-example.md, docs/03-international-frameworks.md trong repo
- The Mom Test (Rob Fitzpatrick); Google PAIR People + AI Guidebook
