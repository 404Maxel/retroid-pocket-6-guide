# Your Own Website Project

Build a website about a topic you enjoy. Think about the content you would like to show.

## Getting Started

Clone your course repository using SSH and switch to the existing `solution` branch. Replace `YOUR-PROJECT` with your repository name:

```bash
git clone git@github.com:ctf-26d/YOUR-PROJECT.git webprojekt
cd webprojekt
git switch solution
```

The basic HTML structure in [index.html](index.html) is already linked to [style.css](style.css). Build a small version on top of it, check it in the browser, and expand it step by step.

Find layout tips, ideas, and links in [Help and Inspiration](help/hilfen.en.md). You may use AI and new techniques for help.

## Saving Your Progress

Work on `solution`. Commit your progress and push it to the course repository (`origin`):

```bash
git add .
git commit -m "Project updated"
git push origin solution
```

## Finishing Up

Before the final push, you can delete the help files in `help/` and briefly describe your project in `README.md`. Commit these changes and push your work to `origin` as shown above.

## Optional: Publish Your Project

Create a **public, empty repository** in your own GitHub account – without a README, license, or `.gitignore`. Replace the placeholders and add it once as a remote called `deploy`. Push your local `solution` branch to its `main` branch:

```bash
git remote add deploy git@github.com:YOUR-USERNAME/YOUR-REPO.git
git push deploy solution:main
```

For later changes, repeat `git push origin solution` and `git push deploy solution:main` after committing.

Publish your public repository with GitHub Pages from `main` and share the link in Slack. Unfinished and experimental projects can be published too.

![Git workflow: work locally on solution and push to origin and optionally deploy](assets/Git-Workflow_%20Lokal%20und%20zwei%20GitHub-Repos.png)
