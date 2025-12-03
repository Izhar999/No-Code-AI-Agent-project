# 🚀 No-Code AI Agent using n8n  
A fully automated **No-Code AI Agent** built using **n8n**, OpenRouter AI models, OpenChat (Public Chat), and Google Sheets — all without writing a single line of code.

---

## ✨ Project Overview
This project demonstrates how to combine **AI + automation** to create an intelligent workflow that can:
- Run an AI chatbot using OpenRouter models  
- Make the chat **publicly accessible** using OpenChat  
- Log messages & interactions inside **Google Sheets**  
- Execute actions automatically with **zero code**

Everything is built visually inside n8n.

---

## 🔧 Features
- 🔹 **Public AI Chat** using OpenChat  
- 🔹 **OpenRouter AI models** for smart responses  
- 🔹 **Google Sheets integration** for data logging  
- 🔹 **Fully visual, no coding required**  
- 🔹 **Reusable workflow** for automation, bots, support systems, lead capture, etc.

---

## 🏗️ Architecture

### **High-Level Flow**
1. **User sends a message** to the public AI chat  
2. **OpenChat API** forwards the message to n8n  
3. **n8n workflow** processes the text  
4. **OpenRouter model** generates AI response  
5. **n8n logs data** to Google Sheets  
6. **Response is sent back** to the user via OpenChat  
7. (Optional) n8n triggers other automations based on intent

---

## 📊 Workflow Diagram

```mermaid
flowchart LR
    A[User Message<br> via OpenChat] --> B[n8n Webhook Trigger]
    B --> C[Process Message]
    C --> D[Send to OpenRouter AI Model]
    D --> E[Receive AI Response]
    E --> F[Log to Google Sheets]
    F --> G[Send Response Back to OpenChat]
