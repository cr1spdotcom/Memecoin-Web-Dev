# Complete Step-by-Step Guide: Publish Your Website & Get on Google

This guide will walk you through **every single step** to publish your Skeleton Coin website and make it searchable on Google.

---

## PART 1: Publish Your Website (Choose ONE Method)

### 🎯 **METHOD 1: Netlify (EASIEST - Recommended for Beginners)**

#### Step 1.1: Create Netlify Account
1. Open your web browser
2. Go to: **https://www.netlify.com**
3. Click **"Sign up"** (top right)
4. Choose **"Sign up with Email"** or **"Sign up with GitHub"** (GitHub is easier if you have it)
5. Enter your email and create a password
6. Check your email and click the verification link
7. You're now logged into Netlify!

#### Step 1.2: Upload Your Website
1. In Netlify, you'll see a dashboard
2. Look for **"Add new site"** button (usually a big button or in the top right)
3. Click **"Deploy manually"** or **"Drag and drop"**
4. You'll see a box that says **"Want to deploy a new site without connecting to Git? Drag and drop your site output folder here"**
5. **Open File Explorer** on your computer
6. Navigate to: `C:\Users\Guest_Cayanga Family\meme-coin-website`
7. **Select ALL files and folders** in that folder:
   - Click on `index.html`
   - Hold **Ctrl** and click on `assets` folder, `sitemap.xml`, `robots.txt`, `README.md`, `PUBLISHING.md`
   - OR just press **Ctrl+A** to select everything
8. **Drag and drop** all these files into the Netlify upload box
9. Wait for upload (you'll see a progress bar)
10. **Your site is now live!** 🎉

#### Step 1.3: Get Your Website URL
1. After upload, Netlify will show you a URL like: `https://random-name-123456.netlify.app`
2. **Copy this URL** - this is your website address!
3. Click on the URL to see your live website
4. **Save this URL somewhere** - you'll need it for the next steps

#### Step 1.4: (Optional) Change Your Site Name
1. In Netlify, click on your site
2. Go to **"Site settings"** (top menu)
3. Click **"Change site name"**
4. Enter a name like: `skeleton-coin` (must be unique)
5. Your new URL will be: `https://skeleton-coin.netlify.app`

---

### 🎯 **METHOD 2: Vercel (Also Easy)**

#### Step 2.1: Create Vercel Account
1. Go to: **https://vercel.com**
2. Click **"Sign Up"**
3. Choose **"Continue with GitHub"** (recommended) or **"Continue with Email"**
4. Follow the signup process
5. You're logged in!

#### Step 2.2: Deploy Your Website
1. Click **"Add New..."** button
2. Click **"Project"**
3. You'll see options - click **"Browse"** or **"Upload"**
4. Navigate to: `C:\Users\Guest_Cayanga Family\meme-coin-website`
5. **Select the entire folder** or all files
6. Click **"Deploy"**
7. Wait 1-2 minutes
8. **Your site is live!** You'll get a URL like: `https://meme-coin-website.vercel.app`

---

### 🎯 **METHOD 3: GitHub Pages (More Steps, But Free Forever)**

#### Step 3.1: Create GitHub Account
1. Go to: **https://github.com**
2. Click **"Sign up"**
3. Enter username, email, password
4. Verify your email
5. Complete the setup

#### Step 3.2: Create a New Repository
1. After logging in, click the **"+"** icon (top right)
2. Click **"New repository"**
3. Repository name: `skeleton-coin-website` (or any name you like)
4. Make it **Public**
5. **DO NOT** check "Add a README file"
6. Click **"Create repository"**

#### Step 3.3: Install Git (If Not Already Installed)
1. Go to: **https://git-scm.com/download/win**
2. Download Git for Windows
3. Run the installer (just click Next, Next, Next - default settings are fine)
4. Restart your computer if asked

#### Step 3.4: Upload Files Using Git
1. **Open PowerShell** (Press Windows key, type "PowerShell", press Enter)
2. Type these commands **one by one** (press Enter after each):

```powershell
cd "C:\Users\Guest_Cayanga Family\meme-coin-website"
```

```powershell
git init
```

```powershell
git add .
```

```powershell
git commit -m "Initial commit - Skeleton Coin website"
```

```powershell
git branch -M main
```

```powershell
git remote add origin https://github.com/YOUR_USERNAME/skeleton-coin-website.git
```
*(Replace YOUR_USERNAME with your actual GitHub username)*

```powershell
git push -u origin main
```

3. You'll be asked for your GitHub username and password (use a Personal Access Token if password doesn't work)

