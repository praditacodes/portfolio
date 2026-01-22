# Quick Deployment Guide for praditabadal.com.np

## 🎯 Fastest Way: GitHub Pages

### Step 1: Create GitHub Repository
1. Go to https://github.com/new
2. Repository name: `portfolio` (or any name)
3. Make it **Public**
4. Click "Create repository"

### Step 2: Upload Files
**Option A: Using GitHub Website**
1. Click "uploading an existing file"
2. Drag and drop ALL your portfolio files
3. Commit changes

**Option B: Using Git (Command Line)**
```bash
cd C:\Users\lenovo\Desktop\portfolio
git init
git add .
git commit -m "Deploy portfolio"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository
2. Click **Settings** → **Pages**
3. Under "Source": Select **main** branch → **/ (root)**
4. Click **Save**

### Step 4: Add Custom Domain
1. In Pages settings, add domain: `praditabadal.com.np`
2. The `CNAME` file is already created in your project ✅
3. Update DNS at your domain registrar:
   - **CNAME Record**: `@` → `YOUR_USERNAME.github.io`
   - Wait 24-48 hours for DNS to propagate

### Step 5: Your Site Will Be Live At
- GitHub URL: `https://YOUR_USERNAME.github.io`
- Custom Domain: `https://praditabadal.com.np` (after DNS updates)

---

## ⚠️ Important: Update Contact Form

Before deploying, update `contact.html` line 19:
1. Sign up at https://formspree.io
2. Create a new form
3. Copy your form ID
4. Replace `your-form-id` in contact.html with your actual form ID

---

## ✅ Checklist Before Going Live

- [ ] All files uploaded to GitHub
- [ ] GitHub Pages enabled
- [ ] Custom domain added in GitHub Pages settings
- [ ] DNS records updated at domain registrar
- [ ] Contact form ID updated in contact.html
- [ ] Test site at GitHub URL first
- [ ] Verify all links work
- [ ] Check mobile responsiveness

---

## 🚀 Alternative: Netlify (Even Easier!)

1. Go to https://app.netlify.com
2. Sign up/login
3. Drag and drop your portfolio folder
4. Add custom domain: `praditabadal.com.np`
5. Update DNS as shown in Netlify dashboard
6. Done! ⚡

---

**Your portfolio is ready to go live! 🎉**
