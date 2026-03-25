# Webparts360 Static Site

A lightweight, fast static version of the Webparts360 marketing website.

## Files

- index.html: Page structure and content
- styles.css: Visual style and responsive layout
- script.js: Mobile navigation and reveal animation

## Quick local preview

Use any static server, for example:

- Python: `python -m http.server 8080`
- Node: `npx serve .`

Then open `http://localhost:8080`.

## Host on GitHub Pages (recommended for this project)

This repo already includes a deployment workflow at `.github/workflows/deploy-pages.yml`.

### One-time setup

1. Create a GitHub repository and push this project to the `main` branch.
2. In GitHub, open repository `Settings` -> `Pages`.
3. Under `Build and deployment`, set `Source` to `GitHub Actions`.
4. Push any change to `main` to trigger deployment.
5. After the workflow completes, your site will be live at:
	- `https://<your-username>.github.io/<your-repo>/`

### If using a custom domain

1. In `Settings` -> `Pages`, set `Custom domain`.
2. Update your DNS records to point to GitHub Pages.
3. Enable HTTPS in the same screen once DNS propagates.

## Other cheap hosting options

1. Cloudflare Pages
- Cost: free tier available
- Best for: global CDN performance and simple Git-based deployments

2. Azure Static Web Apps
- Cost: free tier available
- Best for: tight Azure integration

## Form handling

The contact form currently uses a placeholder Formspree action URL.
Replace `https://formspree.io/f/your-form-id` in index.html with your actual endpoint.
