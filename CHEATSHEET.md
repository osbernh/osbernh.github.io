# Website Cheat Sheet

## Preview locally

```bash
cd /Users/osbern/Documents/Website_Academic/osbernh.github.io
bundle exec jekyll serve
```

Open <http://127.0.0.1:4000>

## Publish changes

```bash
cd /Users/osbern/Documents/Website_Academic/osbernh.github.io
git add .
git commit -m "Update website"
git push
```

## Edit the main sidebar info

Edit:

`/Users/osbern/Documents/Website_Academic/osbernh.github.io/_config.yml`

Important fields:

- `author.avatar`
- `author.name`
- `author.bio`
- `author.location`
- `author.employer`
- `author.uri`
- `author.email`
- `author.googlescholar`
- `author.orcid`
- `author.github`

## Edit the main pages

- Home: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/_pages/about.md`
- Research: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/_pages/research.md`
- Publications page: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/_pages/publications.html`
- Teaching page: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/_pages/teaching.html`
- CV page: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/_pages/cv.md`

## Add a blog post

Create a file in:

`/Users/osbern/Documents/Website_Academic/osbernh.github.io/_posts/`

Filename format:

`YYYY-MM-DD-title.md`

Example:

```md
---
title: "My New Post"
date: 2026-03-26
permalink: /posts/my-new-post/
tags:
  - research
---

Write here.
```

## Add a publication

Create or copy a file in:

`/Users/osbern/Documents/Website_Academic/osbernh.github.io/_publications/`

## Add a teaching item

Create or copy a file in:

`/Users/osbern/Documents/Website_Academic/osbernh.github.io/_teaching/`

## Replace files

- Portrait image: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/images/Portrait.jpg`
- CV PDF: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/files/CV.pdf`
