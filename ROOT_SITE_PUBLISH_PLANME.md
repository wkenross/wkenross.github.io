# Root GitHub Pages Site PlanMe

Updated: 2026-06-12

## Purpose

Publish a clean root website for company/personal website fields that require a
base URL instead of a project subpage.

Primary URL:

```text
https://wkenross.github.io/
```

Supporting URLs:

```text
https://github.com/wkenross
https://wkenross.github.io/frame-showcase/
```

## Current Local State

Local folder:

```text
%USERPROFILE%\OneDrive\projects\wkenross.github.io
```

The folder is a standalone Git repository with remote:

```text
https://github.com/wkenross/wkenross.github.io.git
```

## Launch Plan

1. Review the local `index.html`.
2. Create a public GitHub repository named exactly `wkenross.github.io`.
3. Push local branch `main` to `origin`.
4. Wait for GitHub Pages to build the user site.
5. Confirm `https://wkenross.github.io/` loads.
6. Use the root URL for training sites, job applications, and company website
   fields.
7. Use `https://wkenross.github.io/frame-showcase/` only when a deeper FRAME
   showcase link is appropriate.

## Acceptance Criteria

- repository exists at `https://github.com/wkenross/wkenross.github.io`
- `git push -u origin main` completes successfully
- root URL no longer returns 404
- landing page links to GitHub, LinkedIn, email, and FRAME showcase
- `wb_github` docs identify root site and showcase site as separate lanes

## Notes For Future Codex Operators

Do not confuse the root user site with the FRAME project site:

| Site | Purpose |
|---|---|
| `https://wkenross.github.io/` | Company/personal website root URL. |
| `https://wkenross.github.io/frame-showcase/` | Deeper FRAME automation showcase. |
| `https://github.com/wkenross` | GitHub profile. |
