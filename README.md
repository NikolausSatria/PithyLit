# 🚀 PithyLit: PDF Summarizer for Academic Papers

**Transform Lengthy Research Papers into Concise Insights**  
*Powered by Local AI (Ollama + deepseek-r1) • Built with T3 Stack*

---

## 📌 Overview
**PithyLit** is an open-source tool designed to summarize academic PDF articles using local AI. Built with:
- **Frontend**: Next.js (T3 Stack) + TypeScript + Tailwind CSS  
- **Backend**: tRPC + Prisma ORM  
- **Database**: PostgreSQL  
- **AI Engine**: Ollama with the `deepseek-r1` model (no cloud dependencies!)  

🔗 [Demo](#) | 💻 [My Portfolio](#)  


---

## ✨ Features
- 📤 **PDF Upload** with drag-and-drop functionality
- 🧠 **AI-Powered Summarization** (Ollama + deepseek-r1)
- 🗃️ **Summary History** (Stored in PostgreSQL)
- 🔍 **Key Point Highlighting** from articles
- 🛡️ 100% Privacy (AI runs locally)
- ⚡ Responsive & Dark Mode Support

---

## 🛠️ Tech Stack
| Category       | Technologies                                                                                     |
|----------------|--------------------------------------------------------------------------------------------------|
| **Frontend**   | ![Next.js](https://img.shields.io/badge/Next.js-000?style=flat&logo=next.js&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat&logo=tailwindcss) |
| **Backend**    | ![tRPC](https://img.shields.io/badge/tRPC-2596BE?style=flat&logo=trpc&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white) |
| **Database**   | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) |
| **AI**         | ![Ollama](https://img.shields.io/badge/Ollama-FF6C37?style=flat&logo=ollama&logoColor=white) `deepseek-r1` |
| **Tools**      | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) ![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=flat&logo=eslint) |

---

## 🛠️ Installation
**Prerequisites**:  
- Node.js v18+
- PostgreSQL
- Ollama (installed & `deepseek-r1` model downloaded)

```bash
# Clone repository
git clone https://github.com/NikolausSatria/PithyLit.git
cd pithylit

# Install dependencies
npm install

# Setup database
npx prisma generate
npx prisma migrate dev

# Run Ollama (in a separate terminal)
ollama serve

# Start the application
npm run dev