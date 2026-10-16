# GitHub CLI & CI/CD Basics (GitHub Actions)

## 1. GitHub CLI (`gh`)
*   **What it is:** The official command-line tool from GitHub that brings GitHub features (like pull requests, issues, and repos) directly into your terminal.
*   **Key Commands:**
    *   `gh auth login` — Authenticates your terminal with your GitHub account.
    *   `gh repo clone <owner/repo>` — Clones a repository quickly from the command line.
    *   `gh pr create` — Opens a new pull request for your current branch directly from your terminal.
    *   `gh issue list` — Views and manages open issues for the repository.

## 2. CI/CD in GitHub
*   **What it is:** A software development practice where changes are automatically tested and delivered.
    *   **CI (Continuous Integration):** Automatically building and running tests every time you push code to ensure new changes don't break the project.
    *   **CD (Continuous Deployment/Delivery):** Automatically releasing or deploying your tested code to staging or production environments.

## 3. GitHub Actions
*   **What it is:** GitHub’s built-in automation and CI/CD tool that lets you build custom software development workflows.
*   **Key Concepts:**
    *   **Workflow:** An automated process defined in a configuration file that runs one or more jobs.
    *   **Event:** A specific trigger that kicks off a workflow (e.g., a `push` to `main`, opening a `pull_request`, or a cron schedule).
    *   **Job:** A group of steps that run together on the same virtual machine (runner).
    *   **Step:** An individual task that runs commands (such as installing dependencies or running a test script).
*   **File Structure:** Workflows are written in YAML and stored in your repository under `.github/workflows/<filename>.yml`.
