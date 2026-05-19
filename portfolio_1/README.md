# Anuj Jain — Portfolio
> Built with Astro · Managed via Decap CMS · Hosted on Netlify · Media on Cloudinary

---

## 🚀 Quick Start (First Time)

### 1. Prerequisites
- Node.js 18+ installed → [nodejs.org](https://nodejs.org)
- A GitHub account
- A Netlify account (free) → [netlify.com](https://netlify.com)
- A Cloudinary account (free) → [cloudinary.com](https://cloudinary.com)

### 2. Install & Run Locally
```bash
cd anuj-portfolio
npm install
npm run dev
# → opens at http://localhost:4321
```

### 3. Deploy to Netlify (One Time)
1. Push this folder to a new GitHub repo
2. Go to [app.netlify.com](https://app.netlify.com) → **Add new site** → **Import from Git**
3. Pick your repo — Netlify auto-detects Astro
4. Build command: `npm run build` · Publish directory: `dist`
5. Click **Deploy** — your site is live!

### 4. Enable CMS Login (One Time)
1. In Netlify dashboard → **Identity** tab → **Enable Identity**
2. Under **Registration** → set to **Invite only**
3. **Invite yourself** with your email → accept the invite
4. Under **Services** → **Git Gateway** → **Enable Git Gateway**
5. Now go to `yoursite.netlify.app/admin` → log in → you're in the CMS!

---

## ✏️ Adding / Editing Projects (No Code Needed)

Go to: **`yoursite.netlify.app/admin`**

1. Click **Projects** in the left sidebar
2. Click **+ New Project** or click an existing one to edit
3. Fill in the fields (see field guide below)
4. Click **Publish** → site rebuilds and goes live in ~60 seconds

### Field Guide

| Field | What to put |
|---|---|
| **Title** | Game name e.g. "PuzzleMania" |
| **Subtitle** | Short descriptor e.g. "Solo Mobile Game · Android" |
| **Status** | LIVE / CURRENT / SHIPPED / WIP |
| **Sort Order** | 1 = first, 99 = last |
| **Featured** | Toggle on for top 1–2 projects |
| **Media Type** | Choose GIF / MP4 / YouTube / Image |
| **Media File** | Upload GIF or image directly |
| **Cloudinary Video URL** | Paste full MP4 URL from Cloudinary for videos |
| **YouTube Video ID** | Just the ID: `dQw4w9WgXcQ` from youtube.com/watch?v=**dQw4w9WgXcQ** |
| **Tech Challenge** | What was the hard problem you solved? |
| **Business Outcome** | What shipped? Real-world result? |
| **Code Quality** | Design patterns, architecture decisions |
| **Tags** | Unity, C#, iOS, etc. — add one per line |
| **Key Metrics** | e.g. "3 Platforms", "Live on Play Store" |
| **Accent Color** | Pick a color for this project's highlights |

---

## 🎬 Adding Media (GIFs & Videos)

### Option A — GIF / Image
1. Upload your GIF directly in the CMS media field
2. Or upload to Cloudinary first, copy the URL, paste into **Cloudinary Video URL** field

### Option B — MP4 Video via Cloudinary (Recommended for video)
1. Go to [cloudinary.com](https://cloudinary.com) → Media Library
2. Upload your MP4 file
3. Click the file → copy the URL (ends in `.mp4`)
4. In the CMS → **Media Type**: Video · **Cloudinary Video URL**: paste URL

### Option C — YouTube
1. Upload gameplay footage to YouTube (can be unlisted)
2. Copy the video ID from the URL: `youtube.com/watch?v=` **THIS_PART**
3. In CMS → **Media Type**: YouTube · **YouTube Video ID**: paste the ID

### Cloudinary Free Tier
- **25 GB** storage
- **25 GB** bandwidth/month
- Automatic video compression (your MP4s will load faster)
- Sign up free at [cloudinary.com](https://cloudinary.com)
- After signing up, replace `YOUR_CLOUD_NAME` and `YOUR_API_KEY` in `public/admin/config.yml`

---

## 🗂 Project Structure

```
anuj-portfolio/
├── public/
│   ├── admin/
│   │   ├── index.html      ← CMS entry point (don't touch)
│   │   └── config.yml      ← CMS field definitions (edit to add new fields)
│   └── images/
│       └── projects/       ← Uploaded images land here
├── src/
│   ├── components/
│   │   ├── Nav.astro
│   │   ├── Hero.astro
│   │   ├── Marquee.astro
│   │   ├── About.astro
│   │   ├── Skills.astro
│   │   ├── Projects.astro  ← Main showcase component
│   │   ├── WhyMe.astro
│   │   ├── Contact.astro
│   │   └── Footer.astro
│   ├── content/
│   │   └── projects/       ← One .md file per project (CMS writes these)
│   │       ├── puzzlemania.md
│   │       ├── camel-cash-casino.md
│   │       ├── 7-star-vegas-slots.md
│   │       ├── uroc-framework.md
│   │       └── rnf-casino-suite.md
│   ├── layouts/
│   │   └── Base.astro      ← HTML head, fonts, meta tags
│   ├── pages/
│   │   └── index.astro     ← Main page (assembles all sections)
│   └── styles/
│       └── global.css      ← All design tokens, animations, component styles
├── astro.config.mjs
├── netlify.toml
├── package.json
└── README.md               ← You are here
```

---

## 🎨 Customising the Design

All design tokens live in `src/styles/global.css` at the top:

```css
:root {
  --bg: #0c0c0d;          /* Main background */
  --lime: #C8F135;        /* Accent colour — change this to rebrand */
  --text: #f0ede6;        /* Primary text */
  --text-muted: #6b6860;  /* Secondary text */
  --font-display: 'Instrument Serif', serif;
  --font-body: 'Cabinet Grotesk', sans-serif;
}
```

**To change the accent colour:** edit `--lime` in global.css. One change, updates everywhere.

---

## 🔄 Updating Personal Info

Edit these files directly:
- **About text** → `src/components/About.astro`
- **Skills list** → `src/components/Skills.astro`
- **Stats (13+, 5+)** → `src/components/Hero.astro`
- **Why Hire Me** → `src/components/WhyMe.astro`
- **Contact details** → `src/components/Contact.astro`

After editing: commit + push to GitHub → Netlify auto-redeploys.

---

## 💰 Cost Breakdown

| Service | Free Tier | What You Get |
|---|---|---|
| Netlify | ✅ Free | Hosting, deploys, CMS backend, SSL |
| Decap CMS | ✅ Free | Browser-based project editor |
| Cloudinary | ✅ Free | 25GB storage + video compression |
| **Total** | **$0/month** | Full stack, production-ready |

Optional upgrade: custom domain like `anujjain.dev` → ~$12/year from Namecheap or Google Domains.

---

## 🆘 Common Issues

**CMS won't load at /admin**
→ Make sure you enabled Netlify Identity and Git Gateway (see step 4 above)

**Changes not appearing after publish**
→ Wait 60–90 seconds for rebuild. Check Netlify dashboard → Deploys tab.

**Video not playing**
→ Make sure the Cloudinary URL ends in `.mp4` and the file is not private

**Project order wrong**
→ Edit the Sort Order field in CMS (lower number = appears first)
