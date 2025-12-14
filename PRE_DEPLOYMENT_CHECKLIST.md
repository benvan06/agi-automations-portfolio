# ✅ Pre-Deployment Checklist

Use this checklist before deploying to GitHub + Cloudflare.

---

## 📁 Files Ready for Deployment

### ✅ Core Portfolio Files
- [x] **index.html** - Landing page with correct links
- [x] **Property Listing Readiness Gate.html** - Compliance tool
- [x] **Landlord and Vendor Health Tracker.html** - Churn prediction
- [x] **Pipeline Scoreboard.html** - Sales dashboard
- [x] **Experiment Desision Pad v2.html** - A/B test validator

### ✅ Documentation Files
- [x] **README.md** - Portfolio documentation
- [x] **QUICK_START.md** - Fast deployment guide
- [x] **DEPLOYMENT_GUIDE.md** - Comprehensive options
- [x] **GITHUB_CLOUDFLARE_SETUP.md** - GitHub + Cloudflare guide
- [x] **.gitignore** - Git ignore rules

### 📂 Optional Files (Not Needed for Deployment)
- [ ] **App.tsx** - Can be excluded (not used in static site)
- [ ] **landing page/** folder - Old version (we created index.html)
- [ ] **.claude/** folder - Development files (auto-ignored)

---

## 🎯 Ready to Deploy? Follow These Steps:

### Step 1: Stage Your Files (1 minute)

```bash
cd "c:\VS Repositry\Instruments"

# Add all deployment files
git add .gitignore
git add index.html
git add "Property Listing Readiness Gate.html"
git add "Landlord and Vendor Health Tracker.html"
git add "Pipeline Scoreboard.html"
git add "Experiment Desision Pad v2.html"
git add README.md
git add QUICK_START.md
git add DEPLOYMENT_GUIDE.md
git add GITHUB_CLOUDFLARE_SETUP.md

# Or simply add everything:
git add .
```

### Step 2: Create First Commit

```bash
git commit -m "Initial deployment - AGI Automations portfolio with 4 tools"
```

### Step 3: Create GitHub Repository

1. Go to: https://github.com/new
2. Repository name: `agi-automations-portfolio`
3. Visibility: **Public**
4. DO NOT initialize with README
5. Click "Create repository"

### Step 4: Push to GitHub

```bash
# Replace YOUR-USERNAME with your GitHub username
git remote add origin https://github.com/YOUR-USERNAME/agi-automations-portfolio.git
git branch -M main
git push -u origin main
```

### Step 5: Deploy to Cloudflare Pages

1. Go to: https://dash.cloudflare.com
2. Workers & Pages → Create → Pages → Connect to Git
3. Select your repository: `agi-automations-portfolio`
4. Configure:
   - Framework preset: **None**
   - Build command: (leave empty)
   - Build output directory: **/**
5. Click "Save and Deploy"

### Step 6: Verify Deployment

Your site will be live at:
`https://agi-automations-portfolio.pages.dev`

Test all 4 tools:
- [ ] Click "Listing Readiness Gate" - opens correct tool
- [ ] Click "Pipeline Scoreboard" - opens correct tool
- [ ] Click "Landlord Health Tracker" - opens correct tool
- [ ] Click "Experiment Decision Pad" - opens correct tool

---

## 🧹 Optional Cleanup (Before Deployment)

### Remove Unnecessary Files

If you want a cleaner repo, you can exclude these:

```bash
# Add to .gitignore before committing
echo "App.tsx" >> .gitignore
echo "landing page/" >> .gitignore
echo ".claude/" >> .gitignore
```

Then commit:
```bash
git add .gitignore
git commit -m "Clean up repository"
```

---

## 🎨 Personalization Checklist

Before going live, consider customizing:

### Update Contact Information

Edit `index.html` (line ~235):
```html
<p class="text-xs text-slate-400 mt-2">
    © 2025 AGI Automations •
    <a href="mailto:YOUR-EMAIL@domain.com">Contact</a>
</p>
```

### Add Social Links

```html
<a href="https://linkedin.com/in/yourprofile" class="hover:text-indigo-600">
    <i class="fab fa-linkedin"></i> LinkedIn
</a>
<a href="https://github.com/yourusername" class="hover:text-indigo-600">
    <i class="fab fa-github"></i> GitHub
</a>
```

### Update Meta Tags for SEO

In `index.html` `<head>`:
```html
<meta name="author" content="Your Name">
<meta property="og:title" content="AGI Automations - Data Infrastructure Portfolio">
<meta property="og:description" content="Custom-built operational tools for real estate agencies">
<meta property="og:url" content="https://portfolio.yourdomain.com">
```

---

## 🔍 Final Verification

Before pushing to GitHub, test locally:

```bash
# Start local server
cd "c:\VS Repositry\Instruments"
python -m http.server 8000

# Or use VS Code Live Server extension
```

Visit: http://localhost:8000

**Test Checklist:**
- [ ] Landing page loads correctly
- [ ] All 4 tool cards are visible
- [ ] Clicking each card opens the correct tool
- [ ] Tools are functional (try entering data)
- [ ] Mobile responsive (resize browser window)
- [ ] No console errors (press F12)

---

## 📊 Git Status Overview

Current files to be committed:

```bash
# Check what will be committed
git status

# Should show:
# - index.html
# - 4 tool HTML files
# - 4 documentation MD files
# - .gitignore
```

**Total size:** ~350KB (very lightweight!)

---

## 🚀 You're Ready to Deploy!

All files are prepared and tested. Follow the steps above to:
1. ✅ Push to GitHub
2. ✅ Deploy to Cloudflare Pages
3. ✅ Go live in ~5 minutes!

**Need detailed instructions?** Open [GITHUB_CLOUDFLARE_SETUP.md](GITHUB_CLOUDFLARE_SETUP.md)

---

## 🎉 After Deployment

Once live, share your portfolio:
- [ ] Add to LinkedIn profile
- [ ] Include in email signature
- [ ] Add to business cards (QR code)
- [ ] Share on Twitter/X
- [ ] Email to potential clients

**Your live URL will be:**
- `https://agi-automations-portfolio.pages.dev` (Cloudflare)
- `https://portfolio.yourdomain.com` (with custom domain)

---

**Ready? Let's deploy! 🚀**

Open your terminal and start with Step 1 above!
