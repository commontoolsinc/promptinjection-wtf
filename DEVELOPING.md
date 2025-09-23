# Development & Deployment

This repository contains the source code for promptinjection.wtf, hosted on GitHub Pages.

## Structure

- `docs/` - Contains all website files for GitHub Pages deployment
- `docs/index.html` - Main landing page

## Local Development

To work on the site locally:

1. Make changes to files in the `docs/` folder
2. Open `docs/index.html` directly in your browser to preview

## Deployment

### GitHub Pages (Automatic)

The site automatically deploys to GitHub Pages when changes are pushed to the `main` branch.

**Setup Steps (one-time):**

1. Go to your repository settings on GitHub
2. Navigate to "Pages" in the sidebar
3. Under "Source", select "Deploy from a branch"
4. Select branch: `main` and folder: `/docs`

**Deployment Process:**
- Push to `main` branch triggers automatic deployment
- GitHub automatically serves the `docs/` folder
- Site becomes available at `https://<username>.github.io/promptinjection.wtf`

### Custom Domain (promptinjection.wtf)

To use the custom domain:

1. In repository settings → Pages, add `promptinjection.wtf` as custom domain
2. Create a `docs/CNAME` file containing: `promptinjection.wtf`
3. Configure DNS records for promptinjection.wtf:
   - Add CNAME record pointing to `<username>.github.io`
   - Or add A records pointing to GitHub Pages IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153

## Adding New Pages

1. Create new HTML files in the `docs/` folder
2. Link to them from `index.html` or other pages
3. Push to `main` to deploy automatically