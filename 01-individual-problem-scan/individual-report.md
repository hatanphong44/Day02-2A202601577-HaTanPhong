# Brainstorm Problems

| # | Loại | Vấn đề | Actor | Evidence |
|---|------|--------|-------|----------|
| 1 | Lặp lại | Tìm deadline của từng môn trên Discord | Sinh viên | Mỗi tuần mất khoảng 15–20 phút |
| 2 | Tốn thời gian | Đọc slide và tài liệu dài trước khi làm assignment | Sinh viên | Mỗi môn mất khoảng 1–2 giờ để đọc và ghi chú |
| 3 | AI có thể tốt hơn | Tổng hợp nhiều tài liệu thành ghi chú ôn tập | Sinh viên | Phải đọc nhiều nguồn và tự tổng hợp thủ công |
| 4 | Pain từ người khác | Bạn cùng lớp thường hỏi lại deadline và yêu cầu bài tập | Sinh viên và nhóm | Các câu hỏi lặp lại nhiều lần mỗi tuần trên nhóm chat |
| 5 | Lặp lại | Viết báo cáo tiến độ đồ án theo cùng một format | Sinh viên | Thực hiện hằng tuần trong quá trình làm đồ án |
| 6 | Tốn thời gian | Tìm đoạn code cũ trong nhiều project khác nhau | Sinh viên AI | Mỗi lần tìm mất khoảng 10–30 phút |
| 7 | AI có thể tốt hơn | Debug lỗi Python/PyTorch mất nhiều thời gian vì log dài | Sinh viên AI | Có trường hợp mất vài giờ mới xác định được nguyên nhân |
| 8 | Pain từ người khác | Nhóm đồ án thường quên task hoặc deadline đã phân công | Nhóm dự án | Thành viên phải nhắc nhau nhiều lần |
| 9 | Lặp lại | Tổng hợp tài liệu trước kỳ thi | Sinh viên | Mỗi kỳ thi đều phải gom tài liệu từ nhiều nguồn |
| 10 | Tốn thời gian | Đọc paper AI bằng tiếng Anh | Sinh viên AI | Mỗi bài báo mất khoảng 30–60 phút để đọc và hiểu |

---

# Top 3 Problems

| # | Problem | Lý do chọn | Challenge |
|---|---------|------------|-----------|
| 1 | Đọc slide và tài liệu dài trước khi làm assignment | Workflow rõ, mất nhiều thời gian, hầu hết sinh viên đều gặp | AI tóm tắt có đủ chính xác và không bỏ sót ý quan trọng không |
| 2 | Debug code AI | Pain lớn, nhiều sinh viên gặp | Khó đo chất lượng |
| 3 | Tìm deadline nhiều nơi | Lặp lại thường xuyên | Có thể chỉ cần quy trình tốt hơn |

---

# Problem Card #1 — Đọc slide và tài liệu trước Assignment

## Problem 1 câu

Đọc slide và tài liệu dài trước khi làm assignment.

## Actor

Sinh viên chuẩn bị làm assignment.

## Thời điểm / bối cảnh

Trước mỗi bài tập hoặc bài kiểm tra của môn học.

## Current workflow

1. Kiểm tra deadline
2. Tải slide và tài liệu học
3. Đọc toàn bộ slide/PDF
4. Ghi chú các nội dung quan trọng
5. Đối chiếu với yêu cầu assignment
6. Bắt đầu làm bài

## Bottleneck

Bước 3–4: đọc hiểu và ghi chú tài liệu mất khoảng 60 phút, đặc biệt khi tài liệu dài hoặc bằng tiếng Anh.

## Impact

Mỗi môn học mất khoảng 60–90 phút chuẩn bị. Khi học nhiều môn cùng lúc, sinh viên dễ mất nhiều giờ chỉ để đọc tài liệu và thường bắt đầu làm assignment sát deadline.

## Success metric

Giảm thời gian chuẩn bị từ 90 phút xuống dưới 30 phút nhưng vẫn đảm bảo không bỏ sót nội dung quan trọng của bài học.

## Non-AI alternative

Highlight thủ công, ghi chú bằng Notion hoặc OneNote, tạo template ghi chú theo từng môn.

## AI hypothesis

AI hỗ trợ tóm tắt tài liệu, tạo checklist kiến thức và gợi ý các phần cần đọc kỹ trước khi làm assignment.

## Quick gut

Workflow.

## Draft current workflow

### CURRENT STATE — 90 phút

```text
[1 Kiểm tra deadline: 5']
→ [2 Tải slide/PDF: 5']
→ [3 Đọc tài liệu: 50']
→ [4 Ghi chú: 20']  <-- bottleneck
→ [5 Đối chiếu assignment: 5']
→ [6 Bắt đầu làm bài: 5']
```

## Draft future workflow

### FUTURE STATE — 30 phút

