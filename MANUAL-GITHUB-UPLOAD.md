# Manual GitHub upload — BESTSOL

## 1. Back up first
Download or otherwise preserve the current repository before replacing files. Keep any existing genuine photographs, CNAME file, domain-verification files and GitHub configuration. This export does NOT include a CNAME file and does not configure DNS or HTTPS. Do not delete existing settings or files indiscriminately.

## 2. Check locally
Extract the ZIP. Open index.html from the extracted folder and check all six pages. Do not upload the ZIP as the website. There is no build/install command and no framework dependency.

## 3. Upload to the repository root
In smgrtone/bestsol-site on the intended publishing branch, use Add file → Upload files. Upload the extracted CONTENTS, not an extra enclosing BESTSOL-ready-to-upload folder. Keep the assets/, supad/, tarak/, ghg-measurement/, team/ and contact/ folder structure. The homepage index.html must be at the publishing root. Ensure .nojekyll is included (it may be hidden by your file manager); retain the existing .nojekyll if already present.

The replacement set is:
- index.html
- assets/styles.css
- assets/main.js
- assets/img/header-icon-placeholder.svg, assets/img/logo-fallback.svg and all placeholder-*.svg files
- supad/index.html
- tarak/index.html
- ghg-measurement/index.html
- team/index.html
- contact/index.html

The README/review/validation/manifest/image guide files are supporting documents; they are not linked as site navigation pages. You can include them in the repository. Do not upload the separate preview HTML as index.html.

Review the staged files, enter a commit message, then commit. Browser upload replaces matching files but does not remove unrelated old routes. No deletion is required for the previously described five-page baseline. If your actual repository contains an obsolete duplicate measurement page or an old rice page, inspect and remove that separately only after confirming it is unwanted; do not infer that this upload deletes it.

## 4. Check GitHub Pages publishing
If publishing directly from a branch, Settings → Pages → Build and deployment → Deploy from a branch should point to your intended branch (main for this project) and /(root). Preserve a working Actions-based workflow if that is what your repository actually uses instead of changing it blindly. Check the deployment result and the site URL shown by GitHub Pages. Repository pages and the rendered Pages website are different URLs.

GitHub documentation:
https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 5. Add your photographs
Follow IMAGE-UPLOAD-GUIDE.md. Upload actual photographs to assets/img with the prescribed names. Existing images are not overwritten by any JPG or PNG in this package; it contains only SVG fallback artwork. Commit image uploads on the publishing branch and refresh the rendered site after deployment. Check image descriptions and content against the actual photographs.

## 6. Live checks
Visit Home, Carbon Project, Technology, Measure GHG, Team and Contact. Test mobile Menu, keyboard navigation, email links, publication link, real-image replacement and missing-image fallback. Confirm bestsol.org resolves to the rendered site and HTTPS works; this package alone does not map the domain. Review the supplied CONTENT-REVIEW.md before treating inherited claims as publication-approved.

## Header icon
Upload assets/img/header-icon.png (500 × 500 px square PNG). It replaces the neutral circle on all six pages. logo.png is separate and reserved. This ZIP is the complete site, not a patch; upload its extracted contents to the repository root.
