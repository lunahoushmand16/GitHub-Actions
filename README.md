# Mini-Project: 🎬 Film Tracker – CI/CD Mini Project

This project is a simple film tracking app that demonstrates automated testing and deployment using **GitHub Actions** and **Render**.

Users can:
- Search for films using the OMDb API
- Add them to a watchlist or mark them as seen
- View previously watched films

---

## ⚙️ Tech Stack

- **Vite + React + TypeScript**
- **Vitest** for testing
- **GitHub Actions** for CI/CD
- **Render** for deployment

---

## 🚀 Deployment

This project is automatically deployed to [Render](https://render.com/) when:
 - A pull request is merged into the `main` branch
 - All GitHub Action checks pass (`Checking Tests` and `Deploy To Render`)

🔗 **Live App**: [https://github-actions-3po4.onrender.com](https://github-actions-3po4.onrender.com)

---

## 📦 Setup Instructions

To run locally:

  ```bash
  npm install
  npm run dev
  ```
To run tests:
   ```sh
   npm install
   ```
You'll need a .env file with a dummy or real OMDb API key:
   ```bash
   VITE_OMDB_API_KEY=fakekey123
   ```
## ✅ GitHub Actions Workflow

 - .github/workflows/checking_tests.yml: Runs tests on PRs to main and develop

 - .github/workflows/deploy_to_render.yml: Deploys to Render on merge to main

## 🛡️ Branch Protection Rules
 - develop: Requires tests to pass before merging

 - main: Requires PR, test pass, and deploy success before merging

 ## 🧪 Tests
- Vitest and React Testing Library are used to ensure component behavior is correct and CI pipelines are enforced properly.

## 📚 Credits
Project built as part of a full-stack bootcamp mini-project to practice DevOps workflows and CI/CD concepts.