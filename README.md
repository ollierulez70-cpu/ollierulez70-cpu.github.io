# The Log — GitHub Pages Hosting Guide

This file is your full measurement tracker app. Follow the steps below to host it for free on GitHub Pages so you can access it from any browser, any device, via a private URL.

---

## What You Need
- A free GitHub account (github.com)
- 5 minutes

---

## Step-by-Step Setup

### 1. Create a GitHub account
Go to **github.com** and sign up if you don't have an account. Use any username — it will appear in your URL, so pick something neutral if privacy matters (e.g. `mylogapp` instead of your real name).

### 2. Create a new repository
- Click the **+** icon in the top right → **New repository**
- Repository name: `thelog` (or anything you want — it becomes part of the URL)
- Set visibility to **Private** ← important for privacy
- Do NOT initialize with README (you'll upload your own files)
- Click **Create repository**

### 3. Upload your files
- On the new repository page, click **uploading an existing file**
- Drag and drop `index.html` from this folder
- Also drag and drop `README.md` if you want
- Scroll down, click **Commit changes**

### 4. Enable GitHub Pages
- Go to your repository → **Settings** tab
- Scroll down to **Pages** in the left sidebar
- Under **Source**, select **Deploy from a branch**
- Branch: `main` | Folder: `/ (root)`
- Click **Save**

### 5. Wait ~60 seconds, then visit your app
Your app will be live at:
```
https://YOUR-USERNAME.github.io/thelog/
```
Replace `YOUR-USERNAME` with your actual GitHub username and `thelog` with whatever you named your repo.

---

## Privacy Notes

**Private repo = code is private, but the Pages URL is still publicly accessible.**

If you want the URL itself to be private (not accessible without login):
- GitHub Pages on free accounts does NOT support password protection
- Options for true privacy:
  1. **Use it locally** — just open `index.html` directly in Safari (no hosting needed, most private option)
  2. **Use Cloudflare Access** — free service that adds a login gate in front of any URL
  3. **Netlify + password protection** — free tier supports basic auth

For most people, a private repo with an obscure URL is sufficient — nobody will stumble across it.

---

## Updating the App

When a new version of the app is available:
1. Download the new `tracker.html`
2. Rename it to `index.html`
3. Go to your GitHub repo → click `index.html` → click the pencil (edit) icon → or just drag the new file in and commit
4. GitHub Pages auto-deploys within ~60 seconds

---

## Data & Backups

Your data is stored in the **browser's localStorage** on whatever device you use to visit the URL. This means:
- Data on your iPhone ≠ data on your laptop (they don't sync)
- If you clear browser data, your entries are gone
- **Use the Export JSON button in the History tab regularly** and save the file to iCloud Drive or your Files app

To move data between devices: export on one device, import on the other.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Page not found after enabling Pages | Wait 2 minutes and hard-refresh |
| App loads but data is gone | You're on a different browser/device — use Import JSON |
| URL looks wrong | Check Settings → Pages to confirm the branch and folder |
| Want a custom domain | Settings → Pages → Custom domain (requires a domain you own) |
