# Efraim Talmon (1925–2009) Memorial Website

This repository contains the static website dedicated to the memory of **Efraim Talmon (1925–2009)**: Palyam ship captain, Commander in the Israeli Navy (head of the Gabriel missile project), electronics engineer, scholar, and devoted family man.

The contents were cloned and preserved from the original website (`http://efraimtalmon.com`), modernized and cleaned up for hosting on **GitHub Pages**.

## Key Improvements & Cleanup

- **Zero Website Builder Bloat**: Stripped all proprietary GoDaddy / Starfield Technologies website builder scripts, tracking pixels, ad banners, and convoluted inline font styling.
- **Modern Semantic HTML5**: Structured with `<header>`, `<nav>`, `<main>`, `<section>`, `<figure>`, `<figcaption>`, and `<footer>`.
- **Clean Responsive CSS**: Lightweight (`css/style.css`), mobile-friendly, responsive typography, and dark mode support with zero external CDN dependencies.
- **Local Asset Preservation**: All 27 historical photographs, documents, and scans are downloaded locally under `images/`.
- **Archived Document Recovery**: Recovered the two original linked PDF documents (`Ephraim_Talmon_-_Haaretz_1-1.pdf` and `RU_188_b11_f_TALMON__Ephraim.pdf`) and stored them under `uploads/`.
- **GitHub Pages Ready**: Includes `.nojekyll` to bypass Jekyll processing and serve static HTML directly.

## Site Structure

```text
├── index.html            # Main home page
├── Home_Page.html        # Alias for index.html (compatibility with original links)
├── Career.html           # Efraim's naval career, Palyam, Technion, and Gabriel missile
├── Origins.html          # Family history, parents, youth, and ancestry
├── The_Scholar.html      # Home in Ramat Hasharon, library, languages, and scholarship
├── The_Family.html       # Marriage to Batel, children, grandchildren, and family gatherings
├── css/
│   └── style.css         # Clean, responsive styling
├── images/               # All 27 photographs, clippings, and scans
├── uploads/              # Archived Ha'aretz obituary & Smithsonian/SAO research PDFs
├── robots.txt            # Search engine crawler permissions
└── .nojekyll             # Tells GitHub Pages to serve static files as-is
```

## How to Publish to GitHub Pages

1. **Initialize Git & Push to GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit of clean memorial website for GitHub Pages"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**:
   - Go to your repository on GitHub: **Settings** &rarr; **Pages**.
   - Under **Build and deployment** &rarr; **Source**, select **Deploy from a branch**.
   - Under **Branch**, select `main` and folder `/ (root)`. Click **Save**.
   - Your site will be published at `https://<your-username>.github.io/<repo-name>/`.

3. **(Optional) Custom Domain**:
   - If pointing `efraimtalmon.com` to GitHub Pages, add `efraimtalmon.com` in **Settings** &rarr; **Pages** &rarr; **Custom domain** (or create a `CNAME` file containing `efraimtalmon.com`), and configure DNS records at your domain registrar to point to GitHub Pages IPs.
