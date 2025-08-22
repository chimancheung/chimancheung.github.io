# Academic Website (GitHub Pages, apex domain: chimancheung.com)

This repo is ready to publish as **chimancheung.com** using GitHub Pages (theme: `jekyll-theme-minimal`).

## Quick publish steps

1. **Create the user site repo**
   - On GitHub, create a new repo named **chimancheung.github.io** (must match your username).

2. **Upload the files**
   - Upload all files from this folder (including `CNAME`).

3. **DNS at your registrar**
   - Add A records for `@` (apex) pointing to:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - (Optional) Add AAAA records for `@` (IPv6):
     - 2606:50c0:8000::153
     - 2606:50c0:8001::153
     - 2606:50c0:8002::153
     - 2606:50c0:8003::153
   - Add a CNAME record: `www` → `chimancheung.github.io`

4. **Custom domain in GitHub**
   - In your repo: **Settings → Pages → Custom domain** = `chimancheung.com` (the `CNAME` file here already matches).

5. **Enforce HTTPS**
   - Once DNS has propagated, tick **Enforce HTTPS** in **Settings → Pages**.

6. **Replace placeholders**
   - Swap out PDF placeholders in `papers/` with your actual files, or edit links in `index.md`.
   - Your CV lives at `assets/cv/Chiman_Cheung_CV_v9.pdf` — replace it when you have a new version.

## Local preview (optional)
If you have Ruby/Jekyll:
```bash
gem install bundler jekyll
bundle add jekyll-theme-minimal jekyll-seo-tag jekyll-sitemap
jekyll serve
```
Open http://127.0.0.1:4000

---

**Nav/Links** already assume apex domain and baseurl="".
