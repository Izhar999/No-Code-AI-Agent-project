# 🚀 No-Code AI Agent using n8n  
Build a fully automated **AI Agent** using **n8n**, OpenRouter LLMs, Hosted Chat, and Google Sheets — all without writing code.

This project creates a **public AI chatbot** capable of:
- Reading tasks from Google Sheets  
- Adding or updating tasks  
- Answering questions naturally  
- Prioritizing work  
- Acting as a personal task assistant  

---

## 🌟 Features
- 🔹 **Public AI Chat Interface** (Hosted Chat)
- 🔹 **OpenRouter LLM integration**
- 🔹 **Google Sheets read/write**
- 🔹 **Memory-enabled AI assistant**
- 🔹 **No coding required**
- 🔹 Fully visual drag-and-drop automation in n8n

---

## 🧩 Architecture Diagram (Mermaid)

```mermaid
flowchart LR
    A[User → Hosted Chat] --> B[Webhook Trigger]
    B --> C[AI Agent Node]
    C --> D[OpenRouter Chat Model]
    C --> E[Simple Memory]
    C --> F[Google Sheets - Read]
    C --> G[Google Sheets - Append/Update]
    D --> C
    F --> C
    G --> C
    C --> H[Return Response to Chat]
