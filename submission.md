# Day 16 Submission 
## Name and student ID
- Hoàng Đức Nghĩa - 2A202600371
---
## 1. Idea reframed
Original idea:
> Xây dựng một chatbot AI hỗ trợ trả lời câu hỏi tuyển sinh 24/7 cho các trường đại học mới mở
Reframed as a product opportunity:
> Các phòng tuyển sinh tại các trường đại học mới mở đang gặp vấn đề nghiêm trọng với việc xử lý khối lượng lớn câu hỏi từ học sinh do không có nhiều resource như các trường đại học nổi tiếng hơn, dẫn đến thời gian phản hồi chậm và mất đi nhiều ứng viên tiềm năng. Các giải pháp hiện tại như FAQ hoặc chatbot rule-based không đủ khả năng xử lý các câu hỏi mang tính cá nhân hóa. Chúng tôi tin rằng nếu có thể kết nối AI trực tiếp với dữ liệu hồ sơ và quy trình tuyển sinh, hệ thống có thể cung cấp câu trả lời chính xác theo ngữ cảnh từng học sinh. Điều này giúp giảm tải cho nhân viên tuyển sinh và tăng tỷ lệ chuyển đổi từ quan tâm sang nộp hồ sơ.
---
## 2. Customer / Segment Card
- **Segment name:** Hệ thống tuyển sinh thông minh cho trường đại học mới mở
- **Operational context:** Trong mùa tuyển sinh thì số lượng học sinh muốn tìm hiểu về trường là rất đông nhưng nếu muốn hỏi thông tin thì phản hồi vẫn đang bị chờ lâu
- **Recurring workflow:** Học sinh hỏi một câu hỏi -> phòng tuyển sinh cho vào danh sách chờ -> phòng tuyển sinh đi đến câu hỏi đó -> phòng tuyển sinh đọc câu hỏi -> phòng tuyển sinh đi tìm thông tin liên quan và viết câu trả lời -> Học sinh nhận được câu trả lời
- **Pain moment:** Học sinh muốn hỏi một câu hỏi, nhưng phải mất rất lâu thì mới có câu trả lời -> sinh viên tốn nhiều thời gian tìm hiểu trường và vì mùa tuyển sinh ngắn nên sinh viên dễ bỏ cuộc tìm hiểu về trường và không nộp đơn vào trường nữa
- **Why now:** Với số lượng các trường đại học ngày càng tăng lên nên các trường đại học mới mở càng phải tìm cách attract sinh viên muốn tìm hiểu ứng tuyển vào trường. Vì thế nên, nếu sinh viên thấy chán nản trước việc phản hồi bị chậm thì sinh viễn dễ bỏ tìm hiểu về trường và tìm hiểu, ứng tuyển vào trường khác, nổi tiếng hơn. Dẫn đến việc các trường đại học mới không có nhiều sinh viên ứng tuyển và vẫn cứ obscure; và hậu quả là không phát triển được. Vậy nên các trường đại học cần tìm cách handle số lượng lớn câu hỏi của học sinh để giữ interest của họ.
- **Access path:** Liên hệ với trưởng phòng tuyển sinh các trường đại học để họ ứng dụng phương pháp này để giảm workload cho họ
One-sentence description:
> Phòng tuyển sinh tại các trường đại học tư thục mới mở, đang phải xử lý hàng trăm câu hỏi của học sinh mỗi ngày với nguồn lực hạn chế.
---
## 3. Need Map (2–3 needs)
### Need #1 (priority)
- **Statement (JTBD):** Khi hạn chót nộp hồ sơ đến gần và lượng email/cuộc gọi của học sinh tăng đột biến, tôi muốn có thể giải đáp ngay lập tức và chính xác các câu hỏi thường gặp, để tôi có thể ngăn chặn tình trạng tồn đọng email và tập trung thời gian vào việc đánh giá các hồ sơ thực sự cần cân nhắc kỹ.
- **Current workaround:** Copy-paste các câu trả lời mẫu từ một tài liệu chung, tạo các trang FAQ tĩnh, và thuê sinh viên làm thêm thời vụ để xử lý các câu hỏi cơ bản.
- **Pain signal:** Nhân viên tuyển sinh kiệt sức, thời gian phản hồi email bị trễ từ 48 đến 72 giờ trong những tuần cao điểm, và sự thất vọng của học sinh dẫn đến việc bỏ dở tìm hiểu và không muốn ứng tuyển vào trường nữa.
- **Evidence / proxy evidence:** Các văn phòng tuyển sinh thường xuyên ghi nhận hàng trăm email chưa đọc trong hộp thư chung vào những tuần quanh hạn chót nộp hồ sơ. Số lượng hồ sơ ứng tuyển vào trường thấp đáng kể hơn so với dự tính.
- **Why underserved:** Tính năng trả lời tự động của các hệ thống CRM hiện tại quá cứng nhắc và rập khuôn. Chúng không thể hiểu bối cảnh cụ thể của từng học sinh hoặc tự động trích xuất trạng thái giấy tờ còn thiếu mà không có sự can thiệp của con người.
### Need #2
- **Statement (JTBD):** Khi học sinh hỏi những câu hỏi phức tạp, mang tính cá nhân hóa về trạng thái hồ sơ hoặc nền tảng giáo dục riêng của họ, tôi muốn có thể ngay lập tức cung cấp cho họ câu trả lời chính xác, được cá nhân hóa mà không cần nhân viên can thiệp thủ công, để tôi có thể ngăn họ tiếp tục gửi email/gọi điện khiếu nại và giảm thiểu khối lượng lớn các yêu cầu hỗ trợ thủ công đang tồn đọng,.
- **Current workaround:** Sử dụng các chatbot theo quy tắc tiêu chuẩn, vốn chỉ đưa ra các đường link FAQ chung chung, khiến học sinh bức xúc và bắt buộc phải gửi email trực tiếp cho phòng tuyển sinh. Sau đó, nhân viên phải tự mở CRM thủ công, tra cứu hồ sơ riêng của học sinh và tự gõ câu trả lời tùy chỉnh.
- **Pain signal:** Khối lượng lớn email "cấp độ 2" (tier 2) mà các bot tiêu chuẩn không thể xử lý được, khiến nhân viên tuyển sinh tốn thêm 3-5 phút cho mỗi email chỉ để tìm lại ngữ cảnh hồ sơ của học sinh, dẫn đến thời gian chờ đợi kéo dài.
- **Evidence / proxy evidence:** Phân tích dữ liệu từ cổng thông tin (Portal analytics) cho thấy chatbot hiện tại có tỷ lệ học sinh yêu cầu "chuyển sang nhân viên hỗ trợ" (escalate to human) hoặc tỷ lệ bỏ ngang rất cao; hộp thư chung của phòng tuyển sinh luôn tràn ngập các câu hỏi đặc thù mà các trang FAQ tiêu chuẩn không bao quát được.
- **Why underserved:** Các chatbot và tính năng trả lời tự động trên CRM truyền thống không có khả năng kết nối động (dynamically connect) với cơ sở dữ liệu hồ sơ của học sinh để tự động tổng hợp thông tin và đưa ra một câu trả lời hiểu rõ ngữ cảnh cá nhân của ứng viên.

