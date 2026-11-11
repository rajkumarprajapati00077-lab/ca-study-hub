# CA Study Hub

A simple, clean, mobile-friendly blog for CA Inter Group I (Jan 2027 attempt) study tips, written in clear, simple English. (Rebuilt in English on 11 Nov 2026 — the earlier version was in Hinglish.)

- **Live site:** (see deployment URL)
- **Stack:** plain static HTML + CSS. No build step, no framework, no database.
- **Content:** 7 articles (600–900 words each) + About page.

## Files

- `index.html` — homepage with article cards + exam dates
- `about.html` — about the blog
- `articles/` — 7 article pages
- `styles.css` — all styling (light theme)
- `logo.svg` — full logo (graduation cap + open book + "CA Study Hub" wordmark), used in the site header and footer
- `favicon.svg` — logo mark only, used as the site favicon
- `logo-fb-profile.png` — 500×500 PNG of the logo, for use as a Facebook Page profile picture
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Monetag ad slots (placeholder — fill in later)

There are clearly marked ad slots in the HTML where the Monetag **MultiTag** script goes:

- `index.html` — one slot below the hero (`id="monetag-ad-slot-home"`)
- Every article page — one slot after the article content (`id="monetag-ad-slot-article"`)

Each slot looks like this:

```html
<!-- MONETAG AD SLOT — paste your Monetag MultiTag script here.
     Get it from: monetag.com → Sites → Add your site → MultiTag.
     Do NOT paste any other network's tag here.
     Leave this empty until you have your real tag. -->
<div class="ad-slot" id="monetag-ad-slot-home"><!-- Monetag MultiTag goes here --></div>
```

**How to activate ads (when ready):**
1. Sign up at monetag.com and add this site.
2. Copy the MultiTag script they give you.
3. Paste it inside the `div` (replacing the `<!-- Monetag MultiTag goes here -->` comment) in `index.html` and in each article page.
4. Redeploy. No other code change is needed.

**Do NOT invent a Monetag tag or account ID.** The slots are intentionally empty until the real tag is pasted in. Do NOT put any ad code on EduEliteAI — this is a separate site only.

## Deploy

- **Vercel (tried first):** blocked — the Vercel connection returns 403 for the team scope (`rajkumarprajapati00077-3506s-projects`) and there is no `authorize_team_access` tool available to re-authorize it. The user would need to re-authorize team access before Vercel deploys work again.
- **GitHub Pages (live):** free static hosting. Repo: `rajkumarprajapati00077-lab/ca-study-hub`, branch `main`, Pages build type `legacy` (deploy from branch root). Live at `https://rajkumarprajapati00077-lab.github.io/ca-study-hub/`.

## Accuracy notes

- Exam dates stated on the site (Adv Accounts 2 Jan 2027, Law 4 Jan 2027, Taxation 6 Jan 2027, 2–5 PM, reading from 1:45 PM) are the Jan 2027 Group I dates.
- No ICAI rules, dates, paper patterns, statistics, ranks or toppers are invented on this site. Where a rule is general (e.g. 40% per paper / 50% aggregate), it is the standard, long-standing ICAI passing rule.
- The ICAI mock test series dates in the mock-test article (Series I: 19/21/23 Nov 2026; Series II: 3/5/7 Dec 2026; 10 AM–1 PM) were verified against ICAI's official mock test schedule.
