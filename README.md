# Awesome Recipes

A collection of awesome cooking recipes.

## How to Add a Post

### Filename rules

- Place posts in `_posts/`.
- Filename must follow the Jekyll convention: `YYYY-MM-DD-title.md` (lowercase, words separated by hyphens). Example: `2026-01-03-beef-bourguignon.md`.
- The date in the filename becomes the post date.

### YAML front matter template

Minimal recommended front matter (use this as a starting point):

```yaml
---
layout: post
title: "Your Post Title"
tags: Beef France Stew
---

# Your Post Title

## Ingredients
- Ingredients list here

## Instructions
1. Step-by-step instructions here

## Source
source link here
```

### Notes on the template

- `layout`: use `post` so the post template (post.html) is applied.
- `title`: human-readable title.
- `tags`: this project uses space-separated tags (e.g., `tags: Beef France Stew`). Be consistent.

### Tags guidance

- Use `tags` for fine-grained labels (ingredients, cuisine, technique).
- Stick to a consistent casing (e.g., TitleCase or lowercase) across posts.
- This repo uses space-separated tags (not YAML arrays). Example: `tags: Beef France Stew`.
