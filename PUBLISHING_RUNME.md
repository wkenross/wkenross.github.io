# Root GitHub Pages Publishing RunMe

Generated: 2026-06-12T18:18:16

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

Because GitHub CLI may not be installed on every configured laptop, the web UI
path is the most reliable default:

1. Open `https://github.com/new`.
2. Repository owner: `wkenross`.
3. Repository name: `wkenross.github.io`.
4. Set visibility to `Public`.
5. Do not initialize with README, `.gitignore`, or license because this local
   folder already has those files.
6. Create the repository.
7. Return to PowerShell and run:

```powershell
cd "$env:USERPROFILE\OneDrive\projects\wkenross.github.io"
git push -u origin main
```

If GitHub CLI is installed and authenticated:

```powershell
gh repo create wkenross/wkenross.github.io --public --source . --remote origin --push
```

If GitHub CLI is not installed, create `wkenross.github.io` in the GitHub web UI,
then run:

```powershell
git branch -M main
git push -u origin main
```

The `origin` remote is already configured by this scaffold. If it is ever
missing, restore it with:

```powershell
git remote add origin https://github.com/wkenross/wkenross.github.io.git
```

After GitHub Pages builds, the company/personal website root URL is:

```text
https://wkenross.github.io/
```
