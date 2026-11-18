# SupeRR Selector | IPL & T20I Pressure Dashboard

A transparent, pre-delivery pressure performance dashboard and reliability-adjusted player rankings for IPL and T20I (2022 onward).

## 🚀 Features
- **Pressure Scoring Model**: Transparent heuristics for chase and first innings measuring pre-delivery situational pressure.
- **Player Rankings**: Reliability-weighted rankings for batters and bowlers in high-pressure scenarios (score ≥ 60).
- **Head-to-Head Comparison**: Compare any two players across pressure strike rate / economy vs. normal baseline.
- **Lightweight & Fast**: Self-contained static web application with zero external build dependencies.

## 🌐 Deployment Instructions

### Deploy on GitHub & GitHub Pages
1. Create a repository on [GitHub](https://github.com/new) named `rr_ipl` (or `superr-selector`).
2. Push this local repository to GitHub:
   ```bash
   git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/<REPO_NAME>.git
   git branch -M main
   git push -u origin main
   ```
3. (Optional) Turn on **GitHub Pages**:
   - Go to your repository **Settings** -> **Pages**.
   - Under **Build and deployment** -> **Branch**, select `main` and root `/`.
   - Click **Save**. Your site will be live at `https://<YOUR_GITHUB_USERNAME>.github.io/<REPO_NAME>/`.

---

### Deploy on Render
This repository includes a `render.yaml` blueprint for automatic setup on [Render](https://render.com).

#### Option A: One-Click via Render Blueprint
1. Log in to [Render Dashboard](https://dashboard.render.com).
2. Click **New +** -> **Blueprint**.
3. Connect your GitHub repository.
4. Render will automatically detect `render.yaml` and configure the static site. Click **Apply**.

#### Option B: Manual Static Site Setup
1. Log in to [Render Dashboard](https://dashboard.render.com).
2. Click **New +** -> **Static Site**.
3. Connect your GitHub repository.
4. Fill in the deployment settings:
   - **Name**: `rr-ipl-selector` (or your preferred name)
   - **Branch**: `main`
   - **Build Command**: *(leave empty)*
   - **Publish Directory**: `.`
5. Click **Create Static Site**. Render will assign you a live `.onrender.com` URL.
