# Template Patterns

This file captures the documentation conventions established in this repository's MkDocs template.

## Information architecture

- Use a page-per-topic structure.
- Keep top-level navigation short and operational.
- For local preview in this template, run mkdocs serve --livereload.
- Common page set in this template:
  - `General`
  - `Home`
  - `Category`
  - `Product`
  - `Static`
  - `Mega Menu`
  - `Other`
- Default filenames are simple and lowercase, such as `index.md`, `home.md`, `category.md`, and `product.md`.

## Writing style

- Start each page with a direct explanation of what the page or feature is.
- Use short paragraphs.
- Use `##` headings for editable sections or feature groups.
- Focus on how a client or merchandiser updates the storefront.
- Prefer concrete admin paths like `Storefront > Themes > Customize`.
- Keep caveats short and practical.
- Do not write marketing copy or deep implementation details unless they affect editing.

## Vendor documentation links

- Link inline to official platform documentation when the feature is native to BigCommerce.
- Use HTML links with `target="_blank"` when matching the existing template style.
- Do not duplicate full vendor guidance if a short explanation plus a link is enough.

## Screenshot usage

- Screenshots support the step immediately above them.
- Use repository-relative paths like `![featured-inst.png](img/featured-inst.png)`.
- Prefer descriptive file names based on the UI element or action shown.
- Keep screenshots in `docs/img/` unless the project uses a different image directory.

## Custom feature language

- For built-in platform components, state that the project uses the native BigCommerce feature and explain where it is managed.
- For custom widgets or theme features, state that they are custom to the project or developed by Coalition Technologies.
- When admin controls may not behave exactly as expected because of the custom theme, mention that explicitly in one sentence.

## Brand and theme conventions from this repo

- Primary accent: `#007EA8`
- Dark primary/nav accent: `#00527C`
- Secondary accent: `#7bc2ea`
- Dark neutral: `#313131`
- Light neutral: `#ececec`

These values come from `docs/style.css` and should be treated as the template baseline, not a universal Coalition palette.