#### Step 3.5: Enable GitHub Pages
1. Go back to your GitHub repository page
2. Click **"Settings"** (top menu)
3. Scroll down to **"Pages"** (left sidebar)
4. Under **"Source"**, select **"Deploy from a branch"**
5. Branch: **main**
6. Folder: **/ (root)**
7. Click **"Save"**
8. Wait 1-2 minutes
9. Your site will be at: `https://YOUR_USERNAME.github.io/skeleton-coin-website/`

---

## PART 2: Update Your Website with Real URL

**IMPORTANT:** After you get your live URL, you need to update your files.

### Step 2.1: Note Your Real URL
- Write down your website URL (e.g., `https://skeleton-coin.netlify.app` or `https://yoursite.github.io/skeleton-coin-website/`)

### Step 2.2: Update index.html
1. Open: `C:\Users\Guest_Cayanga Family\meme-coin-website\index.html`
2. Press **Ctrl+F** (Find)
3. Search for: `yoursite.com`
4. **Replace ALL instances** with your real URL (e.g., `skeleton-coin.netlify.app`)
5. **Save the file** (Ctrl+S)

**Places to update in index.html:**
- Line with `<link rel="canonical" href="...">`
- Line with `<meta property="og:url" content="...">`
- Line with `<meta property="og:image" content="...">`
- Line with `<meta name="twitter:image" content="...">`
- In the JSON-LD script: `"url": "..."`

### Step 2.3: Update sitemap.xml
1. Open: `C:\Users\Guest_Cayanga Family\meme-coin-website\sitemap.xml`
2. Find: `<loc>https://yoursite.com/</loc>`
3. Replace `yoursite.com` with your real URL
4. **Save the file**

### Step 2.4: Update robots.txt
1. Open: `C:\Users\Guest_Cayanga Family\meme-coin-website\robots.txt`
2. Find: `Sitemap: https://yoursite.com/sitemap.xml`
3. Replace `yoursite.com` with your real URL
4. **Save the file**

### Step 2.5: Re-upload to Your Host
- **Netlify/Vercel:** Drag and drop the updated files again (or use their dashboard to upload)
- **GitHub:** Run these commands in PowerShell:
  ```powershell
  cd "C:\Users\Guest_Cayanga Family\meme-coin-website"
  git add .
  git commit -m "Update URLs"
  git push
  ```

---

## PART 3: Submit to Google Search Console

### Step 3.1: Go to Google Search Console
1. Open your browser
2. Go to: **https://search.google.com/search-console**
3. Sign in with your **Google account** (Gmail account)

### Step 3.2: Add Your Website Property
1. Click **"Add property"** button
2. Choose **"URL prefix"** (not Domain)
3. Enter your **full website URL** (e.g., `https://skeleton-coin.netlify.app`)
4. Click **"Continue"**

### Step 3.3: Verify Ownership - Method 1 (HTML Tag - Easiest)
1. Google will show you a **meta tag** that looks like:
   ```html
   <meta name="google-site-verification" content="abc123xyz..." />
   ```
2. **Copy the entire meta tag**
3. Open: `C:\Users\Guest_Cayanga Family\meme-coin-website\index.html`
4. Find the `<head>` section (near the top)
5. Paste the meta tag **right after** the `<meta charset="UTF-8">` line
6. **Save the file**
7. **Re-upload to your host** (drag & drop to Netlify/Vercel, or `git push` for GitHub)
8. Go back to Google Search Console
9. Click **"Verify"** button
10. You should see: ✅ **"Ownership verified"**

