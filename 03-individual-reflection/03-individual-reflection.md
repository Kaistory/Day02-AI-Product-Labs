# 03 — Individual Reflection

> Phần cá nhân của **Khải**. Viết bằng trải nghiệm thật của mình, không để AI viết thay.
>
> Lưu ý: tôi làm lab này **một mình**, nên phần "vai trò trong nhóm" tôi điều chỉnh trung thực thành cách tôi tự đóng vai trò người phản biện cho chính mình và dùng AI + phỏng vấn người ngoài thay cho việc nhóm challenge.

## Tôi đã làm gì ở từng phase?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Liệt kê 10 problems theo 4 lăng kính | Có nhiều candidate ở cluster hỏi-đáp lặp |
| Chọn top 3 + Problem Card | Viết Card #1 chi tiết + draft workflow trước/sau | Bài chính để đào sâu |
| Tự pitch + tự challenge | Viết 3 câu hỏi chống lại lựa chọn của chính mình | Lộ ra rủi ro "tài liệu lỗi thời" |
| Convergence | Cluster 10 problems → shortlist → score → chọn 1 | Chọn onboarding Q&A có lý do rõ |
| Validation | Phỏng vấn 3 mentor + 4 TTS, poll 8 người | Phát hiện lớp pain thứ 2 (nguồn lỗi thời) |
| Research | Tìm Notion AI, Confluence AI, Glean, Guru, Slack AI | Thấy không cần build agent từ đầu |
| Workflow | Vẽ current/future + thêm bước 0 làm sạch doc | Workflow bản cuối |
| Problem Statement | Soạn metric đo được + boundary cụ thể | PS v0 → v1 |
| Rule / Workflow / Agent | Lập luận chọn Workflow, không lên Agent | Quyết định nhất quán |
| Decision | Chốt "Go có điều kiện" | Quyết định cuối |

## Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình |
|---|---|---|---|---|
| Scan | Gợi ý thêm problem theo role mentor | Nhắc tôi 2 ý (#8 checklist, #10 feedback cuối kỳ) | Gợi ý "trợ lý AI nội bộ toàn năng" quá rộng | Bỏ ý quá rộng, chỉ giữ ý có workflow thật |
| Problem Card | Đóng vai skeptical PM phản biện | Chỉ ra metric "trả lời đủ đúng" mơ hồ | Không tự thấy rủi ro tài liệu lỗi thời cho đến khi tôi mô tả kỹ | Thêm 2 câu challenge và làm rõ metric đo được |
| Convergence | Hỏi AI tìm lỗ hổng trong lựa chọn của tôi | Đóng vai "người ngoài" challenge thay nhóm | Có lúc đồng ý quá dễ với tôi | Tự ép thêm tiêu chí "so sánh R/W/A được" để loại code review |
| Workflow | Nhờ chuyển mô tả thành sơ đồ | Vẽ nhanh các bước | Gộp bước "làm sạch doc" vào "index" | Tách bước 0 ra vì đó là điều kiện tiên quyết |
| Research | Tìm tool tương tự | Gợi ý Notion AI, Confluence AI, Glean, Guru, Slack AI | Đưa vài con số "tiết kiệm X%" không có nguồn | Bỏ số liệu không verify; chỉ giữ link tài liệu chính thức |
| Problem Statement | Nhờ phản biện field mơ hồ | Chỉ ra boundary chưa nói rõ câu nhạy cảm | Đề xuất nhảy lên Agent | Giữ ở Workflow; thêm boundary "không tự cấp quyền" |
| Decision | Không dùng AI | — | — | Tự chốt "Go có điều kiện" |

## Reflection (câu hỏi mở)

```text
Khó nhất khi làm một mình là không có ai challenge mình. Rất dễ tự thuyết phục rằng lựa chọn
đầu tiên của mình là đúng. Tôi xử lý bằng cách tự đóng hai vai — vai đề xuất và vai phản biện —
và viết ra 3 câu hỏi chống lại chính mình trước khi đào sâu. Nhưng tôi nhận ra tự challenge vẫn
có giới hạn: tôi và AI đều không nghĩ ra rủi ro "tài liệu lỗi thời" cho tới khi một mentor nói
thẳng trong lúc phỏng vấn. Đó là lần "người ngoài" thật sự bẻ lại tư duy của tôi, và nó đổi cả
quyết định cuối: tôi thêm bước 0 (làm sạch + gán owner doc) và chuyển từ "Go" sang "Go có điều
kiện".

Tôi cũng suýt bị solution-first: lúc đầu tôi hào hứng nghĩ ngay đến một con bot agent tự động trả
lời mọi thứ. Khi tự hỏi "nếu agent tự cấp quyền mà cấp nhầm thì ai chịu?", tôi mới quay về Workflow
+ boundary. Câu hỏi đó đến từ việc vẽ workflow chứ không phải từ việc nghĩ về AI.

Đóng góp thật của tôi vào artifact cuối là baseline thời gian (từ 2 đợt onboarding tôi từng kèm),
workflow before/after, và việc đẩy metric từ "nhanh hơn" thành con số đo được. Tôi đã đổi ý sau khi
nghe TTS nói họ ngại hỏi nên tự đoán: ban đầu metric của tôi chỉ là "giảm thời gian mentor", sau đó
tôi thêm "thời gian chờ của TTS" vì pain của họ mới là phần bị giấu.

Điều khó nhất khi viết Problem Statement là boundary: dễ viết chung chung "AI hỗ trợ thôi", nhưng
khó ở chỗ phải nói cụ thể bot KHÔNG được làm gì (cấp quyền, quyết chính sách) và câu nào phải
escalate. Viết được boundary cụ thể mới thấy vì sao Workflow đủ và Agent là thừa.
```

## Bài học của tôi

- Problem tốt không phải problem nghe "AI" nhất, mà là problem có workflow, baseline và metric rõ.
- Làm một mình thì validation rẻ (vài cuộc phỏng vấn) là cách tốt nhất để có người ngoài challenge — nó đổi cả quyết định cuối của tôi.
- Với hỏi-đáp từ tài liệu, "chất lượng nguồn" quan trọng ngang "chất lượng model". AI khuếch đại cả cái đúng lẫn cái sai trong KB.
- Agent không phải đích đến mặc định. Khi hành động có side-effect (cấp quyền), người phải giữ quyền quyết.

Nếu làm lại:

```text
Tôi sẽ log câu hỏi thật trong 1 tuần TRƯỚC khi làm bài để có dữ liệu phân loại lặp/không lặp chính
xác, thay vì ước lượng "60% lặp" từ trí nhớ. Và vì làm một mình, tôi sẽ chủ động tìm thêm 1-2 người
phản biện thật sớm hơn — tự challenge có giới hạn, người ngoài mới thấy điểm mù như "tài liệu lỗi
thời".
```

## Tự kiểm hiểu bài — mạch problem → workflow → metric → boundary → độ phù hợp với AI

```text
Problem: mentor mất ~50'/ngày trả lời câu onboarding lặp, TTS chờ 1-3h, vì tài liệu rải rác/lỗi thời.
→ Workflow: bottleneck ở bước tìm tài liệu đúng & còn hiệu lực; future workflow đưa AI vào retrieve+draft
  kèm trích nguồn, escalate khi không chắc, người verify.
→ Metric: mentor <20'/ngày, TTS chờ <15', câu lặp mentor tự trả <30%, không tăng câu sai phải đính chính.
→ Boundary: bot không cấp quyền, không quyết chính sách, chỉ trả từ nguồn đã duyệt + trích nguồn.
→ Độ phù hợp AI: Workflow (không phải Agent) vì các bước cố định, mơ hồ thấp-vừa, và mọi hành động
  có side-effect đều do người quyết. Decision: Go có điều kiện (làm sạch doc 3 chủ đề trước, pilot 1 đợt).
```
