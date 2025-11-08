# Deploying Old to Gold Website to Vercel

## Method 1: Using Vercel Web Interface (Recommended for beginners)

### Step 1: Push to GitHub
1. Create a new repository on GitHub (https://github.com/new)
2. Name it "old-to-gold" or "oldtogold"
3. Don't initialize with README, .gitignore, or license
4. Copy the repository URL

### Step 2: Connect to GitHub
Run these commands in your terminal:
```bash
git remote add origin YOUR_GITHUB_REPO_URL
git branch -M main
git push -u origin main
```

### Step 3: Deploy on Vercel
1. Go to https://vercel.com
2. Sign up or log in (you can use your GitHub account)
3. Click "Add New Project"
4. Import your GitHub repository
5. Vercel will auto-detect the settings
6. Click "Deploy"
7. Wait for deployment to complete
8. Your site will be live at: `https://your-project-name.vercel.app`

## Method 2: Using Vercel CLI

### Step 1: Install Vercel CLI
```bash
npm install -g vercel
```

### Step 2: Login to Vercel
```bash
vercel login
```

### Step 3: Deploy
```bash
vercel
```

Follow the prompts:
- Set up and deploy? **Yes**
- Which scope? (Select your account)
- Link to existing project? **No**
- Project name? **old-to-gold** (or press Enter for default)
- Directory? **./** (press Enter)
- Override settings? **No**

### Step 4: Deploy to Production
```bash
vercel --prod
```

Your site will be live at: `https://old-to-gold.vercel.app`

## Custom Domain (Optional)
1. Go to your Vercel project dashboard
2. Click on "Settings" → "Domains"
3. Add your custom domain (e.g., oldtogold.com)
4. Follow the DNS configuration instructions

## Notes
- Your website will automatically redeploy when you push changes to GitHub
- Vercel provides free SSL certificates
- The site is optimized and served via CDN globally

