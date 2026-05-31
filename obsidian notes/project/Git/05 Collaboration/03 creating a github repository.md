click the plus icon in the top right of the page to create a github repository,
when we have local repository we can connect it to a Github repository via :

To share your local repository on GitHub, you need to:

## 1. Create an empty repository on GitHub
- Go to github.com → Click **"+"** → **New repository**
- **Do NOT** initialize with README, .gitignore, or license (since you already have a local repo)
- Copy the remote URL (e.g., `https://github.com/username/repo.git`)

## 2. Connect and push your local repo

```bash
# Add GitHub as remote
git remote add origin https://github.com/username/repo.git

# Push your branch (usually main or master)
git push -u origin main
```

**If your default branch is named `master`:**
```bash
git push -u origin master
```

## Complete example:
```bash
# Navigate to your repo
cd my-local-project

# Add remote
git remote add origin https://github.com/john/awesome-project.git

# Push (assuming main branch)
git push -u origin main
```

## After first push:
Your code is on GitHub. Future pushes just need:
```bash
git push
```

## Troubleshooting:
| Issue                           | Fix                                                |
| ------------------------------- | -------------------------------------------------- |
| "remote origin already exists"  | `git remote set-url origin <new-url>`              |
| Reject push (different history) | `git pull origin main --allow-unrelated-histories` |
| Need authentication             | Use GitHub token (not password) or SSH key         |
