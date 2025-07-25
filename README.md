# PRisma

**PRisma** is a full-stack, AI-powered pull request review assistant that integrates with GitHub to provide inline suggestions, detect bugs, and deliver step-by-step code explanations using cutting-edge language models like GPT-4. The tool enhances code quality, streamlines team collaboration, and boosts developer onboarding efficiency.

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Tech Stack](#tech-stack)
- [How It Works](#how-it-works)
- [Quick Start](#quick-start)
- [Configuration](#configuration)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- **AI-Driven Static Code Analysis**  
  Automatically reviews pull requests, flags bugs or anti-patterns, and suggests improvements.

- **Inline Explanations**  
  Generates clear, line-by-line review comments with detailed reasoning and step-by-step fixes.

- **Seamless GitHub Integration**  
  Connects to your repositories, fetching new PRs and posting reviews via GitHub Apps/Webhooks.

- **Customizable Dashboard**  
  Central location to view pull requests, flagged issues, and feedback metrics.

- **Continuous Learning**  
  Learns from team feedback on suggestions to improve future code reviews.

## Demo

Coming soon! Stay tuned for a walkthrough video and live app link.

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

## How It Works

1. **Connect PRisma to your GitHub organization or repository.**
2. **PR events** trigger webhooks that send changed code, diffs, and context to the backend.
3. The **AI review engine** analyzes the code, flags issues, and crafts detailed explanations.
4. **Inline comments** are posted automatically on GitHub PRs for team feedback.
5. All reviews and suggestions appear in the **dashboard** for tracking and learning.

## Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/stealthwhizz/Prisma.git
   cd PRisma
2. Setup Environment Variables
   Create a .env file:
   ```env
   OPENAI_API_KEY=your_openai_key
   GITHUB_CLIENT_ID=xxx
   GITHUB_CLIENT_SECRET=xxx
   DATABASE_URL=your_db_connection_string


