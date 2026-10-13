# My books

A starter for a book collection published with [BookMD](https://github.com/atom-forge/bookmd) on GitHub Pages.

## Get your own copy

1. Click **Use this template → Create a new repository**. Make it **public** (GitHub Pages is not available for private repositories on the free plan).
2. In your new repository open **Settings → Pages → Build and deployment** and set **Source** to **GitHub Actions**.
3. Edit the Markdown files in `content/` (right in the GitHub web editor, if you like) and commit to `main`.
4. Open the **Actions** tab. When the *Deploy book* run is green, your site is at `https://<your-name>.github.io/<repository>/`.

Every later commit to `main` republishes the site. If a link is broken, the run fails and the live site stays as it was.

## What is where

- `content/books.md` – the front page and the list of books.
- `content/my-first-book/` – a sample book: `book.md` is its front page, the other files are pages.
- `portal.config.ts` – site title and entry file.
- `.github/workflows/pages.yml` – builds and deploys the site.

How to write books (metadata, chapters, tags): [authoring guide](https://github.com/atom-forge/bookmd/blob/main/docs/authoring.md). Details of publishing: [deploy guide](https://github.com/atom-forge/bookmd/blob/main/docs/user/deploy-a-book.md).

If the repository is named `<your-name>.github.io` or uses a custom domain, remove the `env: BASE_PATH` lines from the workflow.
