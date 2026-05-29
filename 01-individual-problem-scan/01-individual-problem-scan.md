# 01 — Individual Problem Scan

> Phần cá nhân. Tác giả: **Khải** — junior developer, vừa qua kỳ thực tập 3 tháng và nay được giao kèm 1-2 thực tập sinh (TTS) mới mỗi đợt tại một công ty công nghệ ~80 người.

Góc nhìn: tôi vừa là người *từng đau* khi mới onboard, vừa là người *đang đau* khi phải trả lời lại đúng những câu mình từng hỏi.

---

## Phase 1 — Scan rộng (10 problems)

Tôi scan 10 problems từ trải nghiệm thật trong 3 tháng thực tập + 2 đợt kèm TTS, vượt mức tối thiểu 5.

| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Pain từ người khác / Lặp lại | TTS mới hỏi lại các câu quy trình giống hệt nhau (setup môi trường, tạo branch/PR, xin quyền truy cập) | Mentor, TTS | Mỗi đợt onboarding mentor trả lời ~50 phút/ngày trong 2 tuần đầu; ~60% câu là lặp lại |
| 2 | Tốn thời gian | Tìm lại tài liệu đúng và còn hiệu lực giữa Notion, Confluence, Slack pinned, Drive | Mentor, TTS | 5-10 phút/lần tìm; một số doc đã lỗi thời nhưng vẫn còn |
| 3 | Lặp lại | TTS bị block chờ mentor rảnh mới trả lời được | TTS | Chờ trung bình 1-3 giờ/câu, có khi qua hôm sau |
| 4 | Tốn thời gian | Viết weekly update của TTS gửi mentor, mỗi người một format | TTS, mentor | 20-30 phút/tuần, khó so sánh tiến độ |
| 5 | AI có thể tốt hơn | Code review comment lặp lại các lỗi quy ước (naming, lint, commit message) | Reviewer, TTS | 4-6 comment cùng loại mỗi PR của TTS |
| 6 | Pain từ người khác | TTS không biết hỏi ai cho từng đầu việc (HR / IT / tech lead) | TTS, nhiều phòng ban | Hỏi nhầm người, bị đẩy qua lại 2-3 lần |
| 7 | AI có thể tốt hơn | Search trong Confluence trả kết quả kém, không hiểu câu hỏi tự nhiên | Cả team | 10-15 phút/lần tìm tài liệu kỹ thuật |
| 8 | Tốn thời gian | Onboarding checklist theo dõi thủ công trên giấy/Sheet, dễ sót bước | Mentor | 1-2 bước bị quên mỗi đợt (VD: chưa cấp quyền repo) |
| 9 | Lặp lại | Trả lời cùng câu hỏi về quy định nghỉ phép / chấm công | HR, mentor, TTS | Vài lần/đợt; thông tin nằm trong PDF dài ít người đọc |
| 10 | AI có thể tốt hơn | Tổng hợp feedback cuối kỳ thực tập từ nhiều người để đánh giá | Mentor, manager | 1-2 giờ/TTS, mỗi quý |

Vì sao phần scan này ổn:

- Scan rộng (10) trước khi hội tụ.
- Dùng đủ 4 lăng kính.
- Mỗi problem có actor và dấu hiệu thật (thời gian, tần suất, hậu quả).
- Không bắt đầu bằng "xây chatbot AI" — bắt đầu từ workflow và bottleneck.

---

## Phase 2 — Top 3 Problem Cards

### Chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Câu hỏi onboarding lặp lại (#1 + #2 + #3) | Actor rõ, workflow lặp đều, có baseline thời gian, so sánh được Rule/Workflow/Agent | "Trả lời đủ đúng" đo thế nào; chất lượng tài liệu nguồn |
| 2 | Code review lỗi quy ước lặp (#5) | Pain thật, AI/linter có thể giúp | Phần lớn lỗi quy ước thực ra linter giải được — có cần AI không? |
| 3 | "Hỏi ai cho việc gì" (#6) | Nhiều người đau, scope rõ | Trùng một phần với #1; có thể chỉ là 1 chủ đề trong knowledge base |

---

### Problem Card #1 — Câu hỏi onboarding lặp lại

**Problem 1 câu:**
TTS mới liên tục hỏi lại cùng những câu hỏi quy trình, mentor mất ~50 phút/ngày trong 2 tuần đầu để tìm lại tài liệu rải rác và trả lời thủ công, còn TTS thì bị block chờ.

**Actor:**
Mentor (junior/senior dev) phụ trách kèm 1-2 TTS mỗi đợt; TTS là người bị block.

**Thời điểm / bối cảnh:**
2 tuần đầu mỗi đợt onboarding, cao điểm là tuần 1.

**Current workflow:**

```text
1. TTS gặp vướng → hỏi mentor qua Slack DM / channel
2. Mentor đọc câu hỏi, xác định thuộc chủ đề gì
3. Mentor tìm lại thông tin: Notion onboarding, Confluence, Slack pinned, Drive (đôi khi hỏi người khác)
4. Mentor soạn câu trả lời + dán link
5. Trả lời; nếu TTS chưa hiểu → quay lại bước 1
```

**Bottleneck:**
Bước 3 — tìm lại thông tin đúng và **còn hiệu lực**. Thông tin rải rác 4 nơi, một số đã lỗi thời, mentor là người duy nhất "biết tất cả nằm ở đâu".

**Impact:**
~50 phút/ngày/mentor × ~10 ngày làm việc = ~8 giờ/đợt/mentor. TTS chờ trung bình 1-3 giờ/câu → onboarding chậm. Mentor bị gián đoạn deep work nhiều lần/ngày.

**Success metric:**
Giảm thời gian mentor trả lời câu lặp từ ~50 phút/ngày xuống <20 phút/ngày; giảm thời gian chờ của TTS cho câu đã có tài liệu từ ~2 giờ xuống <15 phút; không làm tăng số câu trả lời sai phải đính chính.

**Non-AI alternative:**
FAQ doc + onboarding checklist + pinned canned answers. Giải quyết câu cố định nhưng không hiểu câu hỏi diễn đạt tự nhiên, vẫn cần người cập nhật, và TTS hay không chịu đọc doc dài.

**AI hypothesis:**
AI trả lời câu hỏi onboarding bằng cách retrieve từ knowledge base đã index (Notion/Confluence/Drive), trả lời **kèm trích nguồn**; câu nào không chắc/không có nguồn → escalate cho mentor.

**Quick gut:**
- [ ] No AI / process fix
- [ ] Rule
- [x] Workflow
- [ ] Agent
- [ ] Chưa biết

#### Draft current workflow

```text
CURRENT STATE — ~50 phút/ngày (cao điểm tuần 1)

[1 TTS hỏi]
→ [2 Mentor phân loại câu hỏi: 1']
→ [3 Tìm lại tài liệu đúng + còn hiệu lực: 5-10']  <-- bottleneck
→ [4 Soạn trả lời + dán link: 3']
→ [5 Trả lời / TTS hỏi tiếp]

Vấn đề: lặp ~60%; TTS chờ 1-3h vì mentor bận.
```

#### Draft future workflow

```text
FUTURE STATE — câu đã có tài liệu trả trong <15 phút (gần như tức thì)

[1 TTS hỏi trong channel]
→ [2 Bot retrieve từ KB đã index]
→ [3 Bot trả lời kèm trích nguồn — NẾU đủ tự tin]
→ [4a Đủ tự tin: TTS nhận trả lời ngay]
    [4b Không chắc / nhạy cảm: escalate cho mentor]  <-- human boundary
→ [5 Mentor review log sai định kỳ → cập nhật KB]

Fallback: bot không có nguồn → "mình chưa chắc, đã chuyển cho mentor",
không bao giờ tự bịa.
```

---

### Problem Cards #2 và #3 — tóm tắt

| Card | Actor | Bottleneck | Metric | Quick gut | Vì sao chưa chọn làm #1 |
|---|---|---|---|---|---|
| Code review lỗi quy ước (#5) | Reviewer, TTS | Comment lặp lại lỗi naming/lint/commit | 4-6 comment lặp/PR → ~0 | Rule (linter) | Phần lớn linter/pre-commit hook giải được — có thể không cần AI |
| "Hỏi ai cho việc gì" (#6) | TTS, nhiều phòng ban | Không biết owner từng đầu việc | Hỏi nhầm 2-3 lần → 0 | Workflow/Rule | Thực chất là 1 chủ đề con của knowledge base ở #1 |

---

## Card tôi muốn pitch nhất

```text
Problem Card #1 — Câu hỏi onboarding lặp lại.
```

Vì sao:

```text
Tôi vừa trải nghiệm cả hai phía: từng là TTS bị block, nay là mentor bị gián đoạn.
Workflow rõ, baseline thời gian đo được, và có thể so sánh thẳng Rule vs Workflow vs Agent.
Bottleneck (tìm lại tài liệu còn hiệu lực) là một bước cụ thể, không mơ hồ.
```

Câu hỏi tôi tự challenge (làm một mình nên tự đóng vai phản biện):

```text
1. Nếu phần lớn pain đến từ TÀI LIỆU LỖI THỜI thì AI có làm vấn đề tệ hơn không
   (trả lời tự tin nhưng từ nguồn sai)?
2. "Trả lời đủ đúng" đo bằng gì để không chỉ là cảm tính?
3. Một FAQ + checklist tốt đã đủ chưa, có cần đến AI không?
```

## Nếu dùng AI ở phase này

- **Scan:** sau khi tự liệt kê 6 problems, tôi hỏi Claude gợi ý thêm theo 4 lăng kính. AI gợi ý "tổng hợp feedback cuối kỳ" (#10) và "onboarding checklist thủ công" (#8) mà tôi chưa nghĩ tới → giữ lại. AI cũng gợi ý "xây trợ lý AI nội bộ toàn năng" → bỏ vì quá rộng, không phải workflow thật.
- **Phản biện Problem Card:** tôi nhờ AI đóng vai skeptical PM. Nó chỉ ra metric "trả lời đủ đúng" còn mơ hồ và cảnh báo rủi ro tài liệu lỗi thời → tôi thêm hai câu hỏi challenge ở trên và làm rõ metric.
