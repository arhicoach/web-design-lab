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

## Primary implementation target: Flexbe

The first production application of this system is the engineering services website. Flexbe is the **primary** site-building platform; other platforms are secondary and should not drive component architecture.

### Flexbe implementation decision tree
1. **Native configurable block first.** Choose a block whose hierarchy and behavior match the pattern. Map typography, colors, spacing, borders, responsive behavior and states to system tokens.
2. **Flexbe layout composition second.** Use free positioning and nested elements for designs that native blocks cannot reproduce faithfully, while checking mobile breakpoints.
3. **Custom code last.** Use HTML/CSS/JS only where supported and necessary; avoid overriding Flexbe's internal generated selectors when stable custom classes or supported settings exist.

### Required implementation spec for every pattern
- Purpose and conversion role on the engineering website.
- Flexbe block/template selection or a clear custom-layout rationale.
- Content hierarchy, desktop/mobile layout and responsive breakpoints.
- Exact design tokens: font roles, spacing, radius, colors and interactive states.
- Asset dimensions and image-cropping guidance.
- Flexbe editor configuration steps and any supported custom CSS/JS.
- QA checklist at 320, 375, 390, 430, 768, 1024 and 1440 px.

### Quality gates
- No horizontal overflow on mobile.
- Readable text, sufficient contrast, keyboard-focus visibility.
- No unexpected sticky overlays or clipped form controls.
- Validate in Flexbe preview before publishing; changes should remain drafts until approved.

### First real-world use case
Engineering services website: premium but practical visual language, clear service proposition, trust signals, project photos, readable pricing explanations and conversion-focused questionnaire. Build and validate reusable sections on Flexbe, then feed learnings back into the design system.
