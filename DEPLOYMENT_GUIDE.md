# AGI Automations Portfolio - Deployment Guide

## 🎯 Quick Start (Recommended: Netlify - 5 minutes)

### Step 1: Prepare Files

1. Move `landing page/landing page.html` to root and rename to `index.html`
2. Update the following links in `index.html`:

```html
<!-- Current (broken) links -->
<a href="readiness_gate_v2.html">           <!-- ❌ File doesn't exist -->
<a href="pipeline_scoreboard_v2.html">      <!-- ❌ File doesn't exist -->
<a href="health_tracker_v3.html">           <!-- ❌ File doesn't exist -->
<a href="Experiment Desision Pad v2.html">  <!-- ✅ EXISTS -->
<a href="client_assessment_report_v2.html"> <!-- ❌ File doesn't exist -->

<!-- Replace with actual files -->
<a href="Property Listing Readiness Gate.html">
<a href="Pipeline Scoreboard.html">
<a href="Landlord and Vendor Health Tracker.html">
<a href="Experiment Desision Pad v2.html">
<!-- Remove or comment out client_assessment_report_v2.html link -->
```

### Step 2: Deploy to Netlify (FREE)

1. **Sign up:** Go to https://netlify.com (use GitHub login)

2. **Deploy:**
   - Click "Add new site" → "Deploy manually"
   - Drag your entire `Instruments` folder
   - Site goes live instantly at `https://random-name-123.netlify.app`

3. **Custom Domain:**
   - Site settings → Domain management
   - Add your domain: `portfolio.yourdomain.com` or `tools.yourdomain.com`
   - Update DNS at your registrar:
     ```
     CNAME  portfolio  random-name-123.netlify.app
     ```

4. **Done!** Free SSL certificate auto-configured.

---

## 🚀 Alternative: GitHub Pages (FREE)

### Step 1: Create Repository

```bash
cd "c:\VS Repositry\Instruments"
git init
git add .
git commit -m "Initial portfolio deployment"
```

### Step 2: Push to GitHub

1. Create new repo at https://github.com/new
   - Name: `agi-automations-portfolio`
   - Public/Private: Your choice

2. Push code:
```bash
git remote add origin https://github.com/YOUR-USERNAME/agi-automations-portfolio.git
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Repo → Settings → Pages
2. Source: `main` branch / `root` folder
3. Save
4. Site live at: `https://YOUR-USERNAME.github.io/agi-automations-portfolio`

### Step 4: Custom Domain (Optional)

1. Settings → Pages → Custom domain: `portfolio.yourdomain.com`
2. Add DNS record:
   ```
   Type: CNAME
   Name: portfolio
   Value: YOUR-USERNAME.github.io
   ```

---

## 📁 File Structure Checklist

Before deploying, ensure this structure:

```
Instruments/
├── index.html                                    (renamed from landing page.html)
├── Property Listing Readiness Gate.html          ✅ EXISTS
├── Pipeline Scoreboard.html                      ✅ EXISTS
├── Landlord and Vendor Health Tracker.html       ✅ EXISTS
├── Experiment Desision Pad v2.html               ✅ EXISTS
└── README.md                                     (optional - about your tools)
```

---

## 🔧 Pre-Deployment Fixes Needed

### Fix 1: Update Landing Page Links

Edit `index.html` (currently `landing page/landing page.html`):

**Line 84:** Change to:
```html
<a href="Property Listing Readiness Gate.html" class="group block...">
```

**Line 105:** Change to:
```html
<a href="Pipeline Scoreboard.html" class="group block...">
```

**Line 126:** Change to:
```html
<a href="Landlord and Vendor Health Tracker.html" class="group block...">
```

**Lines 168-186:** Either:
- Remove this card entirely (file doesn't exist), OR
- Create `client_assessment_report_v2.html` later

### Fix 2: Rename Files (Optional - Better URLs)

For cleaner URLs, rename files to remove spaces:

```bash
mv "Property Listing Readiness Gate.html" "property-listing-readiness.html"
mv "Landlord and Vendor Health Tracker.html" "landlord-health-tracker.html"
mv "Pipeline Scoreboard.html" "pipeline-scoreboard.html"
mv "Experiment Desision Pad v2.html" "experiment-decision-pad.html"
```

Then update links in `index.html` accordingly.

---

## 💰 Cost Comparison

| Option | Cost | SSL | Custom Domain | Speed |
|--------|------|-----|---------------|-------|
| **Netlify** | FREE | ✅ Auto | ✅ Yes | ⚡⚡⚡ Fast CDN |
| **GitHub Pages** | FREE | ✅ Auto | ✅ Yes | ⚡⚡ Good |
| **Vercel** | FREE | ✅ Auto | ✅ Yes | ⚡⚡⚡ Fast CDN |
| **Cloudflare Pages** | FREE | ✅ Auto | ✅ Yes | ⚡⚡⚡ Fastest CDN |

**Recommendation:** Start with **Netlify** (easiest) or **GitHub Pages** (version control).

---

## 🎨 Next Steps After Deployment

1. **Add Analytics:**
   - Google Analytics
   - Plausible (privacy-friendly)

2. **Add Contact Form:**
   - Netlify Forms (free)
   - Formspree

3. **SEO Optimization:**
   - Add meta descriptions
   - Open Graph tags for social sharing

4. **Performance:**
   - All your tools are already optimized (static HTML)!

---

## 🆘 Troubleshooting

### "404 Not Found" when clicking tools
- **Cause:** Filename mismatch in links
- **Fix:** Update hrefs in `index.html` to match actual filenames

### Custom domain not working
- **Cause:** DNS not propagated (takes 24-48 hours)
- **Fix:** Wait, or check DNS with `nslookup portfolio.yourdomain.com`

### Tools not loading CSS
- **Cause:** External CDN links blocked
- **Fix:** Tools use CDN (Tailwind, FontAwesome) - should work everywhere

---

## 📞 Support Resources

- **Netlify Docs:** https://docs.netlify.com
- **GitHub Pages Docs:** https://docs.github.com/pages
- **DNS Setup Guide:** https://www.netlify.com/blog/custom-domains

---

**Ready to deploy? Start with Step 1 above! 🚀**
