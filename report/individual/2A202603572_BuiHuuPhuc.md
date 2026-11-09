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
| 1 |Lặp lại|Khi kéo (pull) code mới từ main để bắt đầu ngày làm việc, tôi muốn đảm bảo môi trường local luôn đồng bộ và không gặp lỗi phụ thuộc, để khởi động công việc ngay trong 5 phút. | DEV, Team Lead |1-2 phút/lần pull, 1-2 lần/ngày |
| 2 |Tốn thời gian |Khi đánh giá (review) một Pull Request khoảng 300 dòng, tôi muốn phát hiện nhanh các lỗi logic, style & security để đưa ra feedback trong 10 phút, tránh kéo dài vòng review. |DEV, Reviewer |40-50 phút/bản|
| 3 |Cần đọc, tổng hợp |Khi phân tích log lỗi production sau một sự cố, tôi muốn tìm nguyên nhân gốc bằng cách kết hợp log, metrics và ticket liên quan, để đưa ra đề xuất fix trong 30 phút|DEV, SRE |1-2 sự cố/giờ, tuần khoảng 1-2 sự cố |
| 4 |Pain từ người khác |Khi designer yêu cầu tôi chuyển đổi một mockup Figma thành component React và muốn xem preview ngay, tôi phải đọc lại spec, tạo component và chạy storybook, mất 15‑20 phút mỗi lần|Designer,DEV |3-4 yêu cầu/tuần, khoảng 18-20 phút/yêu cầu |
| 5 |Pain từ người khác |Khi QA đưa ra danh sách regression test case mới (khoảng 20‑30 case) và muốn tôi cập nhật test automation trong repo, tôi phải đọc spec, viết script, chạy CI, mất ≈ 40 phút mỗi batch|DEV, QA|1‑2 batch/tuần, ≈ 40 phút/batch |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
| 1 |Tóm tắt ngữ cảnh & review Pull Request |Quy trình lặp lại hằng ngày, actor rõ ràng, bottleneck đọc code chiếm phần lớn thời gian, đo lường được baseline |AI có phát hiện được lỗi logic nghiệp vụ sâu hay chỉ soi được syntax/style? |
| 2 |Điều tra log lỗi Production|Pain point lớn, ảnh hưởng trực tiếp đến SLA/uptime của hệ thống, tốn nhiều chất xám để kết nối các manh mối|Log hệ thống có quá dài/nhiều dữ liệu nhạy cảm khiến context window và bảo mật bị hạn chế không? |
| 3 |Viết test cases/Unit Test cho feature mới|Tốn thời gian lặp đi lặp lại, dev thường ngại viết test dẫn đến giảm test coverage|Test do AI sinh ra có đúng format framework và mock data hợp lý không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận được một Pull Request từ đồng nghiệp (200–400 LOC), tôi muốn nhanh chóng hiểu mục đích thay đổi và logic chính, để đưa ra review chất lượng và duyệt PR trong vòng 15 phút|
| Actor |Senior / Mid Backend Developer đóng vai trò Code Reviewer trong team phát triển. |
| Thời điểm / bối cảnh | Mỗi khi có thông báo review PR trên GitHub/GitLab trong giờ làm việc (khoảng 3–4 PR/ngày)|
| Quy trình hiện tại (3–7 bước) |1. Mở PR, đọc description & ticket Jira liên quan
2. Xem danh sách files changed để nắm cấu trúc
3. Đọc từng file code, suy luận luồng dữ liệu và tìm lỗi logic
4. Viết comment góp ý trên từng dòng code 
5. Approve hoặc Request Changes |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: Đọc hiểu luồng code và rà soát lỗi logic: mất trung bình 25 phút/PR, rất dễ mệt mỏi và mất tập trung khi PR đổi nhiều file |
| Impact (nếu không giải thì sao) |PR bị nghẽn (pending review trung bình 1.5 ngày), dev chờ review bị context switching; reviewer đọc vội dễ để lọt bug lên staging/production.|
| Success metric (baseline → target) | Tổng thời gian review 1 PR giảm từ 47 phút → dưới 20 phút; Tỉ lệ bug lọt qua sau review không tăng|
| Phương án không dùng AI |Viết PR template bắt buộc ghi rõ thay đổi; giới hạn PR dưới 200 dòng (quy tắc mềm); cấu hình linter/SonarQube tự động bắt lỗi cú pháp/style |
| Giả thuyết về AI (nếu có) | AI phân tích diff, tóm tắt tóm tắt luồng logic chính, chỉ ra rủi ro tiềm ẩn (edge cases, memory leak, security flaws) để reviewer tập trung kiểm tra|
| Cảm nhận nhanh |Workflow|

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 47 phút/PR

