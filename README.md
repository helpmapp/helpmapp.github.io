# HelpmApp OS - Public Documentation

This repository contains the static build artifacts for **HelpmApp OS**, the "Swiss Social Realism" operating system for service discovery.

**Live Site:** [https://helpmapp.github.io](https://helpmapp.github.io)

## Deployment

This site is automatically deployed from the main [helpmapp/helpmapp](https://github.com/helpmapp/helpmapp) monorepo.

### Process

1. Content is authored in `apps/docs`.
2. `pnpm docs:build` generates the static HTML.
3. Artifacts are synced to this submodule.
4. Pushing to the `main` branch of this repository triggers GitHub Pages.

## Manual Update

```bash
# From root of main repo
pnpm docs:deploy
cd apps/public-site
git add .
git commit -m "deploy: update knowledge base"
git push origin main
```
