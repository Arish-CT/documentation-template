# Brand and Assets

Use this workflow to derive documentation styling and project branding.

## Inspect local sources first

Before asking the user for brand inputs, inspect:

- CSS variables in docs or theme stylesheets
- theme config files
- logo files
- favicon files
- existing screenshots
- current documentation colors or visual callouts

The goal is to inherit the project's real styling instead of guessing.

## Minimum brand inputs

Try to establish:

- primary brand color
- supporting accent or dark color if the project uses one
- logo or favicon asset
- any existing docs styling pattern already applied in the repo

If only one reliable color exists, use it and state that supporting colors are assumed from the existing theme or default docs styling.

## When to ask the user

Ask only when local files do not provide enough information to confidently style the docs. Typical blockers:

- no CSS or theme overrides available
- no identifiable brand assets
- conflicting colors across local files
- a request for branded documentation beyond what the repo supports

## Applying the brand

- Preserve existing docs styling if the repo already has it.
- Use detected colors for metadata, guidance, and any generated UI-facing skill metadata.
- Do not invent a new visual system when the project already defines one.
- If the repo has no styling, document the missing brand inputs as assumptions.

## Current template baseline

This template exposes brand colors in `docs/style.css`:

- primary: `#007EA8`
- primary-dark: `#00527C`
- secondary: `#7bc2ea`
- dark neutral: `#313131`
- light neutral: `#ececec`

Treat these as template defaults only. For other projects, prefer their local CSS over this baseline.
