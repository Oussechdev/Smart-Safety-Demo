# Smart-Safety – Industrial Risk Anticipation Platform 🧠⚙️

Smart-Safety est une plateforme intelligente conçue pour **prédire les risques HSE industriels** et **aider les techniciens** sur le terrain via un chatbot local basé sur une architecture RAG (Ollama + GPT).

## 📸 Aperçu du projet

![Acceuil](./screenshots/2Acceuil.png)
![Dashboard](./screenshots/8.0Dashboard.png)
![Chatbot](./screenshots/10Chatbot.png)
![Prédiction](./screenshots/5.2Choix_moyenInterv_AI.png)

## 🧩 Stack technique

- **Frontend** : ReactJS
- **Backend** : Node.js + Express + MongoDB
- **IA** : GPT and QWEN (via Ollama), PDF Summarizer, RAG local
- **Fonctionnalités** :
  - Prédiction de risques industriels
  - Génération automatique de rapports PDF
  - Chatbot intelligent offline
  - Architecture RAG embarquée pour rapidité et sécurité

## 🚀 Démarrer le projet
A React + FastAPI **HSE platform** that helps OCP employees evaluate risks, record interventions, and learn safety standards — all with a built‑in AI assistant.

---

## 🚀 Quick Start (Front‑end)

```bash
# Install dependencies (first time only)
npm install

# Run the dev server
npm start               # http://localhost:3000
```
*Hot‑reload is enabled, so every save refreshes the browser.*

---

## 🛠️ Essential Dev Commands
| Task | Command | Notes |
|------|---------|-------|
| **Start dev server** | `npm start` | Runs `react‑scripts start`. |
| **Lint & fix** | `npm run lint` | ESLint + Prettier (see *package.json*). |
| **Build for prod** | `npm run build` | Generates `/build` folder. |
| **Test** | `npm test` | React‑Testing‑Library / Jest. |

---

## 🌳 Git Workflow (Daily)
> All commands run from the project root in a terminal.

```bash
# 1. See what changed (optional)
git status

### One‑liner for small tweaks
```bash
git commit -am "fix: typo in navbar" && git push
```

---

## 🧑‍💻 Typical Session Checklist
1. `git pull` — sync with *main* before starting.
2. `npm start` — launch UI, code away.
3. Keep commits small & focused (< 150 LOC, single purpose).
4. Push at least once per work session.
5. Open a Pull Request if working on a branch (triggers CI).

---

## 🤖 Sample Questions for the Chatbot
| Français | English |
|----------|---------|
| *Que faire en cas de produit inflammable ?* | *What should I do in case of a flammable product?* |
| *Quel est le nom complet de l'ingénieur ?* | *What is the engineer’s full name?* |
| *Quelles technologies maîtrise Oussama ?* | *Which technologies does Oussama master?* |

---

## 🔊 Voice Feature (PyAudio)
```powershell
# Activate Python env (back‑end)
.venv\Scripts\Activate

# Install voice deps
pip install streamlit pandas requests openai speechrecognition pyaudio
```

---

## 🧩 Back‑end (FastAPI) Quick Start
```powershell
# In a second terminal, activate the same Python venv
.venv\Scripts\Activate

# Launch API with auto‑reload
uvicorn chat_api:app --reload --port 8000
```

API docs will be available at **http://localhost:8000/docs**.
```bash
cd frontend && npm install && npm start
cd backend && npm install && npm run dev
