# Setting this up as your GitHub profile README

GitHub shows this README on your profile page automatically once it lives in a
**public repository named exactly `sameerchore`** (i.e. the same as your username).

## 1. Create the repo

- On GitHub, click **New repository**.
- Name it `sameerchore` (must match your username exactly).
- Make it **Public**.
- Don't initialise it with a README (you already have one).

## 2. Push these files

```bash
cd sameerchore-github-profile
git init
git remote add origin https://github.com/sameerchore/sameerchore.git
git add .
git commit -m "Add profile README"
git branch -M main
git push -u origin main
```

Once pushed, visit `github.com/sameerchore` — the README renders on your profile.

## 3. What to personalise before (or after) publishing

Everything below is marked with an HTML comment or a bracketed placeholder in
`README.md` so it's easy to find and edit.

- **Email badge** — replace `REPLACE_WITH_YOUR_EMAIL` in the `mailto:` link with
  your real address.
- **LinkedIn / LeetCode / Portfolio badges** — commented out under the main
  badge row. Uncomment the ones you want and drop in your real links.
- **Selected work table** — replace the placeholder rows with your actual
  projects (GitHub repos, hackathon builds, coursework projects, anything
  you're proud of). Three rows are there as a starting shape; add or remove as
  needed.
- **"More things I've built"** — same idea, for smaller or older projects.
- **Stack badges** — a starter list based on a typical CSE third-year
  curriculum plus your stated interest in AI/ML. Swap in whatever you've
  actually used. [shields.io](https://shields.io) has a badge for almost
  every language, framework and tool if you want to add more.

## 4. Why the stats section uses live widgets

Instead of a static, hand-authored "language distribution" graphic, the
**By the numbers** section uses [github-readme-stats](https://github.com/anuraghazra/github-readme-stats)
and [github-readme-activity-graph](https://github.com/Ashutosh00710/github-readme-activity-graph).
These pull real numbers from your GitHub account at view time, styled to match
your palette — so the numbers are always accurate instead of being frozen
placeholder data. As you push more repos and commits, this section updates on
its own.

## 5. About `assets/profile-source.jpg`

This is your uploaded logo, included for reference so you have it alongside
the repo. It isn't referenced inside `README.md` — your GitHub avatar is set
separately in **GitHub → Settings → Public profile**, not through the README.
Upload it there if you haven't already.

## 6. Files in this package

```
sameerchore-github-profile/
├── README.md                   → the profile README itself
├── SETUP.md                    → this file
├── assets/
│   ├── header.svg               → top banner (name, role, meta)
│   ├── divider.svg              → thin section separator, reused throughout
│   ├── footer.svg                → closing banner
│   └── profile-source.jpg       → your uploaded logo (reference only)
└── .github/
    └── topics.yml                → optional repo topics
```

All image paths in `README.md` are relative (`assets/...`), so they work as
soon as the repo is pushed — no need to hard-code your username into raw
GitHub URLs. If you'd rather use absolute `raw.githubusercontent.com` links
(useful if you ever embed this README elsewhere), swap each `assets/x.svg`
for `https://raw.githubusercontent.com/sameerchore/sameerchore/main/assets/x.svg`.