### Step 3.4: Verify Ownership - Method 2 (HTML File - Alternative)
1. In Google Search Console, click **"HTML file"** tab
2. Click **"Download"** - a file will download (e.g., `google1234567890.html`)
3. **Move this file** to: `C:\Users\Guest_Cayanga Family\meme-coin-website\`
4. **Re-upload your entire folder** to your host (including this new HTML file)
5. Go back to Google Search Console
6. Click **"Verify"**
7. You should see: ✅ **"Ownership verified"**

### Step 3.5: Submit Your Sitemap
1. In Google Search Console, look at the left sidebar
2. Click **"Sitemaps"** (under "Indexing")
3. You'll see a box: **"Add a new sitemap"**
4. Enter: `sitemap.xml` (just these words, not the full URL)
5. Click **"Submit"**
6. You should see: ✅ **"Success"** - Google will now crawl your sitemap

### Step 3.6: Request Indexing (Optional but Recommended)
1. In Google Search Console, look at the top search bar
2. It says **"Inspect any URL"** - enter your homepage URL (e.g., `https://skeleton-coin.netlify.app/`)
3. Press Enter
4. Click **"Request indexing"** button
5. Google will add your page to the crawl queue

---

## PART 4: Wait and Monitor

### Step 4.1: How Long Does It Take?
- **Initial indexing:** 1-7 days
- **Appearing in search results:** 1-4 weeks
- **Full indexing:** Can take up to 1-2 months

### Step 4.2: Check Your Progress
1. Go back to Google Search Console
2. Check **"Coverage"** (left sidebar) - see how many pages are indexed
3. Check **"Performance"** - see if people are finding you in search
4. You can also search Google for: `site:yoursite.com` (replace with your URL) to see indexed pages

### Step 4.3: Test Your Site
1. Visit your live website URL
2. Make sure all images load (especially your skeleton warrior image)
3. Test all buttons and links
4. Check on mobile phone too

---

## Quick Checklist

Use this to track your progress:

### Publishing
- [ ] Created hosting account (Netlify/Vercel/GitHub)
- [ ] Uploaded website files
- [ ] Got live website URL
- [ ] Tested website - it works!

### URL Updates
- [ ] Updated `index.html` with real URL (replaced all `yoursite.com`)
- [ ] Updated `sitemap.xml` with real URL
- [ ] Updated `robots.txt` with real URL
- [ ] Re-uploaded files to host

### Google Search Console
- [ ] Created Google Search Console account
- [ ] Added website property
- [ ] Verified ownership (HTML tag or file method)
- [ ] Submitted sitemap.xml
- [ ] Requested indexing for homepage

### Final
- [ ] Website is live and working
- [ ] All images display correctly
- [ ] Waiting for Google to index (check in 1-2 weeks)

---

## Troubleshooting

### Problem: "Site not found" or 404 error
- **Solution:** Make sure your `index.html` is in the root folder, not inside a subfolder

### Problem: Images not showing
- **Solution:** Check that `assets/images/RAAAAH.jpg` exists and the path in HTML is correct

### Problem: Google verification fails
- **Solution:** Make sure you re-uploaded files after adding the verification tag/file

### Problem: Website looks broken
- **Solution:** Check browser console (F12) for errors. Make sure all CSS/JS files uploaded correctly

### Problem: Can't find files to upload
- **Solution:** Make sure you're in: `C:\Users\Guest_Cayanga Family\meme-coin-website`

---

## Need Help?

- **Netlify Support:** https://www.netlify.com/support/
- **Vercel Support:** https://vercel.com/support
- **GitHub Help:** https://docs.github.com/en/pages
- **Google Search Console Help:** https://support.google.com/webmasters

---

**You're all set!** Follow these steps in order, and your website will be live and searchable on Google. 🚀
