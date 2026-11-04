# SquareDojo Blog

The SquareDojo Blog is a Jekyll site powered by the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) theme. It is published at [blog.squaredojo.com](https://blog.squaredojo.com).

## Writing a post

Add Markdown files to `_posts/` using Jekyll's date-based filename format:

```text
_posts/YYYY-MM-DD-your-post-title.md
```

Each post needs front matter. Categories use Chirpy's native category system; use the lowercase slugs below so category URLs remain consistent.

```yaml
---
title: Your post title
date: 2026-11-04 09:00:00 +1100
categories: [general]
tags: [indie-development]
---
```

Available categories are:

- `columnly` → `/categories/columnly/`
- `textarcher` → `/categories/textarcher/`
- `logmypoop` → `/categories/logmypoop/`
- `byostream` → `/categories/byostream/`
- `general` → `/categories/general/`
- `learning` → `/categories/learning/`
- `ventout` → `/categories/ventout/`

Chirpy automatically creates category pages when a post uses a category. It supports featured images, a table of contents, syntax highlighting, Mermaid, maths, embedded videos, captions, and responsive images; see the [Chirpy documentation](https://github.com/cotes2020/jekyll-theme-chirpy/wiki) for their front-matter and Markdown syntax.

## Local development

Install a current Ruby and Bundler, then run:

```shell
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000` to preview the site. Build the production site with `bundle exec jekyll build`.

## GitHub Pages and custom domain

The included `.github/workflows/pages-deploy.yml` is Chirpy's GitHub Pages deployment workflow. In GitHub, open **Settings → Pages**, set **Source** to **GitHub Actions**, and let the workflow deploy pushes to the repository's default branch (`main`).

Then add `blog.squaredojo.com` as the custom domain in the same Pages settings. The committed `CNAME` file supplies this domain during deployment.

At the DNS provider for `squaredojo.com`, create a `CNAME` record for `blog` pointing to `Deepindera.github.io` (or the GitHub Pages hostname shown by GitHub for this repository). Do not add DNS records until the domain is configured in GitHub Pages, and enable HTTPS once GitHub makes it available.

## Licence

This project retains the [MIT licence](LICENSE) from the official Chirpy starter. Chirpy itself is also MIT licensed.
