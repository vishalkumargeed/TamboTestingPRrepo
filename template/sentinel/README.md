# Tambo Sentinel

Tambo Sentinel is an AI-powered agent designed to assist maintainers by automatically reviewing GitHub pull requests and providing context-aware feedback.

---

## 📸 Preview

### Screenshot
![Tambo Sentinel Dashboard](https://via.placeholder.com/800x450?text=App+Running+with+Tambo+UI+Visible)
*The main interface showcasing real-time PR analysis with Tambo UI components.*

### Video Demo
[Watch the AI Interaction Demo](https://your-video-link-here.com)

---

## ⚙️ Prerequisites

To run this project, you will need the following:

* **GitHub Account:** To configure a GitHub App or OAuth for repository access.
* **Database:** A PostgreSQL instance (local or hosted via Supabase/Neon).
* **API Keys:**
    * `AUTH_SECRET`: A secure string for Auth.js sessions.
    * `GITHUB_ID` & `GITHUB_SECRET`: For GitHub authentication.
    * `AI_PROVIDER_API_KEY`: API key for your LLM (OpenAI, Anthropic, etc.).
    * `DATABASE_URL`: Your Prisma connection string.

---

## 🚀 Setup Steps

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/vishalkumargeed/tambo-sentinel.git](https://github.com/vishalkumargeed/tambo-sentinel.git)
   cd tambo-sentinel

# Install DEpendencies 
npm install

# Configure environment variables: Create a .env file in the root directory and add your credentials:
DATABASE_URL="postgresql://..."
AUTH_SECRET="your_secret_here"
GITHUB_ID="your_client_id"
GITHUB_SECRET="your_client_secret"

# Initialize the database: 
npx prisma migrate dev --name init
npx prisma generate

