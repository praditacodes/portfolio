# Deploy Portfolio to praditabadal.com.np

Since you already own the domain **praditabadal.com.np**, you need to deploy your portfolio files to your web hosting server.

---

## 🎯 Step-by-Step Deployment Guide

### Step 1: Access Your Web Hosting

You need to access your hosting account. This could be:
- **cPanel** (most common)
- **FTP Access**
- **File Manager** in your hosting dashboard

**Where to find it:**
- Check your hosting provider's email/account dashboard
- Common providers: Hostinger, Bluehost, Namecheap, GoDaddy, etc.
- Login to your hosting account

---

### Step 2: Upload Files via cPanel (Easiest Method)

1. **Login to cPanel**
   - Go to your hosting provider's website
   - Login to your account
   - Find "cPanel" or "File Manager"

2. **Navigate to Public Directory**
   - Open **File Manager**
   - Go to `public_html` folder (this is your website root)
   - **OR** `www` folder (some hosts use this)
   - **OR** `htdocs` folder

3. **Upload Your Files**
   - Delete any default files (like `index.html` or `index.php` if they exist)
   - Click **Upload** button
   - Select ALL files from your portfolio folder:
     - `index.html`
     - `about.html`
     - `projects.html`
     - `contact.html`
     - `sitemap.xml`
     - `robots.txt`
     - `CNAME` (optional, only if using GitHub Pages)
     - `assets/` folder (upload entire folder)
   - Wait for upload to complete

4. **Verify File Structure**
   Your `public_html` should look like this:
   ```
   public_html/
   ├── index.html
   ├── about.html
   ├── projects.html
   ├── contact.html
   ├── sitemap.xml
   ├── robots.txt
   └── assets/
       ├── css/
       │   └── style.css
       ├── js/
       │   └── script.js
       └── images/
           └── profile.jpg
   ```

---

### Step 3: Upload Files via FTP (Alternative Method)

**If you prefer FTP:**

1. **Get FTP Credentials**
   - From your hosting provider
   - Usually: FTP Host, Username, Password, Port (usually 21)

2. **Use FTP Client**
   - Download **FileZilla** (free): https://filezilla-project.org
   - Or use **WinSCP** (Windows): https://winscp.net

3. **Connect**
   - Enter FTP details
   - Connect to server

4. **Upload Files**
   - Navigate to `public_html` or `www` folder
   - Drag and drop all your portfolio files
   - Ensure folder structure is maintained

---

### Step 4: Set Permissions (If Needed)

In cPanel File Manager:
- Right-click `index.html` → **Change Permissions**
- Set to `644` (readable by web server)
- Do the same for all HTML files
- Folders should be `755`

---

### Step 5: Verify Domain Configuration

1. **Check DNS Settings**
   - Your domain should point to your hosting server
   - A Record: `@` → Your hosting IP address
   - CNAME: `www` → `@` (optional)

2. **Check Domain in Hosting**
   - In cPanel, go to **Addon Domains** or **Domains**
   - Ensure `praditabadal.com.np` is added
   - Document root should be `public_html` or `public_html/praditabadal.com.np`

---

### Step 6: Test Your Website

1. **Wait 5-10 minutes** for files to propagate
2. Visit: **https://praditabadal.com.np/**
3. Check all pages:
   - https://praditabadal.com.np/
   - https://praditabadal.com.np/about.html
   - https://praditabadal.com.np/projects.html
   - https://praditabadal.com.np/contact.html

---

## 🔧 Common Issues & Solutions

### Issue 1: "Index of /" or Directory Listing
**Solution:** Ensure `index.html` is in the root directory (`public_html`)

### Issue 2: 404 Errors
**Solution:** 
- Check file names match exactly (case-sensitive on Linux servers)
- Verify files are in `public_html` not a subfolder
- Check `.htaccess` file if exists

### Issue 3: CSS/JS Not Loading
**Solution:**
- Verify `assets/` folder uploaded correctly
- Check file paths in HTML (should be `assets/css/style.css`)
- Clear browser cache (Ctrl+F5)

### Issue 4: Images Not Showing
**Solution:**
- Verify `assets/images/profile.jpg` exists
- Check file permissions (should be 644)
- Ensure image file name matches exactly

### Issue 5: Domain Not Loading
**Solution:**
- Check DNS propagation: https://www.whatsmydns.net
- Verify domain is added in hosting account
- Contact hosting support if needed

---

## 📋 Pre-Upload Checklist

Before uploading, ensure:

- [ ] All files are ready in your portfolio folder
- [ ] `index.html` exists (this is your homepage)
- [ ] `assets/` folder contains all CSS, JS, and images
- [ ] `profile.jpg` exists in `assets/images/`
- [ ] Contact form ID updated (if using Formspree)
- [ ] All links tested locally

---

## 🚀 Quick Upload Checklist

After uploading:

- [ ] All HTML files uploaded to `public_html`
- [ ] `assets/` folder uploaded with all subfolders
- [ ] `sitemap.xml` and `robots.txt` uploaded
- [ ] `index.html` is in root directory
- [ ] File permissions set correctly (644 for files, 755 for folders)
- [ ] Test website in browser
- [ ] Check all pages load correctly
- [ ] Verify images display
- [ ] Test mobile responsiveness

---

## 💡 Pro Tips

1. **Backup First**: Download existing files from `public_html` before uploading
2. **Use ZIP**: Some hosts allow uploading ZIP and extracting (faster)
3. **Check File Size**: Ensure images aren't too large (optimize if needed)
4. **SSL Certificate**: Enable HTTPS/SSL in your hosting panel (usually free)
5. **Test Locally**: Test your site locally first before uploading

---

## 📞 Need Help?

**If you're stuck:**

1. **Check Hosting Documentation**: Your hosting provider has guides
2. **Contact Hosting Support**: They can help with upload/DNS issues
3. **Common Hosting Panels:**
   - **cPanel**: Most common, has File Manager
   - **Plesk**: Similar to cPanel
   - **Custom Panel**: Check your provider's docs

---

## ✅ After Deployment

Once live:

1. **Submit to Google**: https://search.google.com/search-console
2. **Test Performance**: https://pagespeed.web.dev
3. **Check Mobile**: Test on phone/tablet
4. **Share Your Site**: Your portfolio is live! 🎉

---

**Your portfolio will be live at: https://praditabadal.com.np/**

Good luck! 🚀
