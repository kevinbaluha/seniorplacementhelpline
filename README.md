# Senior Placement Helpline

Static landing page for **seniorplacementhelpline.com** — a lead-generation site for Senior Placement Helpline LLC.

## What It Is

A single-page, fully self-contained HTML landing page designed to:
- Capture leads from families seeking senior assisted living placement
- Funnel inquiries to Higher Vision Health (highervisiohealth.com)
- Provide instant engagement via the embedded Helo chatbot (askhelo.com)

**Phone:** 866-ALF-FIND (866-253-3463)

## Files

| File | Description |
|------|-------------|
| `index.html` | Complete landing page — all CSS is inline in a `<style>` tag, no external dependencies beyond Google Fonts and the Helo chatbot script |

## Deploying to Cloudflare Pages

1. **Push this repo to GitHub** (or GitLab / any supported Git provider).

2. **Log in to Cloudflare Dashboard** → Workers & Pages → Create application → Pages → Connect to Git.

3. **Select the repository** and configure the build:
   | Setting | Value |
   |---------|-------|
   | Framework preset | None |
   | Build command | *(leave blank)* |
   | Build output directory | `/` (or leave blank) |
   | Root directory | `/` |

4. **Deploy.** Cloudflare Pages will serve `index.html` as the root automatically.

5. **Custom domain:** In Cloudflare Pages → your project → Custom domains → Add `seniorplacementhelpline.com` and follow the DNS instructions.

> No build step required — the page is pure HTML/CSS/JS.

## Lead Endpoint

Form submissions POST JSON to `https://highervisiohealth.com/leads`. Update this URL in `index.html` once the real endpoint is configured.

## Chatbot

The Helo chatbot is loaded via `https://askhelo.com/embed.js`. Update `clientId` in the `HeloConfig` block near the bottom of `index.html` once a real client ID is issued.
