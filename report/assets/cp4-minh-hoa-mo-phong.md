# CP4 — Ví dụ mô phỏng cách ghi và phân tích kiểm chứng

Candidate minh họa: người học chuẩn bị tài liệu 10–20 trang trước buổi học, cần nắm ý chính và biết phần phải đọc kỹ.


## 1. Interview Snapshot PV01 — mô phỏng

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên đang học môn nhập môn học máy, chưa quen đọc tài liệu chuyên ngành (nhân vật giả định). |
| Câu nói đáng nhớ nhất (nguyên văn) | Lời thoại mô phỏng: “Mình đọc hết rồi mới biết đoạn nào cần ghi kỹ.” |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Trong kịch bản, sinh viên được giao đọc 18 trang về hồi quy tuyến tính trước buổi học. Vì chưa biết phần nào quan trọng nên đọc từ đầu rồi mới ghi ý; khi vào lớp vẫn phải mở lại tài liệu để giải thích khi nào dùng mô hình. |
| Hiện đang xử lý bằng cách nào (workaround)? | Gạch câu có vẻ quan trọng, đọc lại tiêu đề và kết luận rồi chép vào ghi chú. Bài nào có câu hỏi định hướng trước thì dễ chọn đoạn để đọc hơn, nhưng chưa so sánh thời gian. |
| Mất bao lâu, bao lần? | Giả định 60 phút/bài, 3 bài/tuần: lướt 5' → đọc tuần tự 30' → gạch ý 10' → ghi chú 10' → đánh dấu câu hỏi 5'. Số liệu mô phỏng, chưa đo thực tế. |
| Insight / opportunity rút ra | Cần xác định phần phải đọc kỹ theo mục tiêu buổi học. Tuy nhiên, nhân vật chưa thử đọc theo câu hỏi định hướng nên chưa thể kết luận cần AI; giữ No AI làm đối chứng. |

## 2. Interview Snapshot PV02 — mô phỏng

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên đọc tài liệu kỹ thuật tiếng Anh, chưa vững một số khái niệm xác suất (nhân vật giả định). |
| Câu nói đáng nhớ nhất (nguyên văn) | Lời thoại mô phỏng: “Mình biết cần đọc phần nào, nhưng chưa hiểu thuật ngữ trong phần đó.” |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Trong kịch bản, sinh viên đọc 15 trang về đánh giá mô hình. Dù giảng viên đã chỉ phần cần đọc, sinh viên vẫn phải tra precision, recall và xác suất có điều kiện; khi làm ví dụ mới nhận ra chưa giải thích được cách chọn chỉ số. |
| Hiện đang xử lý bằng cách nào (workaround)? | Tra từ điển, mở slide cũ và xem ví dụ. Bản tóm tắt bạn chia sẻ giúp biết chủ đề nhưng chưa đủ để hiểu khái niệm; với chủ đề quen thì ít phải tra cứu hơn. |
| Mất bao lâu, bao lần? | Giả định 55 phút/bài, 2 bài/tuần: chọn phần cần đọc 5' → đọc phần liên quan 10' → tra thuật ngữ/kiến thức nền 25' → ghi chú 10' → ghi câu hỏi 5'. Số liệu mô phỏng, chưa đo thực tế. |
| Insight / opportunity rút ra | Bottleneck trong kịch bản là hiểu thuật ngữ và kiến thức nền, không phải tìm ý chính. Cần tách nhu cầu giải thích khái niệm khỏi nhu cầu định hướng đọc; tóm tắt ngắn hơn chưa giải quyết nguyên nhân. |

## 3. Tổng hợp hai tình huống mô phỏng

| Nguồn | Quy mô / loại dữ liệu | Tín hiệu xác nhận trong kịch bản | Tín hiệu phản bác / giới hạn |
|---|---|---|---|
| PV01 — khó xác định phần cần đọc | 1 tình huống mô phỏng AI | 60 phút/bài, 3 bài/tuần; đọc tuần tự 30 phút vì chưa biết phần quan trọng. | Chưa thử câu hỏi định hướng; chưa biết No AI có đủ hay không. |
| PV02 — thiếu thuật ngữ và kiến thức nền | 1 tình huống mô phỏng AI | 55 phút/bài, 2 bài/tuần; tra thuật ngữ/kiến thức nền chiếm 25 phút. | Nguyên nhân chính là chưa hiểu khái niệm; bản tóm tắt ngắn hơn chưa giải quyết bottleneck. |

