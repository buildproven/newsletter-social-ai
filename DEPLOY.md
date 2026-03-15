# Deployment

## Quick Deploy (Vercel CLI)

```bash
npm i -g vercel
vercel --prod
```

When prompted, link to buildproven org, project name: `newsletter-social-ai`

## Auto-Deploy (GitHub Actions)

After the manual first deploy (above), add these GitHub secrets to `buildproven/newsletter-social-ai`:

- `VERCEL_TOKEN` — from [vercel.com/account/tokens](https://vercel.com/account/tokens)
- `VERCEL_ORG_ID` — from `.vercel/project.json` after first deploy
- `VERCEL_PROJECT_ID` — from `.vercel/project.json` after first deploy

Every push to `main` will auto-deploy to production after that.

## Live URL

After first deploy:
- Default: `https://newsletter-social-ai.vercel.app`
- Custom domain: `https://newsletter-social.buildproven.ai` (configure in Vercel dashboard)

## Setup Steps Summary

1. Run `vercel --prod` locally (one-time)
2. Copy `orgId` and `projectId` from `.vercel/project.json`
3. Add `VERCEL_TOKEN`, `VERCEL_ORG_ID`, `VERCEL_PROJECT_ID` to GitHub repo secrets
4. Push to `main` — GitHub Actions handles all future deploys

## GitHub Secrets Location

`https://github.com/buildproven/newsletter-social-ai/settings/secrets/actions`
