# Vordali Website — Authoritative Next.js Build

This repository is a Next.js App Router application.

## Package manager

This project uses **npm only**.

- `package.json`
- `package-lock.json`
- Node.js `22.x`

Do not add pnpm, Yarn, Bun, custom Vercel install commands, or a `vercel.json`
file unless the deployment architecture intentionally changes later.

## Vercel settings

- Framework Preset: Next.js
- Root Directory: `./`
- Node.js Version: `22.x`
- Install Command: leave blank
- Build Command: leave blank
- Output Directory: leave blank

Vercel should detect `package-lock.json` and install the project automatically.

## Required environment variables

- `SUPABASE_URL`
- `SUPABASE_SERVICE_ROLE_KEY`

The service-role key is used only inside server-side route handlers.

## Included routes

- `/`
- `/products`
- `/pricing`
- `/labs`
- `/why-vordali`
- `/trust`
- `/privacy`
- `/terms`
- `/sms-terms`
- `/cookies`
- `/acceptable-use`
- `/security`

Old `.html` addresses redirect through `next.config.ts`.

## Supabase

The existing migration remains at:

`supabase/migrations/006_platform_pricing_labs_foundation.sql`

## Recommended GitHub replacement procedure

Delete the current repository contents first, while keeping the repository itself.
Then upload the complete contents of this package to the repository root in one commit.

Suggested commit message:

`Replace repository with authoritative Next.js build`
