# Yuzhang Xie — personal homepage

A static academic homepage. `index.html` contains the profile and page sections; `stylesheet.css` contains the template styling. Public academic details and selected work are linked from the page.

## Preview locally

From this folder, run:

```bash
python3 -m http.server 8080 --bind 127.0.0.1
```

Then open <http://127.0.0.1:8080> in a browser. Stop the server with `Ctrl+C`.

To revise profile text, publication entries, projects, or links, edit `index.html`. To add a CV, place the PDF in this folder (or a subfolder) and add its relative path in the contact links.

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
