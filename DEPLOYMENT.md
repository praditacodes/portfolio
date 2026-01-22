# Portfolio Deployment Guide

## Domain: https://praditabadal.com.np/

This guide will help you deploy your portfolio website to your domain.

---

## 🚀 Deployment Options

### Option 1: GitHub Pages (Recommended - Free & Easy)

1. **Create a GitHub Repository**
   - Go to [GitHub](https://github.com) and create a new repository
   - Name it `portfolio` or `praditabadal-portfolio`
   - Make it public (required for free GitHub Pages)

2. **Upload Your Files**
   ```bash
   # Initialize git repository
   git init
   git add .
   git commit -m "Initial portfolio commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository → Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` → `/ (root)`
   - Click Save

4. **Custom Domain Setup**
   - In GitHub Pages settings, add your custom domain: `praditabadal.com.np`
   - Create a file named `CNAME` in your repository root with content:
     ```
     praditabadal.com.np
     ```
   - Update your domain's DNS settings:
     - Add a CNAME record: `@` → `YOUR_USERNAME.github.io`
     - Or add A records pointing to GitHub Pages IPs:
       - 185.199.108.153
       - 185.199.109.153
       - 185.199.110.153
       - 185.199.111.153

---

### Option 2: Netlify (Free & Fast)

1. **Sign up** at [Netlify](https://www.netlify.com)

2. **Deploy**
   - Drag and drop your portfolio folder to Netlify dashboard
   - Or connect your GitHub repository

3. **Custom Domain**
   - Go to Site settings → Domain management
   - Add custom domain: `praditabadal.com.np`
   - Update DNS records as shown in Netlify dashboard

---

### Option 3: Vercel (Free & Modern)

1. **Sign up** at [Vercel](https://vercel.com)

2. **Import Project**
   - Import from GitHub or upload folder

3. **Add Domain**
   - Go to Project Settings → Domains
   - Add `praditabadal.com.np`
   - Update DNS records as instructed

---

### Option 4: Traditional Web Hosting (cPanel/FTP)

1. **Get Hosting**
   - Purchase hosting from a provider (e.g., Hostinger, Bluehost, etc.)
   - Get FTP credentials

2. **Upload Files**
   - Use FTP client (FileZilla, WinSCP) or cPanel File Manager
   - Upload all files to `public_html` or `www` directory
   - Ensure file structure is maintained

3. **DNS Configuration**
   - Point your domain's A record to hosting IP
   - Or use nameservers provided by hosting

---

## 📋 Pre-Deployment Checklist

- [x] Updated `sitemap.xml` with correct domain
- [x] Updated `robots.txt` with correct domain
- [ ] Update Formspree form ID in `contact.html` (if using contact form)
- [ ] Ensure all images are optimized
- [ ] Test all links (GitHub, LinkedIn, projects)
- [ ] Verify resume PDF is accessible
- [ ] Test on mobile devices
- [ ] Check browser compatibility

---

## 🔧 Important Files to Check

1. **contact.html** - Update Formspree form ID (line 19)
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

2. **All HTML files** - Verify all internal links work correctly

3. **assets/images/** - Ensure profile.jpg exists and is optimized

---

## 🌐 DNS Configuration

For your domain `praditabadal.com.np`, you'll need to configure DNS:

### If using GitHub Pages:
- **CNAME Record**: `@` → `YOUR_USERNAME.github.io`
- **OR A Records**: Point to GitHub Pages IPs (see Option 1)

### If using Netlify:
- **CNAME Record**: `@` → `YOUR_SITE.netlify.app`

### If using Traditional Hosting:
- **A Record**: `@` → Your hosting IP address
- **CNAME Record**: `www` → `@` (optional)

---

## ✅ Post-Deployment Steps

1. **Test Your Site**
   - Visit https://praditabadal.com.np
   - Check all pages load correctly
   - Test mobile responsiveness
   - Verify all links work

2. **Submit to Search Engines**
   - Google Search Console: https://search.google.com/search-console
   - Bing Webmaster Tools: https://www.bing.com/webmasters

3. **SSL Certificate**
   - Most hosting providers (GitHub Pages, Netlify, Vercel) provide free SSL
   - Ensure HTTPS is enabled

4. **Performance Check**
   - Test with Google PageSpeed Insights
   - Optimize images if needed

---

## 🆘 Troubleshooting

**Domain not working?**
- Wait 24-48 hours for DNS propagation
- Check DNS records are correct
- Verify domain is properly connected in hosting settings

**404 Errors?**
- Ensure `index.html` is in root directory
- Check file paths are correct (case-sensitive on some servers)

**Images not loading?**
- Verify image paths are relative (e.g., `assets/images/profile.jpg`)
- Check file names match exactly (case-sensitive)

---

## 📞 Need Help?

If you encounter issues:
1. Check hosting provider's documentation
2. Verify DNS settings with your domain registrar
3. Test locally first before deploying

---

**Good luck with your deployment! 🎉**
