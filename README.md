# Gloria Zhang — Portfolio

A static Jekyll portfolio prepared for GitHub Pages at
[gloriazhangcx-hub.github.io](https://gloriazhangcx-hub.github.io). The site is
configured to publish from the `main` branch and the repository root.

## Update the site

- Edit `index.md` to update the single-page introduction, About, Work Experience,
  and Contact sections. Personal and career details are currently marked as
  placeholders.
- Change the shared design in `assets/css/site.css`.
- The cat illustration is in `assets/images/lavender-cat.svg`.
- Update the site title, description, URL, and plugin settings in `_config.yml`.
- Keep `_config.yml`, `index.md`, `_layouts`, `_includes`, and `assets` in the
  repository root for GitHub Pages publishing.

## Preview locally

Install Ruby and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll. To generate the static output without
starting the server, run `bundle exec jekyll build`; the generated site is in
`_site/`.

## Run Lighthouse

1. Preview the site locally or publish it through GitHub Pages.
2. Open the home page in Chrome.
3. Open Developer Tools → **Lighthouse**, select Performance, Accessibility,
   Best Practices, and SEO, then run an audit for mobile and desktop.

The source is intentionally small: Markdown page content, reusable Jekyll
layouts/includes, and plain HTML/CSS. It has no backend, tracking scripts, or
contact form.