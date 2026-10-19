# Yuzhang Xie — personal homepage

A small, responsive, static homepage based on the downloaded academic homepage template. The original sample profile, papers, projects, experience, awards, social links, and template branding have been removed so that no fictional biography is presented as real.

## Preview locally

From this folder, run:

```bash
python3 -m http.server 8080 --bind 127.0.0.1
```

Then open <http://127.0.0.1:8080> in a browser. Stop the server with `Ctrl+C`.

## Personal details to add

The only personal detail currently confirmed in the files is the name “Yuzhang Xie.” Send the details below (skip anything you do not want public), and the homepage can be filled in accurately:

- Preferred name and, if wanted, Chinese name
- Current role, institution, department, and advisor (if applicable)
- Short introduction and research interests
- Email address and public links (CV, Google Scholar, GitHub, LinkedIn, etc.)
- Publications: title, coauthors, venue/year, and links
- Projects, news, experience, service, or awards to show
- A profile photo, if you want one

The content lives in `index.html`; visual styles live in `stylesheet.css`. Put a CV PDF or profile image in this folder (or a subfolder) and link to it with a relative path, for example `files/cv.pdf`.

## Publish with GitHub Pages

1. Sign in to GitHub and create a **new repository under your own account**. For a personal site at `https://YOUR-USERNAME.github.io`, name the repository `YOUR-USERNAME.github.io`. A regular repository also works and gets a URL like `https://YOUR-USERNAME.github.io/REPOSITORY/`.
2. Upload the contents of this folder to that repository. Ensure `index.html` is at the repository root (not inside an extra nested folder). You can use GitHub's web upload, GitHub Desktop, or Git. For Git, point this existing checkout at the repository you created, then push:

   ```bash
   git remote set-url origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
   git add index.html stylesheet.css images README.md
   git commit -m "Add personal homepage"
   git push -u origin main
   ```

   This downloaded folder already has an `origin` remote configured. Check it with `git remote -v` and replace it with the URL of the repository you created under your own account before pushing. The command above assumes your local branch is called `main`; check with `git branch --show-current` if needed.
3. In the GitHub repository, open **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, choose `main` and `/(root)`, then click **Save**.
4. Wait for the Pages deployment to finish. The public URL appears on the Pages settings screen. It can take a few minutes after the first publish or after later changes.

The site is static HTML and CSS, so it does not need a server, build step, or paid hosting. Anyone with the URL can view a public GitHub Pages site. Avoid publishing private contact details or documents.
