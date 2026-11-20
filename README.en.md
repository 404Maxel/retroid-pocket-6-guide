# Your Own Website Project

## Page Structure

- **Header** with a title or name
- **Introduction** with a short overview or a large image/gallery
- **Main content** with information
- **Contact or closing section**
- **Footer** with additional information

## Basic Decision

- One-page website
- Website with subpages

## Project

Think of a website that you would enjoy creating.

- What is the topic?
- What should be on the website?
- Think about how you can implement this content
    - Do you need any additional knowledge? Ask me or a chatbot

- start with a small version that works in the browser
- then expand it step by step
- regularly check in the browser to see what has changed
- you may use AI and techniques you have not learned yet for help

The goal today is not to submit a perfect website. Use the time to build something independently, try things out, and have fun with it.

## Git Workflow

Clone your project using SSH and switch to the existing `solution` branch. Replace `YOUR-PROJECT` with the name of your course repository:

```bash
git clone git@github.com:ctf-26d/YOUR-PROJECT.git webprojekt
cd webprojekt
git switch solution
```

Work on `solution`. Commit your progress regularly and push it back to the course repository (`origin`):

```bash
git add .
git commit -m "Project updated"
git push origin solution
```

### Optional: Publish Your Project

Create a **public, empty repository** in your own GitHub account – without a README, license, or `.gitignore`. Replace the placeholders and connect it as an additional remote called `deploy`. Then push your local `solution` branch to its `main` branch:

```bash
git remote add deploy git@github.com:YOUR-USERNAME/YOUR-REPO.git
git push deploy solution:main
```

Add the remote only once. For later changes, repeat both push commands after committing:

```bash
git push origin solution
git push deploy solution:main
```

For GitHub Pages, use your public repository and its `main` branch.

![Git workflow: work locally on solution and push to origin and optionally deploy](Git-Workflow_%20Lokal%20und%20zwei%20GitHub-Repos.png)

## Finishing Up

Before the final push, you can delete `hilfen.md` and add a short description of your own project to `README.md`. Commit these changes before pushing.

- push your work to the course repository with `git push origin solution`
- optionally, publish your project from your own public repository using GitHub Pages and share the link in Slack

Unfinished and experimental projects can be published too.
