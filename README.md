# MLCE preliminary research group website

Static website for the Machine Learning in Civil Engineering (MLCE) group at CIMNE.

## File structure

- `index.html`: Home, group identity, About Us and three Research Areas.
- `research.html`: Methods & Technologies.
- `people.html`: Researchers and PhD Students.
- `projects.html`: Selected Projects.
- `publications.html`: Selected Publications and academic profile links.
- `friends.html`: Friends & Collaborators.
- `styles.css`: shared styles, responsive layouts, and accessibility rules.
- `README.md`: development and publishing instructions.
- `AGENTS.md`: repository guidance and approved site structure.

The website uses only HTML and CSS. No installation, build step, or external dependencies are required.

## Local development

1. Clone `https://github.com/cimnemadrid/MLCE_Website.git`, or open your existing checkout.
2. Open `index.html` directly in a web browser.
3. Edit the HTML or CSS in your preferred text editor, save, and refresh the browser.

Keep all six HTML files and `styles.css` together at the repository root. Use relative page and asset paths so they work both locally and under the GitHub Pages repository path. Every page can be opened directly in a browser.

The navigation and footer are repeated in each HTML file. When changing either, update all six copies. Keep the same menu order and set `aria-current="page"` only on the current page's navigation link. All presentation rules belong in the shared stylesheet.

Before publishing:

- Check the desktop layout and a narrow mobile viewport.
- Follow each navigation link from every page and confirm the correct page is highlighted.
- Press Tab to reveal “Skip to content”, then Enter to move focus to the main content.
- Enable reduced motion in your operating system or browser developer tools and confirm anchor navigation no longer scrolls smoothly.

Navigation links use relative filenames such as `people.html`; the skip link uses `#main-content` on each page. Sticky-header anchor offsets are controlled by `--anchor-offset` in `styles.css`; review them if the header or navigation changes.

## Publish to GitHub Pages

Repository: [cimnemadrid/MLCE_Website](https://github.com/cimnemadrid/MLCE_Website).

1. In the repository, open **Settings -> Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select `main` and `/(root)`, then **Save**. Keep all six HTML files and `styles.css` at the repository root.
4. When ready to publish reviewed changes, commit them and push to `main`. GitHub Pages publishes updates from that branch automatically.
5. Check the deployment status in the repository's **Actions** tab and the published URL in **Settings -> Pages**.

Expected website address: [cimnemadrid.github.io/MLCE_Website](https://cimnemadrid.github.io/MLCE_Website/).

Local edits do not publish until committed and pushed to the publishing branch. No custom workflow or build tooling is needed for this setup.

Photographs remain neutral placeholders until approved images are supplied. Old single-page bookmarks such as `index.html#people` should be updated to the corresponding page, such as `people.html`.
