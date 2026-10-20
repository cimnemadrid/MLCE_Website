# AGENTS.md — MLCE Research Group Website

## Project overview

This repository contains the public website of the **Machine Learning in Civil Engineering (MLCE)** research group at **CIMNE** (International Centre for Numerical Methods in Engineering).

- **Group name:** Machine Learning in Civil Engineering (MLCE)
- **Subtitle:** Numerical Modelling, Machine Learning & Artificial Intelligence
- **Institution:** CIMNE
- **Website language:** English
- **Hosting:** GitHub Pages
- **Primary audience:** Researchers, engineering professionals, project partners, prospective students and collaborators

## Research identity

The group develops and applies numerical modelling, machine learning and artificial intelligence methods to practical engineering problems. Work may involve physics-based modelling, data-driven models and hybrid approaches, drawing on numerical simulations, experimental data and monitoring data.

The three agreed application areas are:

1. **Dams**
2. **Environmental Engineering**
3. **Industrial Engineering**

Typical methods and technologies include:

- Numerical Modelling (including FEM, CFD, DEM and multiphysics where relevant)
- Machine Learning & Artificial Intelligence
- Hybrid Modelling
- Digital Tools (e.g. predictive tools, decision support and early warning systems)

Do not invent specific achievements, current memberships, positions, publication records, funded projects, dates or institutional endorsements. Treat unverified details as drafts requiring confirmation.

## Site structure

Keep the current simple site and its main navigation:

- Home (`index.html`): group identity, About Us and the three Research Areas.
- Research (`research.html`): Methods & Technologies.
- People (`people.html`): Researchers and PhD Students.
- Projects (`projects.html`): Selected Projects.
- Publications (`publications.html`): Selected Publications and academic profile links.
- Friends & Collaborators (`friends.html`): collaborator profiles.

Contact information may be placed in the footer. Do not create additional pages, menu items or sections without an explicit request. Preserve the six-page static structure and the single shared `styles.css`. Use the same navigation and footer on every page, with relative page links and `aria-current="page"` on the current navigation item. Keep duplicated navigation and footer markup synchronized manually; no build step is required.

## Technical constraints

- Prefer **semantic HTML and plain CSS**.
- Use JavaScript only when it provides a clear functional benefit.
- **Do not introduce** React, Vue, Bootstrap, Tailwind, package managers, build pipelines or external libraries without explicit approval.
- Keep `index.html` at the repository root so GitHub Pages can serve it.
- Use relative links and asset paths compatible with deployment under a GitHub Pages project URL (for example `/mlce-website/`).
- Retain the existing stylesheet and basic project structure; add `assets/images/` only when images are actually required.
- Avoid unnecessary dependencies, scripts, animations and large assets.

## Design and content guidelines

- Style: **simple, clean, modern, academic and professional**.
- Prioritize readability, clear headings, concise copy and generous whitespace.
- Maintain a responsive layout for desktop, tablet and mobile.
- Preserve a consistent visual identity and reuse existing CSS variables and styles.
- Use restrained imagery; prefer authentic research/project visuals supplied or approved by the group over generic stock images.
- Write website copy in clear **English**, using concise and technically accurate wording.
- Avoid marketing hype and unsupported claims such as “world-leading” or “pioneering”.
- Preserve the exact approved subtitle and the three application-area names unless explicitly asked to change them.

## Accessibility and quality

- Use logical heading hierarchy, semantic landmarks and descriptive link text.
- Provide meaningful alt text for informative images and empty alt text for purely decorative ones.
- Ensure keyboard accessibility, visible focus states and readable contrast.
- Respect `prefers-reduced-motion` where motion is used.
- Check links between all six pages, current-page highlighting, and the skip-to-content anchor beneath the sticky header on small screens.
- Keep HTML and CSS readable and formatted for reviewable Git diffs.

## Workflow for Codex

1. Inspect the relevant files before making changes.
2. Make the **smallest focused change** that satisfies the request.
3. Preserve existing approved content, navigation, visual design and working behavior unless a change is explicitly requested.
4. If content is missing or uncertain, flag the gap instead of making up facts.
5. After changes, check internal links, responsive behavior and relevant accessibility concerns as far as available tools allow.
6. Summarize which files changed, what was changed, and what the user should verify in the browser.
7. **Do not commit, push or deploy** unless explicitly asked. The user controls publication.

## Existing source material

Use the group's CIMNE research page, Fernando Salazar's personal academic website and the MLCE group presentation as content references when they are supplied or accessible. Do not assume those sources are fully up to date; confirm personnel and project status before publishing substantive updates.

Reference URLs:
- https://cimne.com/research/research-clusters/machine-learning-and-models-in-hydro-environmental-engineering/machine-learning-in-civil-engineering/
- https://sites.google.com/view/fernando-salazar-gonzalez
