# Rodrigo Yepez-Lopez Academic Portfolio

## 🚀 Quick Setup Instructions

You already have the template at `E:\academicpages.github.io`. Follow these steps:

---

## Step 1: Copy These Files to Your Template

Copy the contents of this folder to your template directory:

```
rodrigo-site-files/
├── _config.yml              → E:\academicpages.github.io\_config.yml (REPLACE)
├── _data/
│   └── navigation.yml       → E:\academicpages.github.io\_data\navigation.yml (REPLACE)
├── _pages/
│   ├── about.md            → E:\academicpages.github.io\_pages\about.md (REPLACE)
│   ├── cv.md               → E:\academicpages.github.io\_pages\cv.md (ADD NEW)
│   ├── publications.md     → E:\academicpages.github.io\_pages\publications.md (REPLACE)
│   └── portfolio.md        → E:\academicpages.github.io\_pages\portfolio.md (REPLACE)
├── _publications/           → E:\academicpages.github.io\_publications\ (REPLACE ALL)
│   ├── 2021-12-15-proton-radiotherapy.md
│   ├── 2022-12-17-cloud-classification.md
│   ├── 2022-12-17-lstm-pulmonary.md
│   └── 2023-12-15-concept-drift.md
├── _portfolio/              → E:\academicpages.github.io\_portfolio\ (REPLACE ALL)
│   ├── portfolio-1-dementia.md
│   ├── portfolio-2-cancer-db.md
│   ├── portfolio-3-transcription.md
│   ├── portfolio-4-mlops.md
│   └── portfolio-5-nasa.md
└── files/
    └── Rodrigo_YepezLopez_CV.pdf → E:\academicpages.github.io\files\ (ADD)
```

---

## Step 2: Update _config.yml with Your Info

Open `E:\academicpages.github.io\_config.yml` and update these lines:

```yaml
# Line ~10 - Update when you have your domain
url: "https://YOUR_GITHUB_USERNAME.github.io"  

# Line ~12 - Your GitHub repo
repository: "YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME.github.io"

# Line ~52 - Your GitHub username
github: "YOUR_GITHUB_USERNAME"

# Line ~67 - Your LinkedIn (just the username part from linkedin.com/in/USERNAME)
linkedin: "YOUR_LINKEDIN_USERNAME"
```

---

## Step 3: Add Your Profile Photo

1. Get a professional headshot (square works best, at least 300x300 pixels)
2. Name it `profile.png` (or `profile.jpg`)
3. Place it in: `E:\academicpages.github.io\images\profile.png`

---

## Step 4: Run Locally (Test Before Deploying)

### Option A: Using Ruby (Recommended for Windows)

Open PowerShell/CMD in `E:\academicpages.github.io`:

```powershell
# Install Ruby dependencies (first time only)
bundle install

# If you get permission errors, run this first:
bundle config set --local path 'vendor/bundle'
bundle install

# Start the local server
bundle exec jekyll serve -l -H localhost
```

Open browser: **http://localhost:4000**

### Option B: Using Docker

```powershell
cd E:\academicpages.github.io
docker compose up
```

Open browser: **http://localhost:4000**

---

## Step 5: Deploy to GitHub Pages

### 5.1 Create GitHub Repository

1. Go to https://github.com/new
2. Repository name: `YOUR_GITHUB_USERNAME.github.io` (MUST match your username)
3. Make it **Public**
4. Don't initialize with README

### 5.2 Push Your Code

```powershell
cd E:\academicpages.github.io

# Initialize git (if not already)
git init

# Add all files
git add .

# Commit
git commit -m "Initial portfolio site"

# Add remote (replace YOUR_GITHUB_USERNAME)
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME.github.io.git

# Push
git push -u origin main
```

### 5.3 Enable GitHub Pages

1. Go to your repo on GitHub
2. Settings → Pages
3. Source: **Deploy from a branch**
4. Branch: **main** (or gh-pages if it exists)
5. Save

Your site will be live at: `https://YOUR_GITHUB_USERNAME.github.io`

---

## Step 6: Connect Custom Domain (rodrigoyepez.com)

### 6.1 Buy Domain
- Go to [Namecheap](https://namecheap.com) or [GoDaddy](https://godaddy.com)
- Purchase `rodrigoyepez.com` (~$10-15/year)

### 6.2 Configure DNS (in Namecheap)
1. Log into Namecheap → Domain List → Manage
2. Go to **Advanced DNS**
3. Delete existing records
4. Add these:

| Type | Host | Value | TTL |
|------|------|-------|-----|
| A | @ | 185.199.108.153 | Automatic |
| A | @ | 185.199.109.153 | Automatic |
| A | @ | 185.199.110.153 | Automatic |
| A | @ | 185.199.111.153 | Automatic |
| CNAME | www | YOUR_GITHUB_USERNAME.github.io | Automatic |

### 6.3 Configure GitHub
1. In your repo, create file: `CNAME` (no extension)
2. Contents: `rodrigoyepez.com`
3. Or: Settings → Pages → Custom domain → Enter `rodrigoyepez.com`
4. Check "Enforce HTTPS" (after DNS propagates)

### 6.4 Update _config.yml
```yaml
url: "https://rodrigoyepez.com"
```

Commit and push the change.

---

## File Structure Reference

```
academicpages.github.io/
├── _config.yml          # Main site configuration
├── _data/
│   └── navigation.yml   # Top menu links
├── _pages/
│   ├── about.md        # Homepage (/)
│   ├── cv.md           # CV page (/cv/)
│   ├── publications.md # Publications list (/publications/)
│   └── portfolio.md    # Portfolio list (/portfolio/)
├── _publications/       # Individual publication pages
├── _portfolio/          # Individual project pages
├── files/               # Downloadable files (PDFs, etc.)
├── images/              # Images (profile photo, project images)
└── CNAME               # Custom domain file (create when ready)
```

---

## Troubleshooting

### "bundle install" fails
```powershell
bundle config set --local path 'vendor/bundle'
bundle install
```

### Site not updating after push
- GitHub Pages can take 1-10 minutes to rebuild
- Check Actions tab for build status

### Custom domain not working
- DNS propagation can take up to 48 hours
- Use https://dnschecker.org to verify

### Images not showing
- Make sure images are in `/images/` folder
- Use correct path: `/images/profile.png`

---

## Next Steps

1. ✅ Copy files to template
2. ✅ Update _config.yml with your usernames
3. ✅ Add profile photo
4. ✅ Test locally
5. ✅ Deploy to GitHub Pages
6. ✅ (Optional) Connect custom domain

**Questions?** Feel free to ask!
