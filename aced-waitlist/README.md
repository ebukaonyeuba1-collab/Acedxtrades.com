# Aced Xtrades — Wait List Landing Page

A single static page, no build step. Deploys straight to Vercel from GitHub.

## Before you deploy — fill these in

Open `index.html`, find the `CONFIG` object near the bottom (inside the `<script>` tag), and fill in:

- `whatsappNumber` — your official Aced Xtrades WhatsApp number, digits only with country code, no `+` (e.g. `2348012345678`)
- `tiktokHandle` — your TikTok username, no `@`
- `instagramHandle` — your Instagram username, no `@`
- `formEndpoint` — where wait list signups actually get stored. Right now the form is cosmetic — it shows a success message but doesn't save anything anywhere. Easiest fix: create a free form at [formspree.io](https://formspree.io) or [getform.io](https://getform.io), paste the endpoint URL here, and submissions will land in your inbox / their dashboard.

## Deploy to Vercel via GitHub

1. Create a new GitHub repo (e.g. `aced-xtrades-waitlist`) and push these two files to it.
2. Go to [vercel.com/new](https://vercel.com/new), sign in with your GitHub account, and import the repo.
3. Vercel will detect it as a static site automatically — no framework, no build command needed. Click **Deploy**.
4. Once it's live, add your own domain under Project Settings → Domains if you have one.

## What's on the page

- Hero with wait list signup (WhatsApp number + email)
- "The Book" — an illustrative rates panel for crypto and gift cards
- 3-step explainer: join → get messaged on WhatsApp → trade now, migrate later
- Founder/creator section for your TikTok and Instagram handles
- A quiet legal line noting this is currently a manually operated service, not yet a licensed platform — worth keeping given the VASP licensing question
- Second signup form + WhatsApp deep link in the footer

## Editing content later

Everything is in one file, `index.html` — copy is plain text in the HTML, colors and fonts are CSS variables at the top of the `<style>` block (`--black`, `--red`, `--yellow`, `--cream`).
