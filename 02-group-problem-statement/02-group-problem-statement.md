# 02 — Problem Statement (làm cá nhân)

> Bài này tôi (**Khải**) làm **một mình**, không theo nhóm. Giữ nguyên tên folder `02-group-problem-statement/` để khớp cấu trúc repo nộp bài, nhưng phần "hội tụ" được làm từ chính 10 problems tôi đã scan ở phần 01 thay vì gom từ nhiều người.
>
> Candidate problem tôi chọn để đào sâu: **Câu hỏi onboarding lặp lại của thực tập sinh**.

---

## Phase 3 — Convergence từ 10 candidates của tôi về 1

Vì làm một mình, tôi hội tụ từ chính 10 problems đã scan ở phần 01. Tôi vẫn đi qua 4 bước hội tụ (cluster → shortlist → score → chọn 1) để ép mình nói rõ lý do, không nhảy thẳng vào bài "nghe AI nhất".

### 3.1 — Danh sách candidate (từ scan cá nhân)

| # | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
|---|---|---|---|---|
| 1 | Câu hỏi onboarding lặp lại | Mentor, TTS | Tìm lại tài liệu còn hiệu lực | Workflow rõ, có baseline |
| 2 | Copy/format thông tin lặp khi onboard | Mentor | Thao tác tay lặp | Rule có thể đủ |
| 3 | "Hỏi ai cho việc gì" | TTS | Không biết owner | Là 1 chủ đề con của #1 |
| 4 | Weekly update của TTS mỗi người một format | TTS, mentor | Khó so sánh tiến độ | Lặp, nhỏ |
| 5 | Code review lỗi quy ước lặp | Reviewer, TTS | Comment lặp naming/lint | Linter có thể đủ |
| 6 | Không biết hỏi HR/IT/tech lead | TTS | Đẩy qua lại | Trùng #3 |
| 7 | Search Confluence trả kết quả kém | Cả team | Không hiểu câu hỏi tự nhiên | Scope rộng |
| 8 | Onboarding checklist theo dõi thủ công | Mentor | Sót bước | Rule/tool đủ |
| 9 | Câu hỏi nghỉ phép / chấm công lặp | HR, mentor, TTS | Thông tin trong PDF dài | Là 1 chủ đề con của #1 |
| 10 | Tổng hợp feedback cuối kỳ thực tập | Mentor, manager | Gom nhiều nguồn | Tần suất thấp (mỗi quý) |

### 3.2 — Gom trùng / cluster

| Cluster | Candidates | Pattern chung | Ghi chú |
|---|---|---|---|
| A. Hỏi-đáp quy trình lặp lại | #1, #3, #6, #9 | Cùng câu hỏi được hỏi lại; câu trả lời đã tồn tại nhưng rải rác/khó tìm | Cluster lớn nhất, 4 candidate |
| B. Tìm kiếm tài liệu | #7 | Tìm đúng thông tin trong nhiều nguồn | Scope rộng, data khó |
| C. Thao tác lặp / tracking | #2, #8 | Việc tay lặp, dễ sót | Rule/tool thường đủ |
| D. Tổng hợp / báo cáo | #4, #5, #10 | Gom nhiều nguồn rồi viết/đánh giá lại | Tần suất khác nhau |

### 3.3 — Shortlist

