# Documentation Template

Welcome to the project documentation template! This template is designed to help you effectively document your projects using MkDocs, a static site generator that’s geared towards project documentation.

## Using the Documentation Skill

This repository includes a repo-local skill at `skills/ct-ecommerce-docs/` for generating and updating Coalition-style ecommerce documentation.

Invoke it by mentioning `$ct-ecommerce-docs` in your prompt, for example:

`Use $ct-ecommerce-docs to generate the full documentation set for this project, including page map, markdown drafts, screenshot manifest, and assumptions.`

Common uses:

- Generate the full documentation set for a BigCommerce project
- Update specific pages such as Home, Category, or Product
- Audit existing docs and identify missing screenshots
- Preserve the current MkDocs structure while refreshing the content

## Getting Started

1. Installation: Ensure you have MkDocs installed, following this <a href="https://www.mkdocs.org/user-guide/installation/" target="_blank">guide</a>. You can install it via pip:
   `pip install mkdocs`

2. On this repository, click on 'Use this template', then 'Create a new repository'.

3. Clone the new repo into your computer and open the root folder in your IDE.

4. Use the following command to run the MkDocs development server:
   `mkdocs serve --livereload`

5. Once the changes are ready, you can deploy using the command:
   `mkdocs gh-deploy`

6. To visit the page available online, go to your GitHub repository, then go to Settings->Pages and you should see the link. If it's not working, make sure your repository is set as public and that the branch selected for the live page is gh-pages.
