# Content & SEO Admin Workflow

## Recommended MVP: GitHub + Markdown

No database or CMS server is required.

1. Admin opens `src/content/blog/` in GitHub.
2. Creates a new `.md` file.
3. Adds SEO frontmatter: title, description, publication date, category, and optional hero image.
4. Writes the article in Markdown.
5. Opens a pull request for review, or commits directly to `main` for a trusted admin.
6. GitHub Actions builds and publishes the updated static site.

### Why this works well
- Very low cost.
- Version history for every article.
- Easy rollback.
- Excellent performance.
- No WordPress/database maintenance.
- Markdown is portable.

## Optional CMS later: Decap CMS

If non-technical SEO staff should have a form-based editor, add a `/admin` interface using Decap CMS. The CMS can manage Markdown files in GitHub, but GitHub authentication/OAuth must be configured separately. Do not expose repository credentials in browser code.

## Alternative: external headless CMS

For multiple editors, approval workflows, scheduled publishing, media libraries, and richer authoring, use a headless CMS such as Sanity, Contentful, or another service. Astro can fetch the content at build time and still publish a static site.

## SEO fields to maintain

Every post should have:
- SEO title
- Meta description
- Clean slug
- Primary topic/category
- Publication date
- Hero image + descriptive alt text
- Internal links to Services / Projects / Contact
- One clear call to action

## Suggested future content plan

- Construction planning guides
- Residential construction checklists
- Renovation and rehabilitation guides
- Roofing maintenance articles
- Project case studies
- Before/after project stories
- Materials and workmanship explainers
- Company/project updates

Avoid publishing unsupported claims. Keep technical, legal, engineering, and regulatory statements appropriately qualified.
