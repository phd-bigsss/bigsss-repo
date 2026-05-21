# bigsss-repo

A practice repository for learning the basic Git and GitHub workflow. 🎓

This is my commit.

This repository is intended for **complete beginners** who want to practice the four most essential Git operations:

1. **Clone** – download a repository to your computer
2. **Pull** – fetch the latest changes from GitHub
3. **Commit** – save a snapshot of your changes locally
4. **Push** – upload your local commits to GitHub

---

## Prerequisites

- Install Git: https://git-scm.com/downloads
- Create a free GitHub account: https://github.com/join
- (Optional) Install [GitHub Desktop](https://desktop.github.com/) for a visual interface

---

## Step 1 – Clone the repository

Cloning creates a local copy of this repository on your computer.

```bash
git clone https://github.com/phd-bigsss/bigsss-repo.git
```

Then move into the newly created folder:

```bash
cd bigsss-repo
```

---

## Step 2 – Make a change

Open the file `practice.md` in any text editor and add your name or a short message at the bottom. Save the file when you are done.

You can always check what has changed with:

```bash
git status
```

---

## Step 3 – Commit your change

Committing records your change in the local history. It requires two commands:

```bash
# Stage the file you changed
git add practice.md

# Save the snapshot with a short description
git commit -m "Add my name to practice.md"
```

---

## Step 4 – Push your commit to GitHub

Pushing sends your local commit up to this repository on GitHub so others can see it.

```bash
git push
```

---

## Step 5 – Pull the latest changes

Before you start working, or whenever you want to make sure your local copy is up to date, run:

```bash
git pull
```

This downloads any new commits that other people have pushed since you last synced.

---

## Quick reference

| Command | What it does |
|---|---|
| `git clone <url>` | Download a repository for the first time |
| `git status` | Show which files have changed |
| `git add <file>` | Stage a file for the next commit |
| `git commit -m "message"` | Save a snapshot of staged changes |
| `git push` | Upload commits to GitHub |
| `git pull` | Download the latest commits from GitHub |

---

## Troubleshooting

- **Permission denied / authentication error** – Make sure you are logged in. You may need to set up a [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) or [SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).
- **"Your branch is behind"** – Run `git pull` to sync before pushing.
- **Merge conflict** – This happens when two people edited the same line. Open the file, look for the `<<<<<<<` markers, decide which version to keep, save, then `git add` and `git commit`.

---

Happy committing! 🚀
