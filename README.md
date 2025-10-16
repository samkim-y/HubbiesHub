# 👫 HubbiesHub

**HubbiesHub** is a full-stack social + ML platform for husbands to connect, chat, and match based on shared interests.  
It’s built to practice **Software Engineering + ML Infrastructure**, featuring modern web tech and scalable backend design.

---

## 🌟 Features (MVP)
- 🪪 User Authentication (Sign up / Login / JWT Session)
- 👤 Profile Creation + Interest Tags
- 💬 Realtime 1-on-1 and Group Chat
- 🤝 Interest-based Matching via ML Embeddings
- 🗞️ Activity Feed / Posts
- 🧠 ML Service (API for matching + recommendations)

---

## 🧩 Tech Stack

| Layer | Tech |
|-------|------|
| Frontend | (React + TypeScript), TailwindCSS |
| Backend API | FastAPI (Python 3.11) + Socket.IO |
| Database | PostgreSQL |
| Cache / Queue | Redis (Upstash) |
| ML | Sentence-Transformers + FAISS / pgvector |
| DevOps | Docker + GitHub Actions + Vercel / Render |

---

## 🧠 ML Component (Planned)
- Generate sentence embeddings for each user’s interests using `all-MiniLM-L6-v2`
- Store vectors in pgvector / FAISS
- Compute similarity scores → match top N husbands with shared interests

---

## ⚙️ Local Setup
```bash
git clone https://github.com/<your-org>/hubbieshub.git
cd hubbieshub
docker-compose up --build
```

hubbieshub/
├── frontend/         # Next.js + TypeScript UI
├── backend/          # FastAPI + Socket.IO
│   ├── ml/           # ML model + matching service
│   ├── api/          # User / Chat / Match routes
│   └── db/           # ORM models (Postgres)
├── docker-compose.yml
└── README.md


