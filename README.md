# Jennie Ryu — Product Manager Portfolio

This is a static portfolio site (HTML/CSS/JS). It has no build step and is served as-is by GitHub Pages.

## Structure

```
index.html              Home
about/index.html        About me
ecommerce/index.html    E-commerce case studies
resume/index.html       Experience & education
contact/index.html      Contact
404.html                Not-found page
assets/css/style.css    All styles (colors and fonts are CSS variables at the top)
assets/js/main.js       Mobile menu, scroll reveal, marquee navigation
assets/img/             Profile photo & case study images
Youngjoo_Ryu_Resume.pdf Downloadable resume
og-image.png            Link preview image (1200×630)
```

## Editing

- **Text:** edit the HTML file for that page directly.
- **Nav menu:** the same `<nav>` is copied into all 5 pages, so change it in every one.
- **Colors and fonts:** edit `:root` at the top of `assets/css/style.css`.
- **Resume:** replace `Youngjoo_Ryu_Resume.pdf` with a new file of the same name.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000 in a browser.

## Deploy (GitHub Pages)

1. Push to the `main` branch of a repository named `jennieryu.github.io`.
2. In the repository, go to **Settings → Pages → Build and deployment** and choose **Deploy from a branch**, then `main` / `/ (root)`.
3. The site will be live at https://jennieryu.github.io/ within a minute or two.

> If you use a different repository name (for example, `portfolio`), the site is served at `https://jennieryu.github.io/portfolio/`.
> Every page uses relative paths, so it still works, but you need to update the `og:image` and `canonical` URLs in each page's `<head>`,
> and the `/` paths in `404.html`.
