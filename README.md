# 🚀 PRisma

**PRisma** is a full-stack, AI-powered pull request review assistant that integrates with GitHub to provide inline suggestions, detect bugs, and deliver step-by-step code explanations using cutting-edge language models like GPT-4. The tool enhances code quality, streamlines team collaboration, and boosts developer onboarding efficiency.

---

## 📚 Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Tech Stack](#tech-stack)
- [How It Works](#how-it-works)
- [Quick Start](#quick-start)
- [Configuration](#configuration)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## ✨ Features

- **🧠 AI-Driven Static Code Analysis**  
  Automatically reviews pull requests, flags bugs or anti-patterns, and suggests improvements.

- **📌 Inline Explanations**  
  Generates clear, line-by-line review comments with detailed reasoning and step-by-step fixes.

- **🔗 Seamless GitHub Integration**  
  Connects to your repositories, fetching new PRs and posting reviews via GitHub Apps/Webhooks.

- **📊 Customizable Dashboard**  
  Central location to view pull requests, flagged issues, and feedback metrics.

- **🔄 Continuous Learning**  
  Learns from team feedback on suggestions to improve future code reviews.

---

## 🎥 Demo

🚧 Coming soon! Stay tuned for a walkthrough video and live app link.

---

## 🛠 Tech Stack

| Component   | Tech                                                                 |
|-------------|----------------------------------------------------------------------|
| Frontend    | [Next.js](https://nextjs.org/) (React)                               |
| Backend     | [Node.js](https://nodejs.org/) (Express) or [FastAPI](https://fastapi.tiangolo.com/) |
| AI Service  | [OpenAI GPT-4 API](https://platform.openai.com/) or Hugging Face LLMs |
| Database    | [MongoDB](https://www.mongodb.com/) or [PostgreSQL](https://www.postgresql.org/) |
| DevOps      | Docker, GitHub Actions                                               |
| Integration | GitHub REST & Webhook APIs                                           |

---

## ⚙️ How It Works

1. **Connect PRisma** to your GitHub organization or repository.
2. **PR events** trigger webhooks that send changed code, diffs, and context to the backend.
3. The **AI review engine** analyzes the code, flags issues, and crafts detailed explanations.
4. **Inline comments** are posted automatically on GitHub PRs for team feedback.
5. All reviews and suggestions appear in the **dashboard** for tracking and learning.

---

## ⚡ Quick Start

### 1. Clone the Repository

```bash
    git clone https://github.com/YOUR_USERNAME/PRisma.git
    cd PRisma
```
### 2. Install Dependencies

```bash
    cd backend && npm install
    cd ../frontend && npm install
```
### 3. Set Up Environment Variables
```eenv
Copy .env.example → .env in both frontend and backend

Fill in:
1. GitHub App credentials
2. OpenAI or Hugging Face API key
3. Your DB connection string
```
4. Register Your GitHub App
```bash
  1. Go to GitHub Developer Settings
  2. Create a new GitHub App
  3. Set webhook callback URL to:
  4. https://your-backend-domain.com/webhooks/github
```
5. Run Locally
```bash
   # Backend
  cd backend
  npm start

  # Frontend
  cd ../frontend
  npm run dev
```
6. Test It
```bash
1. Open a pull request in a connected repo
2. Watch PRisma analyze and comment on your code 🎯
```

## Configuration

1. Configure AI engine: OpenAI, Claude, or Hugging Face via .env
2. Modify prompts in config/reviewPrompts.js to change tone/style
3. Adjust severity thresholds, token limits, or target files

## 🧪 Usage

PRisma automatically reviews every new pull request
Suggestions are posted as inline comments with detailed explanations
Dashboard shows:
Total PRs reviewed
Common issues flagged
Developer feedback ratings

## 🤝 Contributing

We welcome PRs, ideas, and feedback!
Fork the repo
Create a feature branch
Submit a PR with your change and a clear description

## 📄 License
Licensed under the MIT License — free for personal and commercial use.

