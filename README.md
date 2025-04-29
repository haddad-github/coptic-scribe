# Coptic Scribe

**Coptic Scribe** is a tool to help users learn Coptic, by providing live transliteration, translation, as well as bookmarking and exporting functionalities.

This repository serves as the **entry point** and index for the full Coptic Scribe system.

---

## 🌐 Live Project

**Live website:** [https://copticscribe.com](https://copticscribe.com)

---

## 📦 Project Repositories

| Component | Description | Tech Stack |
|-----------|-------------|------------|
| [`coptic-scribe-frontend`](https://github.com/haddad-github/coptic-scribe-frontend) | React frontend with virtual Coptic keyboard, PDF/CSV export, and search UI | React, TypeScript, Tailwind |
| [`coptic-scribe-user-backend`](https://github.com/haddad-github/coptic-scribe-user-backend) | Auth & bookmark API with JWT authentication and PostgreSQL | Java, Spring Boot, PostgreSQL |
| [`coptic-scribe-dictionary-backend`](https://github.com/haddad-github/coptic-scribe-dictionary-backend) | Dictionary API backend for Coptic word retrieval and search | Go (Gin), PostgreSQL |

---

## 🧱 Architecture Overview

```
                   ┌────────────────────────┐
                   │    React Frontend       │
                   │  (copticscribe.com)     │
                   └──────────┬──────────────┘
                              │
        ┌─────────────────────┼─────────────────────┐
        ▼                                             ▼
┌──────────────────────┐                  ┌──────────────────────────┐
│ Dictionary Backend   │                  │  User API Backend         │
│  (Go + PostgreSQL)    │                  │  (Spring Boot + PostgreSQL) │
└──────────────────────┘                  └──────────────────────────┘
```

---

## 🚀 Getting Started

Each repo includes Docker-based setup and Makefile automation. You can run each one individually for local development.

```bash
# Clone all three repositories:
git clone https://github.com/haddad-github/coptic-scribe-frontend.git
git clone https://github.com/haddad-github/coptic-scribe-dictionary-backend.git
git clone https://github.com/haddad-github/coptic-scribe-user-backend.git
```

See individual READMEs for:

- Environment variable setup
- Docker & local dev usage
- API testing and endpoints

---

## ✨ Key Features

- 🔎 Coptic–Arabic–English dictionary
- 🧠 Real-time transliteration with hover-based pronunciation rule explanations
- 🧾 Export results as CSV, TXT, or Unicode-safe PDF
- 🔐 Secure JWT-based login and signup system
- ⭐ Bookmarking with notes and quick retrieval
- 🐳 Docker-first development with Makefile automation

---

## 🛠️ Tech Stack

| Layer     | Technologies |
|-----------|--------------|
| Frontend  | React, TypeScript, Tailwind CSS |
| Backends  | Go (Gin) + PostgreSQL, Java (Spring Boot) + PostgreSQL |
| Tools     | Docker, Make, Python (Excel parsing), GitHub Actions |
| Cloud     | Azure Static Web Apps + Azure Database for PostgreSQL |

---

## 📜 License

MIT License © 2025 – Rafic Haddad

---

## ✍️ Author

[github.com/haddad-github](https://github.com/haddad-github)
