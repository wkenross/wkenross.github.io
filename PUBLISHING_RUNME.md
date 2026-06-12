# Root GitHub Pages Publishing RunMe

Generated: 2026-06-12T15:42:35

## Target

- Repository: `wkenross/wkenross.github.io`
- Public website URL: `https://wkenross.github.io/`
- Local folder: `%USERPROFILE%\OneDrive\projects\wkenross.github.io`

## Local Review

```powershell
start "$env:USERPROFILE\OneDrive\projects\wkenross.github.io\index.html"
```

## Git Setup

```powershell
cd "$env:USERPROFILE\OneDrive\projects\wkenross.github.io"
git config user.name "Ken Rossiter"
git config user.email "wkenross@users.noreply.github.com"
git add .
git commit -m "Initial root website scaffold"
```

## Create And Push Repository

If GitHub CLI is installed and authenticated:

```powershell
gh repo create wkenross/wkenross.github.io --public --source . --remote origin --push
```

If GitHub CLI is not installed, create `wkenross.github.io` in the GitHub web UI,
then run:

```powershell
git remote add origin https://github.com/wkenross/wkenross.github.io.git
git branch -M main
git push -u origin main
```

After GitHub Pages builds, the company/personal website root URL is:

```text
https://wkenross.github.io/
```
