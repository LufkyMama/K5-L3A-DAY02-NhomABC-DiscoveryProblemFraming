# Báo cáo cá nhân — 2A202603572_BuiHuuPhuc

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Bùi Hữu Phúc
- MSSV: 2A202603572
- Email trường (không bắt buộc, repo có thể để public): phucbh.66.24@gmail.com
- Tên nhóm: Nhóm ABC
- Link repo nhóm: https://github.com/LufkyMama/K5-L3A-DAY02-NhomABC-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại|Khi chuẩn bị cập nhật OKR vào cuối tháng , tôi muốn nhanh chóng thu thập các metric từ jira, google data studio để chèn vào slide, tránh việc mở từng báo cáo một  | PM,EM|2h/tuần( mở 3 dashboard, sao chép 5 cột dữ liệu |
| 2 |Tốn thời gian |Khi nhận phản hồi khách hàng và muốn tổng hợp pain chính cho product-team, tôi phải đọc toàn bộ chuỗi mail và comment trên Confluence |PM,Customer Succes |40-50 phút/Tuần, 10-15 email |
| 3 |Cần đọc, tổng hợp |Khi đánh giá hiệu xuất, tôi cần đánh giá số story point đã hoàn thành, velocity và bug count qua 4-6 sprint gần nhất |PM,EM,CEO |30 phút/đợt mỗi 2-3 tuần |
| 4 |Pain từ người khác |khi designer hỏi về định dạng UI đã được chấp nhận trong sprint trước, tôi phải tìm lại các tin nhắn trên Slack + file Figma để trả lời |Designer,PM |12-15 phút/ mỗi yêu cầu, 3-4 yêu cầu/tuần |
| 5 |Pain từ người khác |khi CEO yêu cầu đánh giá rủi ro của dự án hiện tại trong buổi họp leadership, tôi phải điều tra các issue chưa đóng trong Jira, truy vấn comment trong slack và tham khảo tài liệu Confluence để đưa ra bản tóm tắt ngắn gọn |CEO,PM|20 phút/mỗi lần (họp 2-3 lần/tuần) |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Báo cáo tuần |quy trình rõ, tốn thời gian, có baseline thực tế (xấp xỉ 90 phút/ tuần |Đánh giá “narrative đủ tốt” chưa có tiêu chí đo lường |
| 2 |Review PRD |Pain thực, nhiều người (PM reviewer, design lead) phải đọc 10‑15 trang, thời gian ≈ 45 phút/bản |Độ “chất lượng review” khó đo, ảnh hưởng tới tốc độ phát triển |
| 3 |Đánh giá rủi ro dự án cho CEO |CEO hỏi rủi ro trong buổi leadership, yêu cầu tổng hợp thông tin từ Jira, Slack, Confluence → ≈ 20 phút/mỗi lần, tần suất 2‑3 / tuần |Không chắc CEO sẽ dùng ngay bản tóm tắt, hoặc muốn chi tiết hơn |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi tới sáng thứ Hai, tôi muốn có số liệu sprint và tình hình team ở một chỗ, để gửi báo cáo tuần cho CEO trước 10 h. |
| Actor |Junior PM (Minh) chịu trách nhiệm báo cáo cho Engineering Manager và CEO. |
| Thời điểm / bối cảnh | Sáng thứ Hai, trước buổi họp leadership lúc 10 h.|
| Quy trình hiện tại (3–7 bước) | 1. Export dữ liệu Sprint từ Jira 2. lấy số từ google sheet 3. Đọc lại Slack cả tuần  4.tổng hợp vào google docs 5. Viết narrative 6. review và format 7. gửi email|
| Bottleneck (bước nào, mất bao nhiêu phút) | bước 5. viết narrative khoảng 25 phút (giấy trắng) |
| Impact (nếu không giải thì sao) | 90 phút/tuần cho 1 PM → ≈ 270 phút/tuần cho 3 PM; 3/8 tuần gần nhất báo cáo trễ, gây mất tin cậy với CEO/EM.|
| Success metric (baseline → target) | Baseline ≈ 90 phút/tuần → Target < 30 phút/tuần, đồng thời số câu hỏi lại từ CEO/EM không tăng.|
| Phương án không dùng AI |Template cố định + dashboard Jira + checklist → giảm thời gian format, không giảm thời gian viết narrative. |
| Giả thuyết về AI (nếu có) | viết phác thảo narrative |
| Cảm nhận nhanh |Workflow (AI hỗ trợ viết, người dùng kiểm duyệt). |

Quy trình nháp hiện tại:

```text

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story |Khi nhận PRD 10–15 trang, tôi muốn nắm nhanh các quyết định chính, để comment đúng chỗ trước hạn. |
| Actor |PM reviewer (Minh) cùng design lead. |
| Thời điểm / bối cảnh | Khi PRD mới được đưa lên trong sprint planning (2‑3 lần/tuần).|
| Quy trình hiện tại (3–7 bước) |1. Mở PRD trong Confluence.
2. Đọc toàn bộ tài liệu (≈ 45 phút).
3. Highlight các quyết định/requirement.
4. Viết comment trên PRD.
5. Đánh giá lại với designer. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2 – đọc toàn bộ tài liệu: ≈ 45 phút/bản. |
| Impact (nếu không giải thì sao) |45 phút × 2 bản/tuần ≈ 90 phút/tuần cho 1 PM; kéo dài thời gian quyết định, ảnh hưởng tới tốc độ phát triển. |
| Success metric (baseline → target) |Baseline ≈ 45 phút/bản → Target ≤ 20 phút/bản, độ chính xác comment ≥ 90 % (so với after‑review). |
| Phương án không dùng AI |Sử dụng checklist để “scan nhanh” các phần quan trọng; giảm nhưng vẫn phải đọc toàn bộ tài liệu. |
| Giả thuyết về AI (nếu có) | tóm tắt PRD |
| Cảm nhận nhanh | Workflow (AI tóm tắt, người dùng kiểm tra).|

Quy trình nháp hiện tại:

```text

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story |	Khi CEO chuẩn bị buổi họp leadership, tôi muốn có bản tóm tắt rủi ro dự án (các issue chưa đóng, comment quan trọng), để CEO nắm nhanh tình hình|
| Actor |Junior PM (Minh) hỗ trợ CEO & leadership team |
| Thời điểm / bối cảnh |1-2 ngày trước khi diễn ra buổi họp |
| Quy trình hiện tại (3–7 bước) |1. Truy vấn open issues trong Jira (filter)
2. Tìm thread liên quan trong Slack (keyword)
3. Đọc tài liệu Confluence tương ứng
4. Soạn bản tóm tắt rủi ro (≈ 20 phút) |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2‑3 – phải đọc nhiều nguồn: tổng cộng ≈ 15 phút mỗi lần |
| Impact (nếu không giải thì sao) | Nếu không kịp, CEO có thể đến muộn hoặc thiếu thông tin, gây giảm độ tin cậy và quyết định sai|
| Success metric (baseline → target) |	Baseline ≈ 20 ph phút/đợt → Target ≤ 5 phút/đợt, độ chính xác nội dung ≥ 95 % (so với after‑meeting verification) |
| Phương án không dùng AI |Tạo template rủi ro và bookmark các query Jira/Slack; vẫn tốn thời gian tìm kiếm thủ công |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Card muốn pitch nhất

- Card số:1 báo cáo tuần
- Vì sao: Đây là bottleneck lớn nhất (25 phút mỗi tuần), ảnh hưởng tới toàn bộ team PM, và có baseline đo được; cải thiện sẽ mang lại lợi nhuận thời gian ngay lập tức
- Câu hỏi muốn nhóm phản biện: 1. Tiêu chí “narrative đủ tốt”: Làm sao đo được chất lượng nội dung sau khi AI soạn?
2. Mức độ tự động hoá: AI có nên tự gửi email sau khi PM approve, hay để PM luôn là “gatekeeper”?
3. Rủi ro bảo mật dữ liệu khi AI truy cập dữ liệu Jira/Sheets/Slack – cần kiểm soát gì?


### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|Baseline 90 phút dựa trên trí nhớ, chưa có đo thực|Đồng Ý |Đánh thời gian bấm giờ thực tế 2 tuần → 85 và 95 phút|
|CEO có chắc đọc phần narrative | Đồng ý một phần |Đưa vào giả định cần kiểm chứng ở CP4 (kiểm tra feedback CEO) |
|Gợi ý AI tự gửi báo cáo|Không đồng ý|Giữ “PM review trước khi gửi” làm ranh giới, tránh tự động gửi không kiểm tra|


## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
