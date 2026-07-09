# fMRI Methods & Tools blog

A minimal Jekyll blog hosted on GitHub Pages.

## One-time setup

1. Create a repository on GitHub named **`YOUR_USERNAME.github.io`**
   (this exact name makes it a personal site served at
   `https://YOUR_USERNAME.github.io`).
2. Put all these files in the repository root and push them.
3. On GitHub: **Settings → Pages**. Under "Build and deployment", set
   **Source = Deploy from a branch**, branch = `main`, folder = `/ (root)`.
   Save.
4. Wait ~1 minute, then open `https://YOUR_USERNAME.github.io`.

Before pushing, edit `_config.yml`, `about.md`, and the post to replace every
`YOUR_...` placeholder with your real name / username / repo link.

## Writing a new post

Add a file in `_posts/` named `YYYY-MM-DD-title.md`. The date in the filename
matters — it's how Jekyll orders and dates posts. Each file starts with a
"front matter" block:

```
---
layout: post
title: "My post title"
date: 2026-07-15
categories: tools
---

Write your post here in Markdown.
```

Commit and push — the site rebuilds automatically. New posts appear on the
home page.

## Optional: preview locally before pushing

You don't have to, but if you want to see the site on your own machine first:

```
gem install bundler jekyll
bundle init
# add: gem "github-pages", group: :jekyll_plugins   to the Gemfile
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```
