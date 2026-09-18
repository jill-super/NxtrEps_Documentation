# Docs site

Searchable MD/MDX mirror of the EPS archive (no owner/repo hard-coded).

## Where content lives

- `src/content/docs/` — all pages.
  - `index.mdx` — landing page
  - `overview.md`, `how-to-use.md`, `glossary.md`
  - `roadmap/`, `digital-motor-position/`, `low-output-ceps/`,
    `mechanical-engineering/`, `one-pagers/`, `trm/`,
    `supporting-material/`, `reference/`
- `src/components/SourceFile.astro` — source-file badge (original filename + size).
- `src/styles/custom.css` — readability tweaks.
- `public/` — static assets (figures extracted from the decks, `.nojekyll`).

## Conventions

- One TRM = one page in `trm/`; loose decks grouped by topic in `one-pagers/`.
- Every page ends with a **Sources** table: exact original filename + size + type.
- Figures are extracted from the original decks into `src/assets/` and embedded
  per page; vector-only diagrams stay in the source deck and are noted as such.
