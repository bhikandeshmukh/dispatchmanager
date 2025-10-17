# Deployment Guide - Vercel & GitHub

## Prerequisites
- GitHub account
- Vercel account (free tier works)
- Git installed on your computer

## Step 1: Push to GitHub

### If you haven't initialized git yet:
```bash
git init
git add .
git commit -m "Initial commit with all features"
```

### Create a new repository on GitHub:
1. Go to https://github.com/new
2. Name your repository (e.g., `dispatch-manager`)
3. Don't initialize with README (we already have one)
4. Click "Create repository"

### Push your code:
```bash
git remote add origin https://github.com/YOUR_USERNAME/dispatch-manager.git
git branch -M main
git push -u origin main
```

## Step 2: Deploy to Vercel

### Option A: Using Vercel Dashboard (Easiest)
1. Go to https://vercel.com
2. Sign in with GitHub
3. Click "Add New" → "Project"
4. Import your GitHub repository
5. Click "Deploy" (no configuration needed)
6. Wait 1-2 minutes for deployment
7. Your app is live! 🎉

### Option B: Using Vercel CLI
```bash
# Install Vercel CLI
npm i -g vercel

# Login to Vercel
vercel login

# Deploy
vercel

# For production deployment
vercel --prod
```

## Step 3: Configure Custom Domain (Optional)

1. In Vercel dashboard, go to your project
2. Click "Settings" → "Domains"
3. Add your custom domain
4. Update DNS records as instructed
5. Wait for DNS propagation (5-30 minutes)

## Step 4: Enable HTTPS (Automatic)

Vercel automatically provides HTTPS for all deployments. No configuration needed!

## Step 5: Test PWA Installation

### On Mobile:
1. Open your deployed URL in Chrome/Safari
2. Look for "Add to Home Screen" prompt
3. Install and test offline functionality

### On Desktop:
1. Open in Chrome
2. Look for install icon in address bar
3. Click to install as desktop app

## Updating Your App

### After making changes:
```bash
git add .
git commit -m "Description of changes"
git push
```

Vercel will automatically redeploy your app within 1-2 minutes!

## Troubleshooting

### Camera not working:
- Ensure you're accessing via HTTPS (Vercel provides this automatically)
- Check browser permissions
- Try different browser

### PWA not installing:
- Clear browser cache
- Check manifest.json is accessible at `/manifest.json`
- Verify service worker is registered in DevTools

### Data not persisting:
- Check browser's localStorage is enabled
- Don't use incognito/private mode
- Check browser storage quota

## Environment Variables (If needed in future)

In Vercel dashboard:
1. Go to Project Settings
2. Click "Environment Variables"
3. Add your variables
4. Redeploy

## Monitoring

- View deployment logs in Vercel dashboard
- Check Analytics tab for usage stats
- Monitor errors in browser console

## Support

For issues:
1. Check browser console for errors
2. Verify all files are committed to GitHub
3. Check Vercel deployment logs
4. Ensure HTTPS is enabled

## Your Live URLs

After deployment, you'll get:
- Production: `https://your-project.vercel.app`
- Preview: Automatic preview URLs for each commit
- Custom domain: If configured

---

**Note**: First deployment might take 2-3 minutes. Subsequent deployments are faster (30-60 seconds).
