# Screenshot Workflow

Screenshots are required evidence when documenting editable storefront areas. Use real screenshots when available and never fabricate image references.

## Discovery

Inspect the repo for:

- `docs/img/`
- other docs asset folders
- existing markdown image references
- screenshots attached by the user

Record what exists before drafting the final image placement.

## Naming and placement

- Keep screenshots in the documentation image directory used by the repo, typically `docs/img/`.
- Use descriptive filenames tied to the UI or action shown.
- Insert the image directly after the paragraph or step it supports.
- Use standard markdown image syntax with a relative path.

Examples:

- `page-builder.png`
- `featured-inst.png`
- `discard-publish.png`

## Required-real-screenshot policy

- Use an image reference only when a real file exists.
- If a screenshot is missing, do not add a fake filename just to complete the page.
- Continue drafting the page text even when screenshots are missing.

## Missing-shot checklist

When assets are incomplete, produce a screenshot manifest with one line per required image:

- page or feature name
- screenshot purpose
- expected file path
- status: `available` or `missing`
- short capture note for missing shots

Example format:

| Page | Purpose | Path | Status | Capture note |
| --- | --- | --- | --- | --- |
| Home | Featured products settings | `docs/img/featured-inst.png` | available | Existing asset |
| General | Publish controls in Page Builder | `docs/img/discard-publish.png` | missing | Capture Save, Preview, and Publish controls |

## Partial-asset behavior

If some screenshots exist and others do not:

- place the real screenshots normally
- leave the related text intact for missing images
- append the missing-shot checklist so the next pass can complete the docs

## Quality bar

- Prefer screenshots that clearly show the control or panel being referenced.
- Avoid decorative screenshots that do not support a step.
- If a screenshot is outdated or clearly mismatched, mark it for recapture instead of treating it as complete.
