Swift Creations Ltd — Software Development Agency 

This repository contains the static portfolio website for Swift Creations, a small agency showcasing projects and services. The site is implemented as a simple, responsive static site intended for easy deployment to any static-hosting provider.

**Project Highlights**
- **Single-file static site**: The site is delivered as `index.html` with linked assets under `assets/` for images, icons, and supporting files.
- **Minimal dependencies**: Built with plain HTML and Tailwind CSS utility classes (embedded or pre-built styles) so it’s fast and easy to host.
- **SEO & verification**: Includes `sitemap.xml` and `google6f233b25e4ac8348.html` for search-console verification.

**Table of Contents**
- **Project Overview**
- **Tech Stack**
- **Repository Structure**
- **Local Preview**
- **Deploying**
- **SEO & Analytics**
- **Accessibility & Performance Tips**
- **Customizing the Site**
- **Contributing**
- **License & Legal**

**Project Overview**
- **Purpose**: A marketing portfolio site to present Swift Creations' services, portfolio items, and company information.
- **Audience**: Prospective clients, partners, and search engines.

**Tech Stack**
- **HTML**: Markup lives in `index.html`.
- **CSS**: Tailwind CSS utility classes are used. The styles may be embedded or compiled into CSS that the page references.
- **Assets**: Images, icons, and other static assets live in the `assets/` directory.

**Repository Structure**
- `index.html`: Main entry point for the website.
- `assets/`: Images, icons, and other static resources.
- `google6f233b25e4ac8348.html`: Google Search Console verification file.
- `sitemap.xml`: Sitemap for search engines.
- `privacy-policy.html`, `terms-of-service.html`: Legal pages for site visitors.
- `LICENSE`: Project license.

**Local Preview**
You can preview the site locally in two common ways:

- Open the file directly in a browser: double-click `index.html` or open it from your browser (`File -> Open`).
- Start a simple HTTP server (recommended for testing resource paths):

```powershell
# From the project root (PowerShell)
python -m http.server 8000; Start-Process "http://localhost:8000"
```

Or, with PowerShell 5.1 only, you can run:

```powershell
# Using PowerShell's built-in listener (PowerShell 6+ provides simpler http server options)
npx http-server -p 8000
```

Then open `http://localhost:8000` in your browser.

**Deployment**
The site is ready for static hosting. Here are common hosts and steps:

- GitHub Pages
	- Create a public repository and push this folder as the repository root.
	- In the repo settings go to **Pages**, select branch `main` and folder `/ (root)`, then save.

- Vercel
	- Sign in to Vercel and import the Git repository.
	- Vercel will detect a static site and deploy automatically.

- Netlify
	- Drag and drop the project folder into Netlify’s dashboard or connect your Git repo.
	- Configure build settings if you use a Tailwind build step; otherwise, it's a simple static deploy.

**SEO & Analytics**
- `sitemap.xml` is included to help search engines index your pages.
- `google6f233b25e4ac8348.html` is a verification file for Google Search Console.
- Add an analytics snippet (e.g., Google Analytics, Plausible) inside `index.html` where appropriate.

**Accessibility & Performance Tips**
- Use semantic HTML elements (`header`, `nav`, `main`, `footer`) to improve accessibility and SEO.
- Provide `alt` attributes for images in `assets/`.
- Optimize images (WebP, compressed PNG/JPEG) and lazy-load large media.
- Minify HTML/CSS for production.

**Customizing the Site**
- To change content, edit `index.html` directly.
- To update images or icons, add or replace files in `assets/` and update the file paths in `index.html`.
- If you manage Tailwind locally, update your Tailwind config and rebuild your stylesheet before deployment.

**Contributing**
- This project is intentionally minimal. If you'd like to contribute:
	- Fork the repo and create a feature branch.
	- Make focused changes (content, accessibility, performance improvements).
	- Open a pull request with a clear description of the change.

**License & Legal**
- See the `LICENSE` file in the repository for licensing details.
- Privacy and Terms pages are included as `privacy-policy.html` and `terms-of-service.html` — update them to reflect your legal requirements.

**Troubleshooting**
- If images or assets fail to load when served from a subpath, verify relative paths in `index.html` and ensure your hosting configuration uses the repository root as the publish directory.

**Contact**
- For support or updates, edit the site content directly or open an issue in the repository.

Thank you for using Swift Creations' portfolio template — it's small, fast, and ready to deploy.