```text
[1 Tải tài liệu: 5']
→ [2 AI tóm tắt nội dung: 2']
→ [3 AI tạo checklist kiến thức: 3']
→ [4 Sinh viên review + bổ sung: 15']  <-- human boundary
→ [5 Bắt đầu làm assignment: 5']
```

**Fallback:** AI tóm tắt thiếu hoặc sai → Sinh viên đọc lại tài liệu gốc.

---

# Problem Card #2 — Debug lỗi Python/PyTorch

## Problem 1 câu

Khi gặp lỗi Python hoặc PyTorch, sinh viên thường mất nhiều thời gian đọc traceback và tìm nguyên nhân trước khi có thể sửa lỗi.

## Actor

Sinh viên học AI.

## Thời điểm / bối cảnh

Trong quá trình làm bài tập, đồ án hoặc luyện tập lập trình AI.

## Current workflow

1. Chạy chương trình
2. Chương trình báo lỗi
3. Đọc traceback
4. Tìm kiếm lỗi trên Google/Stack Overflow
5. Thử sửa code
6. Chạy lại chương trình

## Bottleneck

Bước 3–4: đọc traceback và xác định nguyên nhân lỗi mất khoảng 30–90 phút, có trường hợp kéo dài vài giờ.

## Impact

Tiến độ làm bài bị chậm, sinh viên dễ sửa sai hướng hoặc phải thử nhiều cách mới tìm được nguyên nhân.

## Success metric

Giảm thời gian debug từ khoảng 2 giờ xuống dưới 30 phút mà vẫn xác định đúng nguyên nhân lỗi.

## Non-AI alternative

Tra cứu tài liệu chính thức, Stack Overflow hoặc hỏi giảng viên, bạn bè.

## AI hypothesis

AI phân tích traceback, giải thích nguyên nhân lỗi và gợi ý các bước sửa phù hợp để sinh viên tự kiểm tra trước khi áp dụng.

## Quick gut

Workflow.

## Draft current workflow

### CURRENT STATE — 120 phút

```text
[1 Chạy chương trình: 2']
→ [2 Xuất hiện lỗi: 1']
→ [3 Đọc traceback: 30']
→ [4 Tìm cách sửa: 60']  <-- bottleneck
→ [5 Sửa code: 20']
→ [6 Chạy lại: 7']
```

## Draft future workflow

### FUTURE STATE — 30 phút

```text
[1 Chạy chương trình: 2']
→ [2 Copy traceback: 1']
→ [3 AI phân tích lỗi: 2']
→ [4 Sinh viên review + sửa code: 20']  <-- human boundary
→ [5 Chạy lại: 5']
```

**Fallback:** AI phân tích sai → Debug thủ công hoặc tra tài liệu.

---

# Problem Card #3 — Tìm deadline trên nhiều nền tảng học tập

## Problem 1 câu

Sinh viên phải kiểm tra deadline trên nhiều nền tảng khác nhau nên mất thời gian và dễ bỏ sót bài cần nộp.

## Actor

Sinh viên.

## Thời điểm / bối cảnh

Đầu tuần hoặc trước khi lên kế hoạch học tập.

## Current workflow

1. Kiểm tra hệ thống quản lý học tập
2. Mở LMS xem assignment
3. Đọc thông báo trên Discord hoặc nhóm lớp
4. Tự tổng hợp deadline
5. Ghi vào lịch hoặc checklist

## Bottleneck

Bước 3–4: thông tin nằm ở nhiều nơi nên phải tự đối chiếu và tổng hợp, mất khoảng 15–20 phút mỗi tuần.

## Impact

Dễ bỏ sót deadline hoặc mất thời gian kiểm tra lặp lại nhiều lần trong tuần.

## Success metric

Giảm thời gian kiểm tra deadline từ khoảng 20 phút xuống dưới 5 phút và không bỏ sót bài cần nộp.

## Non-AI alternative

Tự cập nhật Google Calendar hoặc checklist sau mỗi buổi học.

## AI hypothesis

AI tổng hợp deadline từ nhiều nguồn thành một danh sách và hỗ trợ nhắc việc khi cần.

## Quick gut

Workflow.

## Draft current workflow

### CURRENT STATE — 20 phút

```text
[1 Kiểm tra hệ thống học tập: 5']
→ [2 Mở LMS: 5']
→ [3 Đọc thông báo: 5']
→ [4 Tự tổng hợp deadline: 3']  <-- bottleneck
→ [5 Lưu vào lịch: 2']
```

## Draft future workflow

### FUTURE STATE — 5 phút

```text
[1 Thu thập deadline từ nhiều nguồn: 1']
→ [2 AI tổng hợp danh sách: 1']
→ [3 Sinh viên kiểm tra: 2']  <-- human boundary
→ [4 Lưu lịch: 1']
```

**Fallback:** Nếu AI thiếu thông tin → Kiểm tra trực tiếp trên các nền tảng học tập.