# 🚀 Deploy Your Portfolio to Vercel

This guide will help you deploy your portfolio website to Vercel in just a few minutes!

## 📋 Prerequisites

- A [GitHub](https://github.com) account
- A [Vercel](https://vercel.com) account (you can sign up with GitHub)

---

## 🎯 Deployment Methods

### **Method 1: Deploy via Vercel Dashboard (Recommended - Easiest)**

This is the simplest method and doesn't require any command-line tools.

#### Step 1: Push to GitHub

1. **Create a new repository on GitHub:**
   - Go to [github.com/new](https://github.com/new)
   - Name it `portfolio` or any name you prefer
   - Keep it **Public** or **Private** (both work with Vercel)
   - **Don't** initialize with README (we already have files)
   - Click **Create repository**

2. **Push your code to GitHub:**
   ```powershell
   # Initialize git (if not already done)
   git init
   
   # Add all files
   git add .
   
   # Commit your files
   git commit -m "Initial commit: Portfolio website"
   
   # Add your GitHub repository as remote (replace USERNAME and REPO_NAME)
   git remote add origin https://github.com/USERNAME/REPO_NAME.git
   
   # Push to GitHub
   git branch -M main
   git push -u origin main
   ```

#### Step 2: Deploy on Vercel

1. **Go to [vercel.com](https://vercel.com) and sign in** (use your GitHub account)

2. **Click "Add New..." → "Project"**

3. **Import your GitHub repository:**
   - You'll see a list of your GitHub repositories
   - Find your portfolio repository
   - Click **Import**

4. **Configure your project:**
   - **Project Name:** Choose a name (e.g., `kashif-portfolio`)
   - **Framework Preset:** Select **Other** (it's a static site)
   - **Root Directory:** Leave as `./`
   - **Build Command:** Leave empty
   - **Output Directory:** Leave empty
   - Click **Deploy**

5. **Wait for deployment** (usually takes 30-60 seconds)

6. **Your site is live!** 🎉
   - You'll get a URL like: `https://your-project-name.vercel.app`
   - You can also add a custom domain later

---

### **Method 2: Deploy via Vercel CLI**

If you prefer using the command line:

#### Step 1: Install Vercel CLI

```powershell
npm install -g vercel
```

#### Step 2: Login to Vercel

```powershell
vercel login
```

#### Step 3: Deploy

```powershell
# Navigate to your portfolio directory
cd c:\portfolio

# Deploy to Vercel
vercel
```

Follow the prompts:
- **Set up and deploy?** → Yes
- **Which scope?** → Select your account
- **Link to existing project?** → No
- **Project name?** → Enter a name (e.g., `kashif-portfolio`)
- **In which directory is your code located?** → `./`

#### Step 4: Deploy to Production

```powershell
vercel --prod
```

Your site is now live! 🚀

---

## 🌐 Custom Domain (Optional)

To use your own domain (e.g., `kashifkhan.com`):

1. Go to your project on Vercel Dashboard
2. Click **Settings** → **Domains**
3. Add your custom domain
4. Follow the DNS configuration instructions
5. Wait for DNS propagation (can take up to 48 hours)

---

## 🔄 Automatic Deployments

Once connected to GitHub:
- **Every push to `main` branch** → Automatic production deployment
- **Every pull request** → Preview deployment with unique URL
- **Instant rollbacks** if something goes wrong

---

## ✅ What's Included

Your portfolio is already configured with:
- ✨ **vercel.json** - Optimized routing and caching
- 📝 **.vercelignore** - Excludes unnecessary files
- 🎨 **Responsive design** - Works on all devices
- ⚡ **Fast loading** - Optimized assets
- 🔒 **HTTPS** - Automatic SSL certificate

---

## 🐛 Troubleshooting

### Images not loading?
- Make sure all images are in the `assets/` folder
- Check that image paths in HTML are correct (e.g., `assets/profile.jpg`)

### Styles not applying?
- Verify `style.css` is in the root directory
- Check the `<link>` tag in `index.html`

### 404 errors?
- Ensure `index.html` is in the root directory
- Check `vercel.json` configuration

---

## 📞 Need Help?

- **Vercel Documentation:** [vercel.com/docs](https://vercel.com/docs)
- **Vercel Support:** [vercel.com/support](https://vercel.com/support)
- **Community:** [github.com/vercel/vercel/discussions](https://github.com/vercel/vercel/discussions)

---

## 🎉 You're All Set!

Your portfolio is ready to be deployed. Choose your preferred method above and get your site live in minutes!

**Good luck!** 🚀
