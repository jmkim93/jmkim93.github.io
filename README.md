# Jungmin Kim personal website

Plain HTML, CSS, and a small theme-toggle script. No Hugo, installation, or build commands.

## Create a fresh GitHub Pages repository

1. Sign in as `jmkim93`. To use https://jmkim93.github.io/, the repository must be named `jmkim93.github.io`.
2. If that repository already exists, keep a backup and rename it to an available name such as `jmkim93-hugo-backup` under Settings > General. Disable its old Hugo deployment workflow and unpublish its Pages site. Do not delete the old repository. This migration may temporarily interrupt the current website.
3. Use GitHub's + menu > New repository. Select your account, name the repository `jmkim93.github.io`, choose Public, enable Add README, and click Create repository.
4. Unzip this package. On the new repository's Code tab, choose Add file > Upload files. Drag in the entire `docs` folder, then Commit changes. Upload the extracted folder, not the ZIP. The root of your repository should contain `docs/index.html` and `docs/publications.html`.
5. Make sure `docs/.nojekyll` exists. Hidden files may not appear in your file picker. If it is missing, use Add file > Create new file, enter `docs/.nojekyll`, and commit the empty file.
6. Open Settings > Pages. Under Build and deployment, set Source to Deploy from a branch, select `main` and `/docs`, then Save. No custom workflow is needed. Keep GitHub Actions enabled for the Pages deployment.
7. Allow up to 10 minutes, then visit https://jmkim93.github.io/. Check Publications, CV, and a paper PDF. Review the Pages deployment in Actions if necessary.

If you prefer to test without renaming the existing repository first, create a differently named public repository, for example `personal-site`, and use the same steps. Its URL will be https://jmkim93.github.io/personal-site/. The package uses relative internal links so it works there too.

Official instructions:
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Package contents

- `docs/index.html`: homepage
- `docs/publications.html`: full publication list, including six conference entries
- `docs/research/`: individual summaries for the eight original research articles
- `docs/cv.pdf`: CV
- `docs/papers/`: 11 existing paper/dissertation PDFs
- `docs/about/`, `docs/pubs/`, `docs/publist/`: redirects for the old URLs
- `docs/.nojekyll`: bypasses Jekyll processing

The newly added CLEO 2026 entry links to its DOI. No local PDF was supplied for that entry.
Other old Hugo pages, posts, tags, archives, and miscellaneous pages are not included. Keep the old repository to migrate them later if desired.

## Editing and appearance

Open `docs/index.html` in a browser. Edit text and embedded styling in the two HTML files. Each page includes its own CSS. Apply site-wide style changes to the homepage, publication list, and pages in `docs/research`. Original research article titles in the full list are currently unlinked; the separate summary pages remain available in `docs/research`. Review, conference, and dissertation titles retain their original external links.

The design uses neutral warm-gray accents with restrained serif headings. The sun/moon icon switches between light and dark modes. The site initially follows the system preference and remembers a chosen theme across pages when hosted. Local file previews may store preferences separately for each file.

For future updates, edit files in `docs`, commit, and push. GitHub Pages republishes automatically.

