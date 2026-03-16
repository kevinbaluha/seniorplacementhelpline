# Senior Placement Helpline

Static landing page for **seniorplacementhelpline.com** — a lead-generation site for Senior Placement Helpline LLC (Marshall Zale).

## What It Is

A single-page, fully self-contained HTML landing page designed to:

- Capture leads from families seeking senior assisted living placement
- Funnel inquiries to Higher Vision Health (highervisiohealth.com)
- Drive phone calls to **866-ALF-FIND (866-253-3463)**

**Sections:** Hero → How It Works → Why Us → Service Area Map → Lead Form → Testimonials → Footer

## Files

| File | Description |
|------|-------------|
| `index.html` | Complete landing page — all CSS inline in `<style>` tag; no external dependencies beyond Google Fonts |

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

4. **Deploy.** Cloudflare Pages serves `index.html` as the root automatically.

5. **Custom domain:** In Cloudflare Pages → your project → Custom domains → Add `seniorplacementhelpline.com` and follow the DNS instructions.

> No build step required — the page is pure HTML/CSS/JS.

## Lead Endpoint

Form submissions POST JSON to `https://highervisiohealth.com/leads`. Update this URL in `index.html` once the real endpoint is configured.

## Phone Number

**866-ALF-FIND** = **866-253-3463** — appears prominently in the top bar, nav, hero, lead form section, CTA band, and footer.
