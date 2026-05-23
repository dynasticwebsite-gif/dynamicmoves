# DM Dance Studio — Vercel Deployment Guide

## Files in this project
```
dm-dance-studio/
├── index.html      ← Your website
├── vercel.json     ← Vercel deployment config
└── README.md       ← This file
```

---

## Step-by-step: GitHub → Vercel

### 1. Create a GitHub Repository
1. Go to **https://github.com/new**
2. Name it `dm-dance-studio` (or any name you like)
3. Set it to **Public** or **Private** — both work with Vercel
4. Click **Create repository**

### 2. Upload your files to GitHub
**Option A — Upload via browser (easiest):**
1. On your new repo page, click **"uploading an existing file"**
2. Drag and drop **both files**: `index.html` and `vercel.json`
3. Click **Commit changes**

**Option B — Using Git (if you have Git installed):**
```bash
git init
git add .
git commit -m "Initial DM Dance Studio deploy"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/dm-dance-studio.git
git push -u origin main
```

### 3. Deploy on Vercel
1. Go to **https://vercel.com** and sign in (use your GitHub account)
2. Click **"Add New Project"**
3. Click **"Import"** next to your `dm-dance-studio` repository
4. On the Configure Project screen:
   - **Framework Preset:** leave as `Other`
   - **Root Directory:** leave as `./`
   - **Build & Output Settings:** leave everything blank
5. Click **Deploy**

✅ Your site will be live in ~30 seconds at a URL like:
`https://dm-dance-studio.vercel.app`

---

## Auto-deploy on every update
After the initial setup, every time you push changes to GitHub, Vercel will **automatically redeploy** your site. No manual steps needed.

---

## Custom Domain (optional)
1. In your Vercel project, go to **Settings → Domains**
2. Add your domain (e.g. `dmdancestudio.com`)
3. Follow the DNS instructions Vercel provides
