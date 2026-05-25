# Petar Raykov – Academic Portfolio

Static site built for [GitHub Pages](https://pages.github.com/), scraped and rebuilt from [petarraykov.com](https://www.petarraykov.com/).

## Structure

```
petarraykov/
├── index.html        ← Home page
├── contact.html      ← Contact page
├── css/
│   └── style.css
├── js/
│   └── main.js
└── README.md
```

## Deploying to GitHub Pages

### Option A – New repository (simplest)

1. Create a new GitHub repo, e.g. `petarraykov.github.io` (use `<username>.github.io` for the root domain).
2. Upload all files in this folder to the repo root.
3. Go to **Settings → Pages → Source** and select `main` branch, `/ (root)`.
4. Your site will be live at `https://<username>.github.io` within a minute.

### Option B – Existing repo subfolder

1. Push these files to a `docs/` folder in any existing repo.
2. In **Settings → Pages → Source**, choose `main` branch, `/docs` folder.
3. Site lives at `https://<username>.github.io/<repo-name>`.

## Custom domain

To use `petarraykov.com`:
1. Add a `CNAME` file in the root with the content: `petarraykov.com`
2. In your DNS provider, add:
   - `A` records pointing to GitHub's IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - OR a `CNAME` record pointing to `<username>.github.io`
3. Enable **Enforce HTTPS** in GitHub Pages settings.

## Contact form

The form on `contact.html` currently shows a static confirmation message. To make it functional, replace the `handleSubmit` function with one of:

- **[Formspree](https://formspree.io/)** – free tier available, just update the `action` URL
- **[Netlify Forms](https://docs.netlify.com/forms/setup/)** – if deploying to Netlify instead
- **EmailJS** – client-side email sending

## Content updates

All content is in plain HTML. Edit `index.html` to update bio, projects, and publications directly.
