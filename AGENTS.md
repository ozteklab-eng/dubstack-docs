# Documentation Project Instructions

Use this file to guide AI assistants and maintain consistent documentation changes.

## About This Project

- This is a DubStack documentation site.
- Pages are MDX files with YAML frontmatter.
- Site configuration lives in `dubstack.json`.
- Static assets live in `images/`, `logo/`, or another configured asset folder.
- Keep authored content in Git; DubStack syncs Git content to the hosted site.

## Writing Standards

- Use active voice and address readers directly.
- Prefer short, specific steps over broad explanation.
- Use sentence case for headings.
- Use inline code for file names, commands, paths, API fields, and config keys.
- Keep examples complete enough to copy and run.

## Component Guidelines

- Use cards for navigation or compact feature summaries.
- Use steps for ordered workflows.
- Use callouts only when information needs to stand apart from normal prose.
- Use tabs when readers must choose between platforms, package managers, or environments.
- Use code groups when showing equivalent examples in multiple languages.

## Safety Rules

- Do not commit API keys, passwords, tokens, magic links, private URLs, or customer secrets.
- Do not hardcode environment-specific values unless the page is explicitly documenting that environment.
- Keep generated or test-only pages out of the production navigation unless they are intentional examples.

## Change Checklist

- Update `dubstack.json` when adding, removing, or moving pages.
- Check links after renaming files or slugs.
- Verify the rendered page before publishing important docs changes.
- Keep page titles, descriptions, and navigation labels consistent.