| Candidate | Vì sao vào shortlist | Rủi ro / điều chưa rõ |
|---|---|---|
| Onboarding Q&A lặp (cluster A, đại diện #1) | Tôi hiểu domain sâu nhất; workflow & baseline rõ | Chất lượng tài liệu nguồn; đo "đúng" thế nào |
| Search Confluence (#7) | Pain rộng, nhiều người | Scope rộng, dễ thành "xây search engine" |
| Code review lỗi quy ước (#5) | Workflow rõ, đo được số comment | Linter có thể giải mà không cần AI |

### 3.4 — Score để chọn 1

Chấm 1-5. Tôi tự chấm và buộc mình ghi lý do từng cột, đúng tinh thần "ép nói rõ lý do" của bước này.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Onboarding Q&A lặp | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| Code review lỗi quy ước | 4 | 5 | 4 | 4 | 5 | 3 | 4 | 29 |
| Search Confluence | 4 | 3 | 3 | 3 | 2 | 4 | 3 | 22 |

Candidate tôi chọn:

```text
Câu hỏi onboarding lặp lại của thực tập sinh.
```

Vì sao chọn:

```text
- Tôi vừa là TTS từng bị block, vừa là mentor đang bị gián đoạn → hiểu domain hai phía.
- Workflow rõ nhất và có baseline thời gian (đo được từ 2 đợt onboarding tôi từng kèm).
- Validate nhanh được: hỏi chính các TTS và mentor quanh mình.
- So sánh Rule / Workflow / Agent rất rõ ràng.
```

Vì sao không chọn các candidate còn lại:

```text
- Code review lỗi quy ước: phần lớn linter/pre-commit hook giải được → khó so sánh R/W/A
  một cách thú vị, AI dễ thành thừa.
- Search Confluence: scope rộng, dễ trượt sang "xây search engine"; quá lớn cho một buổi lab.
```

Làm một mình tôi xử lý "disagreement" thế nào:

```text
Không có người khác challenge nên tôi tự đóng hai vai: vai đề xuất và vai phản biện. Tôi viết
ra 3 câu hỏi chống lại lựa chọn của chính mình (xem phần 01) và dùng AI như "luật sư của quỷ"
để tìm lỗ hổng, sau đó tự chốt. Phần validation (Phase 4) đóng vai trò người ngoài challenge
thay cho nhóm.
```

---

## Phase 4 — Quick Validation + Research

### 4.1 — Quick validation

Làm một mình nên tôi dựa vào **phỏng vấn người ngoài** thay cho góc nhìn nhóm: hỏi nhanh 3 mentor + 4 TTS, và một mini poll 8 người từng onboard.

| Nguồn | Số người / mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Tôi sửa problem thế nào |
|---|---:|---|---|---|
| Interview mentor | 3 | 3/3 nói 2 tuần đầu trả lời câu lặp rất mệt; đều xác nhận "tài liệu có nhưng khó tìm/cũ" | 1 mentor nói pain lớn nhất là **tài liệu lỗi thời**, không phải tốc độ trả lời | Tách rõ 2 lớp pain: (a) tìm/trả lời chậm, (b) nguồn không đáng tin. AI chỉ trị (a) nếu (b) được làm sạch trước |
| Interview TTS | 4 | 4/4 ngại hỏi lại vì sợ làm phiền → tự loay hoay/đoán | 1 TTS thích hỏi người thật hơn bot | Boundary: bot trả câu factual, vẫn giữ kênh hỏi mentor cho câu cần ngữ cảnh |
| Mini poll | 8 | 6/8 từng hỏi lại ≥3 lần cùng một câu trong tuần đầu | 2/8 nói nơi họ có checklist tốt nên ít đau | Thêm non-AI alternative: checklist + FAQ là điều kiện nền |

Insight sau validation:

```text
Pain thật gồm HAI lớp:
1) Tìm và trả lời câu lặp tốn thời gian (mentor) + chờ lâu (TTS).
2) Tài liệu rải rác và LỖI THỜI khiến cả người lẫn bot dễ trả lời sai.

→ AI giải tốt lớp (1) NHƯNG sẽ khuếch đại lớp (2) nếu nguồn chưa được làm sạch.
Đây là điều chỉnh quan trọng so với problem ban đầu, và là phần thay cho "nhóm challenge".
```

### 4.2 — Research giải pháp đã có

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học |
|---|---|---|---|---|---|
| Notion AI Q&A | https://www.notion.com/help/notion-ai | Hỏi-đáp từ nội dung workspace | Trả lời tự nhiên ngay trong nơi lưu doc | Chỉ trong Notion; phụ thuộc doc cập nhật | Nếu KB rải nhiều app, một mình Notion AI không đủ |
| Atlassian Intelligence (Confluence) | https://www.atlassian.com/software/confluence/ai | Tìm/tóm tắt/trả lời trên Confluence | Tốt cho tài liệu kỹ thuật có cấu trúc | Vẫn lỗi thời nếu doc cũ; giới hạn trong Atlassian | Cần cơ chế giữ doc tươi, không chỉ search tốt hơn |
| Glean | https://www.glean.com/ | Trợ lý search doanh nghiệp gom nhiều app | Gom KB rải rác + trích nguồn | Chi phí/triển khai nặng cho team nhỏ | Pattern đúng: trả lời kèm trích nguồn xuyên nhiều nguồn |
| Guru | https://www.getguru.com/ | KB có "verification" — card hết hạn phải duyệt lại | Trực tiếp trị bệnh tài liệu lỗi thời | Cần người duy trì verify | **Bài học mạnh nhất:** coi tài liệu là thứ sẽ mục, phải có owner verify định kỳ |
| Slack AI | https://slack.com/features/ai | Search & tóm tắt trong Slack | Tốt khi câu trả lời nằm trong thread cũ | Chỉ 1 nguồn; không gom Notion/Confluence | Dùng như 1 input, không phải toàn bộ solution |

Research takeaway:

```text
Không cần build agent tự chạy. Hướng hợp lý: Workflow RAG Q&A —
retrieve từ KB đã index nhiều nguồn, trả lời KÈM TRÍCH NGUỒN, escalate khi không chắc.
Bài học từ Guru: vấn đề không chỉ là "tìm nhanh hơn" mà là "nguồn còn đáng tin" →
phải làm sạch + gán owner cho tài liệu 3 chủ đề lặp nhất TRƯỚC khi bật bot.
```

---

## Phase 5 — Workflow + Problem Statement

### 5.1 — Current workflow

| Bước | Actor | Input | Output | Thời gian/tần suất | Ghi chú |
|---|---|---|---|---|---|
| 1 | TTS | Câu hỏi quy trình | Tin nhắn hỏi mentor | nhiều lần/ngày tuần 1 | Có khi ngại hỏi → tự đoán |
| 2 | Mentor | Câu hỏi | Phân loại chủ đề | ~1' | |
| 3 | Mentor | Chủ đề | Tài liệu/đáp án đúng | **5-10'** | **Bottleneck:** rải 4 nguồn, một số lỗi thời |
| 4 | Mentor | Đáp án | Câu trả lời + link | ~3' | |
| 5 | TTS/Mentor | Câu trả lời | Hiểu / hỏi tiếp | 1-3h chờ | TTS bị block khi mentor bận |

```text
CURRENT STATE — 5 bước, ~50 phút/ngày/mentor (cao điểm tuần 1)

[1 TTS hỏi]
→ [2 Phân loại: 1']
→ [3 Tìm tài liệu đúng + còn hiệu lực: 5-10']  <-- bottleneck
→ [4 Soạn trả lời + link: 3']
→ [5 Trả lời / hỏi tiếp]  (TTS chờ 1-3h)
```

Bottleneck chính:

```text
Bước 3 — tìm lại thông tin đúng VÀ còn hiệu lực giữa Notion/Confluence/Slack/Drive.
Mentor là điểm nghẽn duy nhất vì chỉ họ biết "cái gì nằm ở đâu và cái gì còn đúng".
```

### 5.2 — Future workflow

```text
FUTURE STATE — câu đã có tài liệu trả gần như tức thì

ĐIỀU KIỆN NỀN (làm trước khi bật bot):
[0 Làm sạch + gán owner cho doc 3 chủ đề lặp nhất:
    setup môi trường, git workflow, xin quyền truy cập]  -- Rule/người

[1 TTS hỏi trong channel]
→ [2 Bot retrieve từ KB đã index (nhiều nguồn)]      -- Workflow step
→ [3 Bot draft trả lời KÈM TRÍCH NGUỒN]              -- Workflow step
→ [4 Cổng tự tin:
      4a đủ tự tin + có nguồn → trả lời TTS ngay
      4b không chắc / câu nhạy cảm (lương, nghỉ phép, cấp quyền)
         → escalate cho mentor/HR]                   -- Human boundary
→ [5 Mentor review log câu sai hằng tuần → cập nhật KB]  -- Human-in-the-loop

Fallback:
- Bot không có nguồn → trả "mình chưa chắc, đã chuyển cho mentor", KHÔNG bịa.
- Nếu tỉ lệ sai cao → tắt auto-answer, để bot chỉ gợi ý link cho mentor.

Bottleneck mới: bước 0 (làm sạch tài liệu) + bước 5 (verify) —
đây là bottleneck CHẤP NHẬN ĐƯỢC vì là điểm kiểm soát chất lượng.
```

Before/after impact:

| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| Số bước (phía mentor) | 5 | 2 (escalate + verify) | Mentor chỉ chạm câu khó/nhạy cảm |
| Thời gian mentor/ngày | ~50' | < 20' | Target chính |
| Thời gian TTS chờ (câu có tài liệu) | 1-3h | < 15' | Bot trả ngay |
| % câu lặp mentor phải tự trả lời | ~60% | < 30% | Bot gánh câu factual |
| Risk mới | Không có hallucination | Có hallucination + rủi ro nguồn lỗi thời | Bắt buộc trích nguồn + verify log |

### 5.3 — Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Mentor phụ trách onboarding TTS; TTS là người bị block. |
| **Workflow** | TTS hỏi → mentor phân loại → tìm tài liệu đúng/còn hiệu lực → soạn trả lời → trả lời. |
| **Bottleneck** | Tìm lại tài liệu đúng và còn hiệu lực giữa 4 nguồn rải rác, một số lỗi thời. |
| **Impact** | ~50 phút/ngày/mentor trong 2 tuần đầu; TTS chờ 1-3h/câu; onboarding chậm. |
| **Success Metric** | Mentor < 20 phút/ngày; TTS chờ < 15 phút cho câu đã có tài liệu; không tăng số câu trả lời sai phải đính chính. |
| **Boundary** | Bot không tự cấp quyền, không quyết định chính sách (lương/nghỉ phép); chỉ trả lời từ nguồn đã duyệt, kèm trích nguồn; không bịa. |

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0 — Vị trí trên ma trận

Bài toán nằm ở ô:

```text
Độ phức tạp: trung bình-cao (3+ nguồn dữ liệu, retrieve + trả lời + cổng tự tin).
Độ mơ hồ: trung bình (đa số câu có đáp án đúng/sai rõ; một số cần ngữ cảnh).
→ Ô "phức tạp cao × mơ hồ thấp-vừa": Workflow điều phối nhiều bước rõ ràng, CHƯA cần Agent.
```

Vì sao:

```text
- Output phần lớn có đúng/sai rõ (factual onboarding) → mơ hồ không cao.
- Cần gom 3+ nguồn + bước retrieve→draft→escalate → phức tạp đủ để cần workflow, không chỉ 1 rule.
- AI KHÔNG cần tự quyết bước tiếp theo hay tự gọi công cụ ngoài → chưa cần Agent.
```

### 6.1 — So sánh Rule / Workflow / Agent

| Mức | Phương án cho bài toán | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | FAQ bot khớp keyword + canned answers + checklist | Đủ cho ~30-40% câu cố định, diễn đạt chuẩn | Không hiểu biến thể ngôn ngữ; cứng nhắc; vẫn cần người cập nhật | Dùng cho lớp đáy (FAQ chắc chắn), không đủ cho toàn bộ |
| **Workflow** | RAG Q&A: retrieve KB → draft trả lời kèm trích nguồn → cổng tự tin → escalate; mentor verify log | Hợp vì các bước tuyến tính, AI chỉ hỗ trợ retrieve + diễn đạt | Hallucination, nguồn lỗi thời, low-confidence routing chưa chuẩn | **Chọn** |
| **Agent** | Bot tự quyết, tự hành động: tự cấp quyền, tự tạo ticket, tự sửa doc | Chỉ cần nếu phải tự lập kế hoạch nhiều nhánh + gọi nhiều tool có side-effect | Quá rộng; nhiều permission; side-effect nguy hiểm (cấp nhầm quyền) | Chưa chọn |

Mức chọn:

```text
Workflow (có lớp Rule cho FAQ đáy).
```

Vì sao chọn:

```text
- Retrieve nhiều nguồn + diễn đạt tự nhiên cần AI, vượt khả năng của Rule thuần.
- Các bước cố định, tuyến tính → workflow đủ, dễ kiểm soát.
- Có cổng tự tin + escalate + verify → risk nằm trong tầm kiểm soát.
```

Vì sao không chọn mức đơn giản hơn (Rule) — và không chọn mức cao hơn (Agent):

```text
- Rule thuần bỏ sót ~60% câu hỏi diễn đạt biến thể → không đạt metric.
- Agent thừa: không cần tự lập kế hoạch động; các hành động có side-effect (cấp quyền)
  PHẢI do người quyết. Lên Agent chỉ tăng rủi ro mà không tăng giá trị ở giai đoạn này.
```

### 6.2 — Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Mentor phụ trách onboarding TTS; TTS bị block. |
| **Workflow** | TTS hỏi → phân loại → tìm tài liệu đúng/còn hiệu lực → soạn trả lời → trả lời. |
| **Bottleneck** | Tìm lại tài liệu đúng và còn hiệu lực giữa 4 nguồn rải rác, một số lỗi thời. |
| **Impact** | ~50 phút/ngày/mentor (2 tuần đầu); TTS chờ 1-3h/câu; onboarding chậm. |
| **Success Metric** | Mentor < 20 phút/ngày; TTS chờ < 15 phút (câu có tài liệu); % câu lặp mentor tự trả lời < 30%; không tăng số trả lời sai phải đính chính. |
| **Boundary** | Bot không tự cấp quyền, không quyết chính sách; chỉ trả lời từ nguồn đã duyệt + trích nguồn; câu nhạy cảm/không chắc → escalate. |
| **AI intervention point** | Sau khi câu hỏi vào channel, trước khi mentor phải đọc và tìm tài liệu — bot retrieve + draft kèm nguồn. |
| **Mức chọn** | Workflow (RAG Q&A) + lớp Rule cho FAQ đáy. |
| **Rủi ro & người thật kiểm tra** | Risk: hallucination, nguồn lỗi thời, escalate sai ngưỡng. Người thật: mentor verify log hằng tuần + duyệt câu nhạy cảm; owner doc giữ KB tươi. |

### 6.3 — Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú |
|---|---|---|
| Actor và workflow đã rõ chưa? | Yes | Mentor + TTS, workflow 5 bước rõ |
| Baseline và success metric đã đo được chưa? | Yes | Có baseline ~50'/ngày từ 2 đợt; sẽ log lại 1 đợt để xác nhận |
| Có data/input đủ dùng chưa? | **Not Yet** | Tài liệu 3 chủ đề lặp nhất cần làm sạch + gán owner trước |
| Nếu AI sai, hậu quả có chấp nhận được không? | Yes (có điều kiện) | Câu factual: thấp; câu nhạy cảm escalate → không để bot quyết |
| Có người review/owner vận hành không? | Yes | Mentor verify log + owner doc |
| Có cách non-AI đơn giản hơn không? | Một phần | FAQ/checklist gánh đáy, nhưng không đủ cho câu biến thể |

Decision:

```text
Go — với scope nhỏ VÀ điều kiện tiên quyết.
```

Lý do:

```text
Problem, workflow, metric rõ; AI nằm ở một bước cụ thể (retrieve + draft) với human boundary
rõ ràng. Nhưng validation cho thấy nguồn lỗi thời là rủi ro thật → Go có điều kiện, không Go mù.
```

Nếu Go, pilot nhỏ nhất:

```text
- Điều kiện tiên quyết: làm sạch + gán owner cho doc 3 chủ đề lặp nhất
  (setup môi trường, git workflow, xin quyền truy cập).
- Index 3 chủ đề đó vào 1 RAG bot trong channel onboarding.
- Chạy 1 đợt onboarding (2 tuần): bot trả lời kèm trích nguồn, escalate khi không chắc.
- Đo: thời gian mentor/ngày, thời gian chờ TTS, % câu bot trả đúng, số câu phải đính chính.
```

Nếu Not Yet (cho phần còn lại):

```text
Các chủ đề ngoài 3 chủ đề trên: chưa bật bot cho đến khi doc được làm sạch và có owner.
```

Nếu No-Go (cho nhánh Agent):

```text
Không làm agent tự cấp quyền/tự sửa doc. Thay vào đó giữ con người quyết các hành động
có side-effect; bot chỉ trả lời và gợi ý.
```

---

## File nộp kèm

```text
02-group-problem-statement-workflow.md         (before/after ASCII — đã nhúng ở mục 5.1, 5.2)
02-group-problem-statement-research-notes.md   (chi tiết research mục 4.2)
```
