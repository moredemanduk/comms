# 🚀 Connecting to GitHub & Vercel

This guide will walk you through connecting your project to GitHub and deploying it on Vercel.

## 📋 Prerequisites

- GitHub account
- Vercel account (sign up at [vercel.com](https://vercel.com))

---

## 1️⃣ Connect to GitHub

### Step 1: Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **"+"** icon in the top right → **"New repository"**
3. Name your repository (e.g., `comms`)
4. **Don't** initialize with README, .gitignore, or license (we already have these)
5. Click **"Create repository"**

### Step 2: Connect Your Local Repository

✅ **Already done!** Your repository is connected to:
- **Repository:** [moredemanduk/comms](https://github.com/moredemanduk/comms.git)
- **Remote:** `git@github.com:moredemanduk/comms.git`
- **Branch:** `main` (pushed and tracking)

---

## 2️⃣ Connect to Vercel

### Option A: Via Vercel Dashboard (Recommended)

1. Go to [vercel.com](https://vercel.com) and sign in
2. Click **"Add New..."** → **"Project"**
3. Click **"Import Git Repository"**
4. Select your GitHub repository (`comms`)
5. Vercel will auto-detect Next.js settings
6. Click **"Deploy"**

That's it! Vercel will:
- Build your project
- Deploy it to a production URL
- Set up automatic deployments on every push to `main`

### Option B: Via Vercel CLI

```bash
# Install Vercel CLI globally
npm i -g vercel

# Login to Vercel
vercel login

# Deploy (from project root)
vercel

# Follow the prompts to link your project
```

---

## 3️⃣ Automatic Deployments

Once connected, Vercel will automatically:
- ✅ Deploy every push to `main` branch
- ✅ Create preview deployments for pull requests
- ✅ Run your build command (`npm run build`)
- ✅ Provide you with a production URL

---

## 🔧 Troubleshooting

### GitHub Connection Issues
- Make sure you've added the remote: `git remote -v`
- Verify your GitHub credentials are set up correctly
- Check that you have push access to the repository

### Vercel Deployment Issues
- Ensure your `package.json` has a `build` script
- Check that Next.js is properly configured
- Review build logs in the Vercel dashboard

---

## 📚 Next Steps

- Customize your app in `app/page.tsx`
- Add environment variables in Vercel dashboard (Settings → Environment Variables)
- Set up custom domains (Vercel dashboard → Settings → Domains)
- Configure branch protection rules in GitHub for production deployments

---

**Need help?** Check out:
- [Vercel Documentation](https://vercel.com/docs)
- [Next.js Documentation](https://nextjs.org/docs)
- [GitHub Documentation](https://docs.github.com)

