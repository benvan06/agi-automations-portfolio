# AGI Automations - Data Infrastructure Portfolio

> Custom-built operational tools for real estate agencies to reduce churn, accelerate pipeline velocity, and ensure compliance.

## 🚀 Live Demo

[View Portfolio](https://your-domain.com) *(Update after deployment)*

---

## 🛠️ Tools Included

### 1. **Property Listing Readiness Gate**
- **Purpose:** Pre-flight compliance checklist ensuring listings meet portal requirements
- **Features:**
  - 6 required sections (Property Data, Photos, EPC, AML/KYC, Legal, Risk)
  - Role-based approval workflow
  - SHA-256 hashing for audit trails
  - GO/NO-GO decision logic
- **Tech:** React 18, TailwindCSS, LocalStorage for baseline tracking

### 2. **Landlord & Vendor Health Tracker**
- **Purpose:** Churn prediction engine identifying at-risk accounts
- **Features:**
  - Multi-factor health scoring (engagement, maintenance, sentiment, tenure)
  - Z-score normalization for fair comparison
  - P1 renewal risk flagging (≤60 days + low score)
  - ARR-weighted risk ranking
  - Owner-based account segmentation
- **Tech:** React 18, Statistical analysis, CSV export

### 3. **Pipeline Scoreboard**
- **Purpose:** Weekly Business Review (WBR) dashboard for sales forecasting
- **Features:**
  - Pipeline velocity tracking
  - Deal stage progression
  - Revenue forecasting
  - Team performance metrics
- **Tech:** React 18, TailwindCSS, Data visualization

### 4. **Experiment Decision Pad**
- **Purpose:** A/B test validation with statistical rigor
- **Features:**
  - Statistical significance calculation
  - Sample size estimation
  - Risk guardrails
  - Confidence interval visualization
- **Tech:** React 18, Statistical formulas, Interactive calculator

---

## 📦 Deployment

### Quick Deploy (5 minutes)

**Option 1: Netlify (Recommended)**
```bash
# 1. Visit netlify.com and sign up
# 2. Drag the "Instruments" folder to deploy
# 3. Site live instantly with free SSL + CDN
```

**Option 2: GitHub Pages**
```bash
# 1. Create repository
git init
git add .
git commit -m "Portfolio deployment"
git remote add origin https://github.com/YOUR-USERNAME/agi-portfolio.git
git push -u origin main

# 2. Enable Pages in repo settings
# 3. Site live at: YOUR-USERNAME.github.io/agi-portfolio
```

See [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md) for detailed instructions.

---

## 🏗️ Technical Architecture

**Stack:**
- **Frontend:** Pure HTML/CSS/JS with React 18 (CDN)
- **Styling:** TailwindCSS (CDN)
- **Icons:** FontAwesome 6
- **Fonts:** Google Fonts (Inter)
- **Storage:** LocalStorage for baseline persistence
- **Deployment:** Static hosting (no backend required)

**Why Static?**
- ✅ Zero server costs
- ✅ Instant global CDN distribution
- ✅ No security vulnerabilities (no backend)
- ✅ Works offline (after first load)
- ✅ Easy to customize per-client

---

## 📊 Use Cases

### For Real Estate Agencies:
- **Compliance Teams:** Readiness Gate prevents portal rejections
- **Lettings Managers:** Health Tracker reduces landlord churn
- **Sales Directors:** Pipeline Scoreboard forecasts revenue
- **Marketing Teams:** Experiment Pad validates campaign tests

### For Consultants:
- **Portfolio Showcase:** Demonstrate technical capabilities
- **Client Demos:** Customize with prospect's data
- **Proof of Value:** Show ROI before full implementation

---

## 🎨 Customization

Each tool is self-contained in a single HTML file. To customize:

1. **Branding:** Update colors in Tailwind config (lines 14-30)
2. **Data:** Replace sample JSON with client data
3. **Logic:** Adjust scoring weights or thresholds
4. **Export:** Add client logo, white-label footer

Example: Change primary color from indigo to client's brand:
```javascript
tailwind.config = {
  theme: {
    extend: {
      colors: {
        brand: {
          primary: '#YOUR-COLOR',
          accent: '#YOUR-ACCENT'
        }
      }
    }
  }
}
```

---

## 📝 File Structure

```
Instruments/
├── index.html                                # Portfolio landing page ✅
├── Property Listing Readiness Gate.html      # Compliance tool ✅
├── Landlord and Vendor Health Tracker.html   # Churn prediction ✅
├── Pipeline Scoreboard.html                  # Sales dashboard ✅
├── Experiment Desision Pad v2.html           # A/B test validator ✅
├── README.md                                 # This file
└── DEPLOYMENT_GUIDE.md                       # Setup instructions
```

---

## 🔒 Data Privacy

**All tools run 100% client-side:**
- ✅ No data sent to external servers
- ✅ No analytics tracking (unless you add it)
- ✅ No cookies (except LocalStorage for baselines)
- ✅ No third-party data sharing

**LocalStorage usage:**
- Readiness Gate: Baseline snapshots for audit diffs
- Health Tracker: Baseline snapshots for tier movements
- All stored data remains on user's device

---

## 📈 Roadmap

**Potential Enhancements:**
- [ ] Backend integration (API endpoints for CRM data)
- [ ] Multi-user collaboration (shared baselines)
- [ ] Email notifications (Netlify Functions)
- [ ] PDF export (client-side generation)
- [ ] Mobile apps (React Native wrapper)

---

## 📞 Support

**Documentation:**
- [Deployment Guide](DEPLOYMENT_GUIDE.md)
- [Netlify Docs](https://docs.netlify.com)
- [GitHub Pages Docs](https://docs.github.com/pages)

**Contact:**
- Email: your-email@domain.com
- Website: https://your-domain.com

---

## 📄 License

© 2025 AGI Automations. All rights reserved.

**Usage Terms:**
- ✅ Use for client projects (with attribution)
- ✅ Customize for specific agencies
- ✅ White-label for consulting work
- ❌ Resell as standalone SaaS without permission

---

## 🙏 Credits

**Built with:**
- React 18 (Facebook)
- TailwindCSS (Tailwind Labs)
- FontAwesome (Fonticons)
- Google Fonts (Google)

**Inspired by:**
- Amazon's 6-pager culture
- Stripe's operational rigor
- Airbnb's data-driven decision making

---

**Ready to deploy your portfolio? Start with [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md)! 🚀**
