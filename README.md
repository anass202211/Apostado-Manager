# Apostado Manager - Website Portal

This repository contains the official premium, dark-themed, responsive marketing website for the **Apostado Manager** Discord Bot. Built using semantic HTML5, modern vanilla CSS3 design variables, and pure JavaScript.

## Website Pages Included

- `/index.html` - The feature-rich Landing Page (dynamic canvas particles background, stats counters, accordion FAQ, glassmorphic cards).
- `/pages/support.html` - The Support Hub (categorized FAQ, support invite buttons, contact links).
- `/pages/privacy.html` - The Discord-compliant Privacy Policy.
- `/pages/terms.html` - The Discord-compliant Terms of Service.
- `/404.html` - Premium interactive 404 Error page.

---

## Deployment Guide: GitHub Pages

Follow these simple steps to host this static website on GitHub Pages for free.

### Step 1: Initialize Git and Upload to GitHub
1. Create a **new public repository** on GitHub named `apostado-manager-website` (do not initialize it with a README or gitignore).
2. Open a terminal in the folder containing these files (`apostado-manager-website/`) and execute the following commands:
   ```bash
   # Initialize local git repository
   git init

   # Stage all project files
   git add .

   # Commit files
   git commit -m "feat: initial commit premium website"

   # Rename branch to main
   git branch -M main

   # Link your local repository to GitHub (replace with your real repository URL)
   git remote add origin https://github.com/YOUR_USERNAME/apostado-manager-website.git

   # Push files to GitHub
   git push -u origin main
   ```

### Step 2: Enable GitHub Pages
1. Go to your repository page on GitHub.
2. Click on the **Settings** tab (the gear icon on the right side of the sub-navigation menu).
3. In the left sidebar, locate the **Code and automation** section and click on **Pages**.
4. Under the **Build and deployment** section, look for the **Source** setting and verify it is set to **Deploy from a branch**.
5. Under **Branch**, select `main` from the dropdown list, and set the folder parameter to `/ (root)`.
6. Click the **Save** button.

### Step 3: Publish and Access Your Site
1. GitHub Actions will automatically start a deployment worker. Wait 1-2 minutes.
2. Refresh the **Pages** settings screen. You will see a notification box at the top stating:
   > Your site is live at `https://YOUR_USERNAME.github.io/apostado-manager-website/`
3. Click the link to test your live, production-ready website!

---

## Custom Domains Configuration (Optional)

To serve the website under a custom domain (e.g., `https://apos.gg`):
1. In the **GitHub Pages** settings screen, scroll down to **Custom domain**.
2. Type your domain name (e.g., `apos.gg`) and click **Save**.
3. Configure the DNS settings with your domain registrar:
   - Create a **CNAME record** pointing your `www` subdomain to `YOUR_USERNAME.github.io`.
   - Create **A records** pointing your root apex domain directly to GitHub's server IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
4. Once DNS propagation completes, check **Enforce HTTPS** in the GitHub Pages settings to secure your custom domain.
