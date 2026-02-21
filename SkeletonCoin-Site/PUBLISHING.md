# How to Publish Your Skeleton Coin Website & Get on Google

Follow these steps to put your site online and make it searchable on Google.

---

## Step 1: Publish (Host) Your Website

You need to upload your site to a **host**. These options are **free**:

### Option A: GitHub Pages (free, no signup complexity)

1. Create a **GitHub** account: [github.com](https://github.com)
2. Create a **new repository** (e.g. `skeleton-coin-site`). Leave it empty, no README.
3. On your PC, open **PowerShell** or **Command Prompt** and run:

   ```powershell
   cd "C:\Users\Guest_Cayanga Family\meme-coin-website"
   git init
   git add .
   git commit -m "Skeleton Coin website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/skeleton-coin-site.git
   git push -u origin main
   ```
   Replace `YOUR_USERNAME` with your GitHub username.

4. On GitHub: **Settings → Pages → Source**: choose **main** branch, **/ (root)**. Save.
5. Your site will be at: **`https://YOUR_USERNAME.github.io/skeleton-coin-site/`**

### Option B: Netlify (drag & drop)

1. Go to [netlify.com](https://www.netlify.com) and sign up (free).
2. **Add new site → Deploy manually**.
3. **Drag and drop** your entire `meme-coin-website` folder onto the upload area.
4. Netlify gives you a URL like `https://random-name-123.netlify.app`. You can change it in **Site settings → Domain management**.

### Option C: Vercel

1. Go to [vercel.com](https://vercel.com) and sign up.
2. **Add New → Project**.
3. Import your folder (or connect GitHub if you use it). Deploy.
4. You get a URL like `https://your-project.vercel.app`.

---

## Step 2: Update Your Real URL Everywhere

After you know your **real URL** (e.g. `https://yoursite.netlify.app` or your custom domain):

1. **index.html** – Find and replace `https://yoursite.com` with your real URL:
   - `canonical`, `og:url`, `og:image`, `twitter:image`
   - In the JSON-LD `"url"` block

2. **sitemap.xml** – Replace `https://yoursite.com` with your real URL (in `<loc>` and anywhere else).

3. **robots.txt** – Replace `https://yoursite.com` in the `Sitemap:` line.

Then **re-upload** or **re-deploy** the updated files.

---

## Step 3: Submit to Google (Make It Searchable)

### 3.1 Google Search Console

1. Go to [search.google.com/search-console](https://search.google.com/search-console).
2. Sign in with a Google account.
3. **Add property**:
   - Choose **URL prefix**.
   - Enter your **full site URL** (e.g. `https://yoursite.netlify.app`).
4. **Verify** ownership:
   - **HTML file**: Download the file Google gives you, put it in your `meme-coin-website` folder, redeploy, then click **Verify**.
   - **HTML tag**: Add the `<meta>` tag Google gives you inside the `<head>` of `index.html`, redeploy, then **Verify**.
5. After verification, go to **Sitemaps**.
6. Add: `sitemap.xml` (or `https://yoursite.com/sitemap.xml` with your real URL).
7. Click **Submit**.

### 3.2 Request Indexing (Optional but Helpful)

1. In Search Console, open **URL Inspection**.
2. Enter your homepage URL (e.g. `https://yoursite.com/`).
3. Click **Request indexing**.

Google will crawl your site. It can take a few days to a few weeks to show up in search results.

---

## Step 4: Optional – Custom Domain

- **Netlify / Vercel**: In **Domain settings**, add your own domain (e.g. `skeletoncoin.com`). They’ll show you what to set at your domain registrar (DNS).
- **GitHub Pages**: In repo **Settings → Pages**, set a **Custom domain** and configure DNS as GitHub instructs.

After you switch to a custom domain, **repeat Step 2** and **Step 3** using the new URL.

---

## Quick Checklist

- [ ] Site published (GitHub Pages, Netlify, or Vercel)
- [ ] Replaced `yoursite.com` with your real URL in `index.html`, `sitemap.xml`, `robots.txt`
- [ ] Redeployed after changes
- [ ] Property added and verified in Google Search Console
- [ ] `sitemap.xml` submitted in Search Console
- [ ] URL Inspection → Request indexing for homepage

---

## Why It Gets Searchable

- **Meta tags** (`description`, `keywords`) help Google understand your page.
- **sitemap.xml** tells Google which pages to crawl.
- **robots.txt** allows crawlers and points to the sitemap.
- **Search Console** tells Google your site exists and lets you monitor indexing and search performance.

Your site is now set up to be **published** and **searchable on Google**. Replace `yoursite.com` with your real URL and submit the sitemap for best results.