---
## 4. Strategy Statement
For phòng tuyển sinh của các trường đại học tư thục mới mở từ 5 năm trở xuống, có CRM nhưng chưa tự động hóa phản hồi
who struggle with việc xử lý khối lượng lớn câu hỏi từ học sinh với tốc độ chậm và thiếu cá nhân hóa
our product helps them giảm backlog hàng trăm email và thời gian phản hồi của các câu hỏi từ 48–72h xuống còn vài giây và tránh mất interest của các sinh viên tiềm năng do chờ đợi
through một hệ thống AI kết nối trực tiếp với CRM tuyển sinh để truy xuất trạng thái hồ sơ theo thời gian thực, sau đó dùng RAG để tổng hợp quy định tuyển sinh và generate câu trả lời cá nhân hóa
unlike các chatbot rule-based hoặc FAQ tĩnh và hệ thống CRM truyền thống
because we can leverage dữ liệu hồ sơ học sinh theo thời gian thực, lịch sử tương tác, và khả năng hiểu ngữ cảnh để tạo ra câu trả lời linh hoạt và cá nhân hóa.
---
## 5. Moat Hypothesis
**Moat mechanism:** dataset hội thoại tuyển sinh + mapping giữa câu hỏi và trạng thái hồ sơ thực tế của học sinh, được tích lũy qua từng mùa tuyển sinh và gắn chặt với CRM nội bộ của từng trường
(ví dụ: domain-learning flywheel, data compounding, workflow embedding...)
If we deploy 50 times in the same vertical,
the following things get systematically better:
1. Độ chính xác của câu trả lời tăng lên nhờ học từ hàng triệu câu hỏi tuyển sinh thực tế
2. Khả năng hiểu intent và các edge-case trong tuyển sinh (thiếu giấy tờ, deadline, điều kiện đặc biệt) được cải thiện mạnh
3. Dataset về hành vi học sinh (hỏi gì trước khi apply, drop ở đâu) giúp tối ưu funnel tuyển sinh cho từng trường
Why competitors cannot easily replicate this:
> Vì hệ thống tích lũy dữ liệu interaction thực tế + tích hợp sâu vào workflow nội bộ của từng trường (CRM, hồ sơ, quy trình xét tuyển), tạo ra lợi thế dữ liệu và chi phí chuyển đổi rất cao.

