# todd-dsm.github.io

Personal portfolio site built with Astro + Tailwind CSS.

## Development

```bash
npm install
npm run dev      # Start dev server at localhost:4321
npm run build    # Build for production
npm run preview  # Preview production build
```

## Adding Content

### Blog Posts

Create a markdown file in `src/content/blog/`:

```markdown
---
title: "Your Post Title"
description: "Short description for cards and SEO"
date: 2026-02-05
tags: ["Tag1", "Tag2"]
featured: false
draft: false
---

Your content here. Supports full markdown.
```

The filename becomes the URL slug: `my-post.md` → `/blog/my-post`

### Portfolio Case Studies

Create a markdown file in `src/content/portfolio/`:

```markdown
---
title: "Project Title"
description: "Short description for cards"
date: 2024-01-01
tags: ["AWS", "Kubernetes"]
result: "82% cost reduction"
role: "Senior Engineer"
tech: ["EKS", "Terraform", "ArgoCD"]
featured: false
order: 4
---

## The Challenge

What problem needed solving.

## The Approach

How you solved it.

## The Result

Measurable outcomes.

## Lessons Learned

What you'd share with others.
```

Set `featured: true` for full-width display. Lower `order` values appear first.

## Deployment

Pushes to `main` trigger GitHub Actions → GitHub Pages deployment.
