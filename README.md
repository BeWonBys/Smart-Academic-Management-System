# 📘 Smart Academic Management System

A collaborative academic management platform built and maintained by a team using Git & GitHub workflows.

---

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Getting Started](#getting-started)
- [Team Git Workflow](#team-git-workflow)
- [Repository Structure](#repository-structure)
- [Team Rules](#team-rules)
- [License](#license)

---

## 📌 About the Project

The **Smart Academic Management System** is designed to streamline academic operations including student management, course scheduling, and performance tracking. This repository is collaboratively maintained by a development team following a structured Git workflow.

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/) / XAMP / VScode
- A GitHub account

### Installation

```bash
# 1. Fork this repository (click Fork on GitHub)

# 2. Clone your fork
git clone https://github.com/YOUR-USERNAME/Smart-Academic-Management-System.git
cd Smart-Academic-Management-System

# 3. Add the original repo as upstream
git remote add upstream https://github.com/MAIN-OWNER/Smart-Academic-Management-System.git

# 4. Verify remotes
git remote -v
```

---

## 👥 Team Git Workflow

### 🔁 Step-by-Step Guide

#### 1. Fork the Repository
Go to the main repository on GitHub and click **Fork**. This creates your personal copy.

#### 2. Clone Your Fork
```bash
git clone https://github.com/YOUR-USERNAME/Smart-Academic-Management-System.git
cd Smart-Academic-Management-System
```

#### 3. Add Upstream Remote
```bash
git remote add upstream https://github.com/MAIN-OWNER/Smart-Academic-Management-System.git
```

#### 4. Create a New Branch ⚠️ MANDATORY
```bash
git checkout -b feature-name
# Example:
git checkout -b feature-login
```

> ❌ **Never work directly on the `main` branch.**

#### 5. Make Your Changes & Commit
```bash
git status
git add .
git commit -m "Added login feature"
```

#### 6. Push to Your Fork
```bash
git push origin feature-name
```

#### 7. Create a Pull Request
- Go to your fork on GitHub
- Click **Compare & Pull Request**
- Set **Base branch** → `main` | **Compare branch** → your feature branch
- Click **Create Pull Request**

#### 8. Merge (Project Owner Only)
The project owner will review the code and click **Merge Pull Request**.

---

### 🔄 Syncing Your Fork After a Merge

```bash
git checkout main
git fetch upstream
git merge upstream/main
git push origin main
```

---

### 📋 Complete Workflow Summary

```bash
# Fork on GitHub, then:

git clone https://github.com/YOUR-USERNAME/Smart-Academic-Management-System.git
cd Smart-Academic-Management-System

git remote add upstream https://github.com/MAIN-OWNER/Smart-Academic-Management-System.git

git checkout -b feature-name

# Make changes...
git add .
git commit -m "Your descriptive commit message"

git push origin feature-name

# Create Pull Request on GitHub

# After merge, sync your fork:
git checkout main
git fetch upstream
git merge upstream/main
git push origin main
```

---

## 📁 Repository Structure

```
Smart-Academic-Management-System/
├── README.md          # Project documentation
├── .gitignore         # Files excluded from Git tracking
├── LICENSE            # MIT License
└── src/               # Source code
```

### Important Files

| File | Purpose |
|------|---------|
| `README.md` | Project overview and workflow guide |
| `.gitignore` | Excludes `node_modules/`, `.env`, `build/`, `dist/`, `*.log` from tracking |
| `LICENSE` | MIT License — allows reuse while protecting authors |

---

## 📌 Team Rules

| Rule | Status |
|------|--------|
| Never push directly to `main` | ❌ Forbidden |
| Always create a new branch | ✅ Required |
| Always open a Pull Request | ✅ Required |
| Write meaningful commit messages | ✅ Required |
| Pull latest updates before starting work | ✅ Required |

---

## ⚖️ License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

> 💡 **Tip:** Always run `git fetch upstream` before starting new work to make sure you have the latest changes from the main repository.
