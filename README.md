# Dayu Xia - Personal Website

This repository hosts my personal website built with the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) Jekyll theme.

## Main Sections

- Home: portrait, academic overview, education, experience, selected projects, and publication
- Projects: selected robotics, embodied AI, and learning-systems work
- Travel: photo-preview cards for travel and photography posts

The homepage is defined in `index.html`; shared fonts are loaded through
`_includes/metadata-hook.html`. Theme-page styling lives in
`assets/css/jekyll-theme-chirpy.scss`, and Travel reuses `_layouts/blogs.html`
with a category filter.

The optimized homepage portrait is `images/dayu-xia.jpg`. It appears beside the
introduction on desktop and above it on smaller screens; replacements should
omit EXIF metadata.

## Local Development

```bash
bundle install
bundle exec jekyll s
```

The site will be available at `dyxia1241.github.io`.

## Deployment

Use `main` for development and deployment. Set GitHub Pages to use GitHub Actions;
pushes to `main` run `.github/workflows/pages-deploy.yml` to build and publish the site.
