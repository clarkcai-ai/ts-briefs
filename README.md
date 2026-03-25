# Production Briefs

A single-page static web app for managing production brief data — job tracking, editing instructions, ad set recipes, and more.

## Deploying to GitHub Pages

1. Create a new repository on GitHub (e.g. `production-briefs`).
2. Push this repo:
   ```bash
   git remote add origin git@github.com:YOUR_USERNAME/production-briefs.git
   git push -u origin main
   ```
3. In the GitHub repo, go to **Settings > Pages**.
4. Under **Source**, select **Deploy from a branch**, choose `main`, root `/`, and click Save.
5. The site will be live at `https://YOUR_USERNAME.github.io/production-briefs/` within a minute or two.

No build step is needed — GitHub Pages serves `index.html` directly.

## Data Persistence

All brief data is stored in the browser's `localStorage`. This means data is local to each browser/device.

To transfer data between browsers or back up your work:

- **Export**: Click the **Export** button in the header to download a `.json` file containing all brief data.
- **Import**: Click the **Import** button and select a previously exported `.json` file to restore data.

## Local Development

Open `index.html` directly in a browser, or use any static file server:

```bash
npx serve .
```
