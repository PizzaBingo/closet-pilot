# Closet Pilot: Antigravity, Git & Multi-Device Quick Guide

* **Google Doc Version:** [Closet Pilot: Antigravity, Git & Multi-Device Quick Guide](https://docs.google.com/document/d/1KoNNEuMbhwMItir2rNFklmwMymiROuqGhefqPIr1Up8/edit)
* **GitHub Repository:** [https://github.com/PizzaBingo/closet-pilot](https://github.com/PizzaBingo/closet-pilot)
* **Git Identity:** `Jared Stewart` (`jaredstewartise@gmail.com`)

## 1. Google-to-External Cheat Sheet

| Google Internal | External Equivalent | How It Works |
| :--- | :--- | :--- |
| **Piper + CitC (`hg`)** | **Git** (local) | Instead of a single cloud monorepo (`google3`), each project is a local folder tracked by **Git**. |
| **CL (Changelist)** | **Commit / Branch** | Locally, you save snapshots of your work as **commits** (`git commit`) on a **branch**. |
| **Critique + Piper Backup** | **GitHub** (cloud) | **GitHub** hosts your repository in the cloud. Run `git push` to upload commits or open a **Pull Request (PR)**. |
| **CodeSearch (CS)** | **Antigravity / Local Search** | Antigravity reads and searches your local project directly; GitHub provides a web view. |
| **Blaze + `BUILD` files** | **Package Managers** | Each language uses its own build/package tool (e.g., `npm` for JS/TS, `pip` or `uv` for Python). |

## 2. Switching Between Your Windows PC and MacBook

### A. Before Leaving Your Windows PC
1. Tell Antigravity: *"Commit and push all my latest changes to GitHub."*
2. **Tip for Chat Context:** Antigravity chat history stays on the computer where it ran. If you finish a `/grill-me` or `/plan` session and want those decisions on your MacBook, tell the agent: *"Save our agreed plan and decisions into `GEMINI.md` (or `PLAN.md`) and push to GitHub."*

### B. First-Time Setup on Your MacBook ("Clone" the Repo)
1. Open **Antigravity** on your MacBook, start a chat, and paste:

```text
Help me sign into GitHub (`gh auth login`), clone https://github.com/PizzaBingo/closet-pilot into my projects folder, and set my git user.name to "Jared Stewart" and user.email to "jaredstewartise@gmail.com".
```

2. In Antigravity's left sidebar, click **Projects** and open the newly cloned `closet-pilot` folder.
3. Because `GEMINI.md` and `README.md` are inside the repository, Antigravity on your MacBook will automatically load all of your project context and instructions.

### C. Ongoing Daily Workflow Between Computers
* **When finishing on Machine A:** Tell Antigravity *"Commit and push to GitHub"* (`git push`).
* **When sitting down at Machine B:** Tell Antigravity *"Pull the latest changes from GitHub"* (`git pull`).

## 3. Ready-to-Use `/grill-me` Prompt for `closet-pilot`

Once you open the `closet-pilot` project in Antigravity, start a new conversation and paste:

```text
/grill-me Read README.md and GEMINI.md to understand Closet Pilot. This is my first coding project outside of Google's internal environment, and I want to build an MVP that takes the friction out of selling clothes I don't want anymore.

Interview me to lock down the product design, user flow, and tech stack for Version 1—specifically covering:
1. How I want to capture/upload photos and get AI Photo Coach feedback
2. How the "Sell, Consign, or Donate" triage, platform recommendations, and sold-comp pricing should work
3. How the garment measurement checklist and listing copy generator should look
4. How simple the inventory tracker should be for the MVP
5. The simplest local setup and Gemini API integration for me to run and test right away
```