**Nhận định minh họa:**

- Hai tình huống có thời gian chuẩn bị dài nhưng nguyên nhân khác nhau. Không coi mọi người đọc chậm là cùng một nhóm nhu cầu.
- PV01 minh họa nhu cầu định hướng đọc; PV02 phản bác việc áp dụng cùng giải pháp tóm tắt cho mọi người.
- Chưa có tình huống đo thử thành công cách đọc có câu hỏi định hướng hoặc công cụ AI. Giữ cả hai phương án để so sánh bằng dữ liệu thật.
- Hai tình huống không phải hai người được phỏng vấn; không dùng thời gian trong bảng làm baseline đo được hoặc suy ra tỷ lệ người học gặp pain.

## 4. Minh họa cách sửa problem

| Nội dung | Ban đầu | Điều chỉnh đề xuất nếu dữ liệu thật cho thấy tương tự |
|---|---|---|
| Actor | Người học đọc tài liệu 10–20 trang trước buổi học. | Người học chưa xác định được phần phải đọc kỹ theo mục tiêu một buổi học cụ thể. |
| Bottleneck | Đọc toàn bộ tài liệu mất nhiều thời gian. | Tìm và lựa chọn phần liên quan trước khi đọc kỹ; kiểm tra lại bằng thời gian từng bước. |
| Phạm vi | Mọi nguyên nhân khiến người học đọc chậm. | Tách trường hợp thiếu thuật ngữ/kiến thức nền để xem xét riêng. |
| Success metric | Chỉ tập trung giảm thời gian chuẩn bị. | Đo cả thời gian và mức hiểu bài; tính cả thời gian đọc hướng dẫn/tóm tắt, kiểm nguồn và tự kiểm. |
| Boundary | Chưa xác định. | Công cụ không thay người học đọc đoạn quan trọng; mọi nhận định phải kiểm được với nguồn. |

**Cách đo thử đề xuất:** Ghi baseline thời gian và chất lượng của cách đọc hiện tại. Chuẩn bị bộ câu hỏi và đáp án độc lập với đầu ra AI, so sánh trên bài có độ khó tương đương. Thử đọc theo câu hỏi định hướng trước; chỉ cân nhắc AI nếu vẫn còn bước nghẽn. Mục tiêu dưới 30 phút/bài chưa phải kết quả đã đạt.

## 5. Minh họa kết luận về giả định và quyết định

| Giả định trong báo cáo nhóm | Nhận định từ bộ mô phỏng |
|---|---|
| #1 — Pain lặp lại ở người học ngoài nhóm | Hai kịch bản minh họa pain, nhưng không tạo bằng chứng ngoài nhóm hoặc làm tăng điểm bằng chứng thực tế. |
| #2 — Khó chọn phần quan trọng là nguyên nhân chính | PV01 phù hợp, PV02 cho thấy nguyên nhân khác; nếu gặp pattern này trong dữ liệu thật thì cần thu hẹp actor. |
| #3 — Nhanh hơn mà không giảm mức hiểu | Chưa được kiểm tra; cần đo thử chất lượng và thời gian. |
| #4 — Người học kiểm lại nguồn | Kịch bản có nhắc mở lại tài liệu, nhưng chưa chứng minh người học kiểm chứng đầu ra AI; cần hỏi hoặc quan sát thực tế. |
| #5 — Công cụ xử lý được tài liệu và dẫn nguồn | Đối chiếu research ở mục 3.3 của báo cáo nhóm; khả năng xử lý đúng file dự kiến vẫn cần thử. |
| #6 — Quyền dùng tài liệu, tài khoản và chi phí phù hợp | Chưa có dữ liệu xác nhận. |

**Kết luận minh họa:** Not Yet đối với việc khẳng định bài toán đã được kiểm chứng hoặc triển khai AI. Cần phỏng vấn thật, làm rõ baseline, kiểm quyền dùng tài liệu và đo thử trước khi chốt. Đây là đề xuất minh họa, chưa phải quyết định của nhóm ở CP6.
