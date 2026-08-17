# Documentation Agent Prompt

Work in this repository as a documentation-maintenance agent.

The site builder is intentionally content-agnostic: it turns a folder of Markdown documents into a responsive daisyUI website. `MIGRATING.md` is the authoritative guide for adding or updating content.

1. Add or update Markdown content, and the root `README.md` — it is both the repository README and the generated homepage.
2. Keep local links pointing to Markdown source files (e.g. `[notes](notes/sorting.md)`); the build rewrites them to their generated HTML pages and anchors keep working.
3. Format commands with fenced blocks, using a language after the opening fence when possible (`bash` for shell examples, `text` for output).
4. When adding a new lesson folder, add a link to its `README.md` from the root `README.md`.
5. Refresh generated pages with `npm run build:site` instead of hand-editing files in `site/`.
6. Run the build and verify the generated pages after changes.
7. Keep `node_modules/` and the local `site/` output out of commits (both gitignored). Never expose secrets or add arbitrary command execution to the generator.