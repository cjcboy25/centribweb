# Centribuild Construction Services — Static Website

Astro static website based on the 2026 Centribuild company profile.

## Stack
- Astro
- Markdown blog content
- GitHub Pages deployment
- Custom domain: `senbuilds.ph`

## Local development

```bash
npm install
npm run dev
```

Open the VM's IP address on port 4321 from the host laptop:

`http://VM_IP:4321`

The dev server is configured with `--host 0.0.0.0`.

## Build

```bash
npm run build
npm run preview
```

## Content updates

Blog posts live in:

`src/content/blog/`

Add a Markdown file with frontmatter:

```md
---
title: "Your article title"
description: "SEO description"
pubDate: 2026-09-10
category: "Construction"
hero: "/images/blog/example.jpg"
---

Article content here.
```

Then commit and push:

```bash
git add .
git commit -m "Add blog post"
git push
```

GitHub Actions builds and publishes the site.

## Important brand note

The supplied company profile identifies the business as **Centribuild Construction Services**, while the requested domain is **senbuilds.ph**. The site therefore keeps the Centribuild brand in the content and uses `senbuilds.ph` as the deployment/domain target.

## Excluded from this MVP

- Organizational Chart
- Permits and Certifications

These are intentionally not included in the navigation or page content yet.
=======
# centribweb
Centribuild Web Portfolio