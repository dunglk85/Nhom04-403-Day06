# Prototype — AI Customer Support Agent (Xanh SM)

## Thông tin nhóm

- **Nhóm:** Nhóm 4
- **Track:** XanhSM

## Mô tả

Chatbot hỗ trợ khách hàng Xanh SM xử lý các yêu cầu lặp lại (khiếu nại tài xế, mất đồ, FAQ). Agent hỏi người dùng 2–4 câu để xác định intent, sau đó gợi ý giải pháp hoặc tạo ticket — kèm confidence. Người dùng chấp nhận hoặc yêu cầu hỗ trợ từ CSKH thật.

## Level: Mock prototype

- UI build bằng Claude Artifacts (HTML/CSS/JS)
- 3 flows chính chạy thật:
  1. Phân loại intent từ tin nhắn tiếng Việt → xác định loại yêu cầu (khiếu nại / mất đồ / FAQ)
  2. Hỏi làm rõ khi confidence thấp → bổ sung thông tin (mã chuyến, thời gian)
  3. Trả lời từ knowledge base (RAG) hoặc đề xuất tạo ticket

## Links

- Prototype: https://claude.site/artifacts/xxx
- Prompt test log: xem file `prototype/prompt-tests.md`
- Video demo (backup): https://drive.google.com/xxx

## Tools

| Layer | Tool | Ghi chú |
|-------|------|---------|
| UI | Claude Artifacts | HTML/CSS/JS |
| AI | Claude (Anthropic API) | System prompt + few-shot |
| Prompt | System prompt + few-shot examples | 10 intent phổ biến |

## Phân công

| Thành viên | Phần | Output |
|-----------|------|--------|
| Ngô Gia Bảo | Canvas + failure modes | `prototype/`, `spec/spec-final.md` phần 1 -> 4 |
| Nguyễn Dương Ninh | User stories 4 paths  | `spec/spec-final.md` phần 6, `demo/slides.pdf` |
| Lê Kim Dũng | UI prototype + demo script + prompt engineering | `prototype/`,`promptype-readme.md`, `spec/spec-final.md` phần 5|
