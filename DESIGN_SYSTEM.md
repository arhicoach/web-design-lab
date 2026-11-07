# Web Design Lab — Design System v3.0

An interactive, framework-independent design system playground for reviewing foundations, components and page patterns.

## Live site
https://arhicoach.github.io/web-design-lab/

## Architecture
- **Foundations:** typography scale, semantic colors, spacing scale.
- **Atoms:** buttons, inputs, selects, textarea, checkbox.
- **Molecules:** feature cards and accessible modal.
- **Organisms:** navigation and hero.
- **Templates:** sample pricing cards.

## Design tokens
| Token | Default | Purpose |
| --- | --- | --- |
| `--accent` | `#6159e8` | Primary action and highlight |
| `--radius` | `14px` | Component rounding |
| `--density` | `1` | Control spacing multiplier |
| `--base` | `15px` | Base font size |
| `--bg` | `#f6f7fa` | Page background |
| `--surface` | `#fff` | Cards and panels |
| `--text` | `#161b29` | Primary text |
| `--muted` | `#697386` | Secondary text |
| `--border` | `#e5e8f0` | Dividers and strokes |

## Using the playground
1. Choose a category tab.
2. Adjust theme, accent, radius, density or typography in the control panel.
3. Test button states, form controls and modal interaction.
4. Copy CSS tokens to reuse in a new project.

Settings persist in the browser via localStorage when available.

## Current limitations
- A visual prototype, not a production-ready package.
- The form, pricing and navigation demos are non-transactional.
- Visual QA across real browsers/devices and accessibility audit are still needed.
- Tokens are currently embedded in a standalone HTML file for zero-build GitHub Pages deployment.

## Roadmap
- Extract tokens into portable JSON and CSS files.
- Add semantic color contrast diagnostics.
- Add interactive state matrix and responsive previews.
- Add production-oriented components and layout patterns.
- Add framework adapters (Tilda, vanilla HTML/CSS, React).
- Create a versioned review process for the team.
