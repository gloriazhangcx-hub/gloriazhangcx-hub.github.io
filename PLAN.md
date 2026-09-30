# Portfolio Site Plan

## Goal

Create a publish-ready personal portfolio as a static Jekyll site for
`gloriazhangcx-hub.github.io`, with all website files at the project root so
GitHub Pages can publish from the `main` branch and `/` (root).

## Pages and design

- Home, About, Work Experience, and Contact pages, with shared navigation and
  footer.
- Responsive, single-column layout with a light theme, purple accents, and a
  vintage-inspired typographic style.
- Semantic HTML, accessible color contrast, SEO metadata, sitemap, and favicon.
- Reusable Jekyll layouts and includes; Markdown page content with YAML front
  matter; plain HTML and CSS with no unnecessary dependencies.

## Content and assumptions

- No résumé, biography, experience details, or email address were provided.
  Use clearly labeled placeholders for personal and career content; do not
  invent employers, achievements, projects, or metrics.
- Do not include a public email or `mailto` link.
- The only supplied visual reference is a preference for purple; there are no
  reference website URLs.

## Delivery and verification

- Keep `_config.yml`, `index.md`, `_layouts`, `_includes`, assets, and all other
  site files directly in the project root.
- Include a README with instructions for editing content, previewing locally,
  and running Lighthouse.
- Check the Jekyll/GitHub Pages configuration and navigation, and inspect the
  responsive layout at 375px and 1280px widths. Aim for Lighthouse scores of at
  least 90 in Performance, Accessibility, Best Practices, and SEO.