[1. Đọc Jira & PR desc: 5'] → [2. Xem files changed: 5'] 
→ [3. Đọc hiểu luồng & tìm lỗi: 25'] ← BOTTLENECK
→ [4. Viết comment: 10'] → [5. Chốt verdict: 2']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story |	Khi hệ thống bắn alert lỗi 500 trên kênh Slack, tôi muốn nhanh chóng tìm ra file code và dòng gây lỗi cùng payload gây crash, để tạo hotfix trong vòng 30 phút|
| Actor |On-call Developer / Backend Developer phụ trách trực vận hành|
| Thời điểm / bối cảnh | Khi có sự cố đột xuất hoặc alert từ Sentry/Datadog gửi về Slack (khoảng 2–3 lần/tuần)|
| Quy trình hiện tại (3–7 bước) |1. Nhận alert Slack, bấm link mở Sentry/Datadog
2. Copy error message và trace ID tìm trong log server (Kibana/CloudWatch)
3. Đọc stack trace, đối chiếu commit code gần nhất để tìm root cause
4. Tái hiện lỗi ở môi trường local với payload lỗi
5. Viết code sửa lỗi & tạo hotfix PR |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 3: Đọc stack trace & phân tích commit gần nhất: mất 25 phút, phải lục nhiều tab và liên hệ giữa log trừu tượng với code thực tế|
| Impact (nếu không giải thì sao) |Thời gian MTTR (Mean Time To Recovery) kéo dài, ảnh hưởng trải nghiệm người dùng cuối, vi phạm SLA hệ thống|
| Success metric (baseline → target) |Thời gian định vị root cause giảm từ 38 phút (bước 1+2+3) → dưới 10 phút; Tỉ lệ chẩn đoán đúng root cause ngay lần đầu đạt > 80%|
| Phương án không dùng AI |Thiết lập log tập trung có cấu trúc (structured JSON logging); gắn Source Maps chuẩn xác; viết playbook hướng dẫn triage từng mã lỗi phổ biến|
| Giả thuyết về AI (nếu có) |AI nhận stack trace + đoạn code nghi ngờ, giải thích nguyên nhân gây crash và đề xuất đoạn patch code gợi ý |
| Cảm nhận nhanh | Workflow|

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 73 phút/sự cố

[1. Nhận alert: 3'] → [2. Tra cứu log server: 10'] 
→ [3. Đọc stack trace & tìm root cause: 25'] ← BOTTLENECK
→ [4. Tái hiện local: 15'] → [5. Viết hotfix: 20']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story |	Khi hoàn thành logic một API endpoint mới, tôi muốn có bộ Unit Test bao phủ đủ các case biên (edge cases), để tự tin merge code mà không làm crash các module khác|
| Actor |Backend Developer (Node.js/Python/Go)|
| Thời điểm / bối cảnh |Cuối mỗi sprint task khi chuẩn bị tạo Pull Request (2–3 task/tuần)|
| Quy trình hiện tại (3–7 bước) |1. Đọc lại requirement để liệt kê các test case cần viết
2. Viết file setup, mock database và dependencies 
3. Viết từng test case chi tiết cho các kịch bản thành công và lỗi
4. Chạy test suite và kiểm tra code coverage
5. Sửa lỗi test fail|
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 3: Viết chi tiết từng test case và chuẩn bị mock data: mất 35 phút, công việc nặng tính boilerplate và gõ phím lặp lại |
| Impact (nếu không giải thì sao) | Dev có xu hướng bỏ qua test hoặc chỉ viết test sơ sài (happy path), khiến coverage thấp (<50%), kỹ thuật nợ (tech debt) tăng cao|
| Success metric (baseline → target) |	Thời gian viết test giảm từ 80 phút → dưới 30 phút/task; Unit test coverage duy trì tối thiểu > 75%. |
| Phương án không dùng AI |Dùng code snippet/boilerplate generator; tái sử dụng các fixture test có sẵn; áp dụng thư viện mock data tự động (Faker) |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 80 phút/task

[1. Liệt kê test case: 10'] → [2. Setup mock: 15'] 
→ [3. Viết test code & mock data: 35'] ← BOTTLENECK
→ [4. Chạy & đo coverage: 10'] → [5. Debug test fail: 10']
```

### Card muốn pitch nhất

- Card số:1 (Tóm tắt ngữ cảnh & review Pull Request)
- Vì sao: 1. Tần suất xảy ra mỗi ngày (high frequency), ai làm dev cũng gặp ít nhất 2–4 lần/ngày.
 2. Bottleneck rõ ràng: bước "đọc hiểu luồng code" tốn thời gian nhất và gây mệt mỏi nhận thức (cognitive load).
 3. Phạm vi vừa vặn để thực nghiệm trong một buổi lab (có thể thử nghiệm ngay với prompt tóm tắt git diff).
 4. Ranh giới rõ ràng: AI chỉ hỗ trợ tóm tắt luồng và cảnh báo điểm nóng; quyết định approve/reject vẫn 100% nằm ở người review (Human-in-the-loop).
- Câu hỏi muốn nhóm phản biện:
  1. Nếu dựa vào AI để tóm tắt luồng, reviewer có bị tâm lý chủ quan, lướt qua code mà không soi kỹ các lỗi logic ngầm hay không?
  2. Với các PR lớn (>400 LOC), giới hạn token và context window của mô hình có làm AI bỏ qua các file liên quan không?
  3. Linter/SonarQube đã làm rất tốt việc bắt lỗi syntax/format, vậy AI thực sự tạo ra giá trị khác biệt ở điểm nào ngoài việc "tóm tắt bằng lời"?

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