---
## 6. Initial TAM / SAM / SOM view
| Layer | Estimate                               | Key assumptions                                                                                          | Confidence |
| ----- | -------------------------------------- | -------------------------------------------------------------------------------------------------------- | ---------- |
| TAM   | ~3 – 12 tỷ VND / năm                   |  khoảng 240 trường ĐH tại Việt Nam; 40%–70% có nhu cầu automation tuyển sinh; pricing 30–70M/năm            | low        |
| SAM   | ~120M – 700M VND / năm                 | Giới hạn: trường tư thục, mới mở ≤5 năm, có CRM nhưng chưa automation; ước tính còn ~4–10 trường phù hợp | low        |
| SOM   | ~30M – 280M VND / năm (1–4 khách hàng) | Có thể chốt ~20%–40% SAM trong 12–18 tháng; sales cycle B2B giáo dục chậm                                | low        |
**Top 3 unknowns requiring further research:**
1. Các trường có thực sự sẵn sàng chi 30–70M/năm cho bài toán này hay không (budget + willingness to pay)
2. Mức độ ảnh hưởng của việc phản hồi chậm (48–72h) tới tỷ lệ nộp hồ sơ thực tế
3. Khả năng tích hợp CRM hiện tại (API, chất lượng dữ liệu, chi phí triển khai thực tế)
**Judgment:**
- [ ] Worth pursuing now
- [x] Worth pursuing but not now (need to validate willingness to pay + expand market scope ngoài trường mới tại Việt Nam)
- [ ] Not worth pursuing as currently framed
---
## 7. Positioning Note (2 sentences)
**What we are:**
> Một hệ thống AI tuyển sinh thông minh giúp tự động hóa và cá nhân hóa toàn bộ quá trình tư vấn ứng tuyển cho học sinh
**What we are not / not yet:**
> Không chỉ là một chatbot FAQ hay công cụ trả lời tự động đơn giản, và chưa phải là một hệ thống thay thế hoàn toàn quyết định tuyển sinh của con người
---
## 8. Self-assessment before Day 17
Trong 6 mắt xích (Idea Customer Need Strategy Moat Market Size), mắt xích nà
> Market Size là mắt xích yếu nhất, vì segment hiện tại quá hẹp do chỉ tập trung vào trường mới tại Việt Nam, dẫn đến TAM/SAM nhỏ và khó scale thành một startup lớn.
Open questions chúng tôi muốn khám phá thêm ở Day 17:
1. Các trường đại học sẵn sàng chi bao nhiêu tiền mỗi năm cho hệ thống tuyển sinh thông minh này và cần đặt mức giá là bao nhiêu ?
2. Việc giảm thời gian phản hồi có thực sự làm tăng tỷ lệ nộp hồ sơ không, hay chỉ cải thiện trải nghiệm?
3. Hệ thống CRM của các trường hiện tại có đủ khả năng tích hợp (API, dữ liệu sạch) để triển khai solution này một cách thực tế không?
