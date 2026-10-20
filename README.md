# MLCE preliminary research group website

Static website for the Machine Learning in Civil Engineering (MLCE) group at CIMNE.

## File structure

- `index.html`: all website content and section navigation.
- `styles.css`: shared styles, responsive layouts, and accessibility rules.
- `README.md`: development and publishing instructions.

The website uses only HTML and CSS. No installation, build step, or external dependencies are required.

## Local development

1. Clone `https://github.com/fersa/mlce-website.git`, or open your existing checkout.
2. Open `index.html` directly in a web browser.
3. Edit the HTML or CSS in your preferred text editor, save, and refresh the browser.

Keep `styles.css` beside `index.html`. Use relative paths for local assets so they work both locally and under the GitHub Pages repository path.

Before publishing:

- Check the desktop layout and a narrow mobile viewport.
- Follow each navigation link and confirm the destination is visible below the sticky header.
- Press Tab to reveal “Skip to content”, then Enter to move focus to the main content.
- Enable reduced motion in your operating system or browser developer tools and confirm anchor navigation no longer scrolls smoothly.

Keep section IDs aligned with navigation links. Sticky-header anchor offsets are controlled by `--anchor-offset` in `styles.css`; review them if the header or navigation changes.

## Publish to GitHub Pages

Repository: [fersa/mlce-website](https://github.com/fersa/mlce-website).

1. In the repository, open **Settings -> Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select `main` and `/(root)`, then **Save**. Keep `index.html` and `styles.css` at the repository root.
4. When ready to publish reviewed changes, commit them and push to `main`. GitHub Pages publishes updates from that branch automatically.
5. Check the deployment status in the repository's **Actions** tab and the published URL in **Settings -> Pages**.

Expected website address: [fersa.github.io/mlce-website](https://fersa.github.io/mlce-website/).

Local edits do not publish until committed and pushed to the publishing branch. No custom workflow or build tooling is needed for this setup.

Note: This version contains placeholders for unfinished sections and is intended as a starting point.
