---
name: ct-ecommerce-docs
description: Use when generating or updating Coalition Technologies ecommerce documentation, especially MkDocs-style client handoff docs for BigCommerce storefronts that need page-by-page markdown, admin editing steps, screenshot requirements, image placement, custom widget coverage, and brand-aware styling.
---

# CT Ecommerce Docs

## Overview

Use this skill to create or update Coalition-style ecommerce documentation from a project repository. It is optimized for BigCommerce storefront handoff docs built in MkDocs, but it can adapt to similar Coalition ecommerce projects by inspecting the repo first and then drafting only the pages and instructions supported by the codebase and assets.

Default deliverables:

- recommended page map
- per-page markdown drafts or update plan
- screenshot manifest with available and missing assets
- brand/style inputs used
- assumptions for missing project details

## Workflow

### 1. Inspect the project before drafting

Start by reading the project files that already define the documentation shape:

- docs config such as `mkdocs.yml`
- existing markdown files under `docs/`
- custom CSS, theme variables, or brand assets
- existing screenshots or image folders
- any README or project notes that explain deployment or editing flows

If the project uses MkDocs, note the local preview command and use it when you need to verify the rendered docs. In this template, the expected command is mkdocs serve --livereload.

If the repo already has documentation, preserve its information architecture and naming unless the user asks for a restructure.

For the documentation pattern and tone to mimic, read [references/template-patterns.md](references/template-patterns.md).

### 2. Infer the documentation set

Build the initial page list from the repo evidence, not from a rigid template. Use the Coalition default matrix only as a starting point. Read [references/page-specs.md](references/page-specs.md) to decide which pages to keep, omit, merge, or add.

When enough repo evidence exists, proceed directly. When critical inputs are missing, state the assumptions explicitly in the output.

### 3. Derive brand and styling

Look for brand inputs in local files first:

- CSS custom properties
- theme overrides
- logos or favicons
- existing screenshot framing or image styling

If those files do not provide a usable palette or brand direction, ask the user for the missing inputs before finalizing the docs. Follow [references/brand-and-assets.md](references/brand-and-assets.md).

### 4. Handle screenshots as evidence, not decoration

Use real screenshots when they exist. Do not invent screenshots or pretend an image exists.

If screenshots are partial or absent:

- keep drafting the text
- produce a concrete missing-shot checklist
- place image references only where real files exist

Follow the rules in [references/screenshot-workflow.md](references/screenshot-workflow.md).

### 5. Draft Coalition-style docs

Write concise, page-by-page documentation that helps a client or internal editor manage the storefront without reading theme code.

Prefer this structure:

- page title
- short explanation of the page or feature
- H2 sections per major editable area or feature
- direct editing path in BigCommerce or Page Builder
- short caveat when custom theme behavior limits the native admin controls
- screenshot immediately after the paragraph it supports

Keep external vendor docs linked inline when they explain a built-in platform feature better than a local rewrite.

### 6. Produce complete outputs

Unless the user narrows the scope, provide:

- the recommended page inventory
- markdown drafts or update targets for each page
- screenshot manifest
- brand inputs and styling assumptions
- open questions only when they block accuracy

## Output Rules

- Mirror the repo's existing navigation labels when they already exist.
- Use one markdown file per top-level documentation page unless the current project clearly uses a different pattern.
- Keep tone direct and operational, not promotional.
- Use relative image paths that match the repo's docs structure.
- Put screenshots in the docs image directory used by the project, typically `docs/img/`.
- When a feature is native to the platform, link to the official vendor documentation rather than over-explaining the platform.
- When a feature is custom, document exactly where it is edited and mention any limits or design-specific behavior.

## Common Invocation

Use `$ct-ecommerce-docs` to generate or update client documentation for this ecommerce project, including page drafts, screenshot requirements, and brand-aware styling guidance.



