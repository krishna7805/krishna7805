# Third-party assets embedded in the SVGs

## Fonts (base64 WOFF2, Basic Latin subsets, embedded in every SVG)
- **Unbounded** 800, (c) 2022 The Unbounded Project Authors, https://github.com/googlefonts/unbounded. SIL Open Font License 1.1: `Unbounded-OFL-1.1.txt`
- **JetBrains Mono** 500 and 700, (c) 2020 The JetBrains Mono Project Authors, https://github.com/JetBrains/JetBrainsMono. SIL Open Font License 1.1: `JetBrainsMono-OFL-1.1.txt`
- Source files: the `@fontsource/unbounded` and `@fontsource/jetbrains-mono` npm packages (latin subset), further reduced to Basic Latin plus a few punctuation marks with fontTools `pyftsubset`. No outlines were edited.

## Brand marks (inline SVG paths)
Simple Icons data is CC0 1.0 (`SimpleIcons-CC0-1.0.md`). The marks remain trademarks of their owners (`SimpleIcons-DISCLAIMER.md`); they are used here only to label the technologies and profiles they identify.

| Mark | Source | Brand hex |
| --- | --- | --- |
| Java | simple-icons@6.0.0 (java.svg, removed from current releases) | #007396 |
| Spring | simple-icons@16.34.0 (spring) | #6DB33F |
| Hibernate | simple-icons@16.34.0 (hibernate) | #59666C |
| Python | simple-icons@16.34.0 (python) | #3776AB |
| JavaScript | simple-icons@16.34.0 (javascript) | #F7DF1E |
| React | simple-icons@16.34.0 (react) | #61DAFB |
| Node.js | simple-icons@16.34.0 (nodedotjs) | #5FA04E |
| Express | simple-icons@16.34.0 (express) | #0A0A0A |
| MySQL | simple-icons@16.34.0 (mysql) | #4479A1 |
| PostgreSQL | simple-icons@16.34.0 (postgresql) | #4169E1 |
| Firebase | simple-icons@16.34.0 (firebase) | #DD2C00 |
| Supabase | simple-icons@16.34.0 (supabase) | #3FCF8E |
| Git | simple-icons@16.34.0 (git) | #F03C2E |
| GitHub | simple-icons@16.34.0 (github) | #181717 |
| Instagram | simple-icons@16.34.0 (instagram) | #FF0069 |
| LinkedIn | simple-icons@6.0.0 (linkedin.svg, removed from current releases) | #0A66C2 |

- **Java** and **LinkedIn** are no longer shipped in current Simple Icons releases, so those two paths come from the last releases that carried them (v6.0.0, npm package `simple-icons`, `icons/java.svg` and `icons/linkedin.svg`).
- Rendering tweaks for contrast on the navy background: near-black marks (Express, GitHub) are drawn in off-white, and dim marks (Java, Hibernate, Python, MySQL, PostgreSQL) are lightened by 32%. Shapes are unchanged.
- The generic SQL database glyph, location pin, arrows, capability icons and slide artwork are original, simple vector shapes (no brand marks).
- Portraits are embedded from the supplied `id.png` and `right_pointing.png`, resized (Lanczos, alpha preserved) and losslessly recompressed; nothing was redrawn or masked.
